+++
title = "Removing private files from the hugo posts folder"
author = ["Cameron Smith"]
lastmod = 2020-09-24T14:24:25-04:00
slug = "removing_private_files_from_the_hugo_posts_folder"
draft = false
+++

## Removing private files from public directory {#removing-private-files-from-public-directory}

The objective is to generate a script `move-private-md.sh` that can be run to temporarily move the markdown files in your hugo posts directory that you intend to keep private so that you can commit them to your git repository for public consumption. Another approach would be to add this list to a private `.gitignore` listing; however, this would not give you the ability to _toggle_ the private files in and out of your local hugo server so that you can view all of the org-roam files integrated prior to removing the private ones.

`org-babel-tangle` is used to write the code blocks script to be used whenever some private files need to be removed from the hugo posts folder which needs to be cleaned out prior to a git commit. After running `org-babel-tangle` with this file open from your `notes/org/private` directory, you can look at, review, and if comfortable with the content execute the script `move-private-md.sh`. It will print out the name of the temporary directory to which it has moved the copies of the md files with equivalent names to the org files in your `notes/org/private` directory.


## Write out a file containing the file listing {#write-out-a-file-containing-the-file-listing}

Here we need to list the files in a directory, and remove the files from another directory with the same root filename and a different extension.

```shell
ls *.org | wc -l
ls *.org > private-notes.txt
printf "\nListing of files intended to become private\n"
head -5 private-notes.txt
cat private-notes.txt | wc -l
```


## Transform the file extensions {#transform-the-file-extensions}

We will use `xargs -a filename.txt rm` to remove finally remove the files. This command expects the filenames to be exact. Since the target files are `md` rather than `org` files, we will use the python program `massedit` to replace the extension with a regular expression.

```shell
python -m massedit -e "re.sub(r'\.org', r'.md', line)" private-notes.txt > private-md.diff
head -8 private-md.diff
tail -5 private-md.diff
```

This demonstrates the transformation from `org` to `md` filenames with the same root name. Now we write the changes.

```shell
python -m massedit -e "re.sub(r'\.org', r'.md', line)" -w private-notes.txt
printf "\nListing of files intended to become private after substitution of org with md\n"
head -8 private-notes.txt
cat private-notes.txt | wc -l
```


## Moving the files that match the transformed listing {#moving-the-files-that-match-the-transformed-listing}

We are now ready to use `xargs -a private-notes.txt rm` to remove remove the specified files.

```shell
tail -5 private-notes.txt
pwd
cp private-notes.txt ~/projects/notes/content/posts
cd ~/projects/notes/content/posts
pwd
printf "\nNumber of md files in posts directory prior to removal\n"
ls *.md | wc -l

# create temporary directory
tmp_dir=$(mktemp -d -t org-roam-private-$(date +%Y-%m-%d-%H-%M-%S)-XXXXXXXXXX)
# xargs -a private-notes.txt -I{} rm {} # this would work with GNU xargs
tr '\n' '\0' < private-notes.txt | xargs -0 -I _ mv _ $tmp_dir # this works with BSD xargs

printf "\nNumber of md files in posts directory after to removal\n"
ls *.md | wc -l
printf "\nprivate markdown files moved to:
$tmp_dir\n
recover with:
mv $tmp_dir/*.md ~/projects/notes/content/posts
rm -fr $tmp_dir"
```

Now we check the number of remaining files in the directory. This should equal the number of files in the `org` directory.

```shell
pwd
ls ../*.org | wc -l
cd ~/projects/notes/content/posts
pwd
ls *.md | wc -l
```

Let's compare the files in the two directories.

```shell
pwd
ls ../*.org | wc -l
find ../ -name "*.org" -maxdepth "1"  -exec basename {} .po \; | sort > org-files.txt
ls ~/projects/notes/content/posts/*.md | wc -l
find ~/projects/notes/content/posts/ -name "*.md" -maxdepth "1"  -exec basename {} .po \; | sort > md-files.txt
python -m massedit -e "re.sub(r'\.org', r'', line)" -w org-files.txt
python -m massedit -e "re.sub(r'\.md, r'', line)" -w md-files.txt
head -5 org-files.txt
head -5 md-files.txt
# icdiff org-files.txt md-files.txt
```
