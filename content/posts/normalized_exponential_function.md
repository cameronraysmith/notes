+++
title = "normalized exponential function"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:21-04:00
slug = "normalized_exponential_function"
draft = false
+++

## also known as the [softmax function]({{< relref "softmax_function" >}}) {#also-known-as-the-softmax-function--softmax-function-dot-md}


### <https://en.wikipedia.org/wiki/Softmax%5Ffunction> {#https-en-dot-wikipedia-dot-org-wiki-softmax-function}


## \\[p(\mathcal{C}\_k \vert x) = \frac{\exp(a\_k)}{\Sigma\_j \exp(a\_j)}\\] {#p--mathcal-c-k-vert-x--frac-exp--a-k--sigma-j-exp--a-j}


## where \\[a\_k = \ln p(\mathbf{x} \vert \mathcal{C}\_k) p(\mathcal{C}\_k)\\] {#where-a-k-ln-p--mathbf-x-vert-mathcal-c-k--p--mathcal-c-k}


## the [softmax function]({{< relref "softmax_function" >}}) terminology derives from the fact that if \\[a\_k > a\_j\\] for all \\[j \neq k\\] then \\[p(\mathcal{C}\_k) \approx 1\\] and \\[p(\mathcal{C}\_j) \approx 0\\] {#the-softmax-function--softmax-function-dot-md--terminology-derives-from-the-fact-that-if-a-k-a-j-for-all-j-neq-k-then-p--mathcal-c-k--approx-1-and-p--mathcal-c-j--approx-0}


##  {#}
