+++
title = "jupyter hub"
author = ["Cameron Smith"]
lastmod = 2020-09-24T23:06:44-04:00
slug = "jupyter_hub"
draft = false
+++

## technical overview {#technical-overview}


### <https://jupyterhub.readthedocs.io/en/stable/reference/technical-overview.html> {#https-jupyterhub-dot-readthedocs-dot-io-en-stable-reference-technical-overview-dot-html}


### ![](https://jupyterhub.readthedocs.io/en/stable/%5Fimages/jhub-parts.png) {#img}


## install jupyterhub {#install-jupyterhub}


### example:: <https://github.com/parente/z2jh-aws> {#example-https-github-dot-com-parente-z2jh-aws}

<!--list-separator-->

-  [Terraform](https://www.terraform.io/) for AWS infrastructure config management

<!--list-separator-->

-  Swap these for GCE vs GKE and GCR

    <!--list-separator-->

    -  [AWS Elastic Container Registry](https://aws.amazon.com/ecr/)%C2%A0(ECR) for storing custom JupyterHub and user images

<!--list-separator-->

-  <https://github.com/jupyterhub/helm-chart>

    -   [Helm](https://helm.sh)
    -   [Helmfile](https://github.com/roboll/helmfile) for deploying applications to Kubernetes including
        -   [external-dns](https://github.com/kubernetes-incubator/external-dns),
        -   [nginx-ingress](https://github.com/kubernetes/ingress-nginx),
        -   [jetstack/cert-manager](https://github.com/jetstack/cert-manager)

<!--list-separator-->

-  [Cloudflare](https://cloudflare.com/) for DNS

<!--list-separator-->

-  [Let's Encrypt](https://letsencrypt.org/) for TLS certificates

<!--list-separator-->

-  [Homebrew](https://brew.sh/) for installing client tools on macOS

<!--list-separator-->

-  [Make](https://www.gnu.org/software/make/) for simplifying local commands


### <https://zero-to-jupyterhub.readthedocs.io/en/latest/setup-jupyterhub/setup-jupyterhub.html> {#https-zero-to-jupyterhub-dot-readthedocs-dot-io-en-latest-setup-jupyterhub-setup-jupyterhub-dot-html}


### the zero-to-jupyterhub instructions use helm to install jupyterhub; however, we want to manage the installation with terraform. the terraform helm provider does this. {#the-zero-to-jupyterhub-instructions-use-helm-to-install-jupyterhub-however-we-want-to-manage-the-installation-with-terraform-dot-the-terraform-helm-provider-does-this-dot}

<!--list-separator-->

-  <https://github.com/hashicorp/terraform-provider-helm>


## configure jupyterhub {#configure-jupyterhub}


### List of all configurable values for jupyterhub {#list-of-all-configurable-values-for-jupyterhub}

<!--list-separator-->

-  <https://github.com/jupyterhub/zero-to-jupyterhub-k8s/blob/master/jupyterhub/values.yaml>


### Configure the login to use the account that makes sense to you (Google, GitHub, etc.). {#configure-the-login-to-use-the-account-that-makes-sense-to-you--google-github-etc-dot--dot}

<!--list-separator-->

-  <https://github.com/jupyterhub/oauthenticator>


### Use a suitable pre-built image for the user container or build your own: {#use-a-suitable-pre-built-image-for-the-user-container-or-build-your-own}

<!--list-separator-->

-  [a containerized jupyter notebook with multiple kernels on Arch Linux]({{< relref "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux" >}})


### Host it on [https://your-domain.com](https://your-domain.com/). {#host-it-on-https-your-domain-dot-com-dot}
