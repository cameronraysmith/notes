+++
title = "kubernetes"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:12-04:00
slug = "kubernetes"
draft = false
+++

## tutorials {#tutorials}


### [Learn Kubernetes Basics | Kubernetes](<https://kubernetes.io/docs/tutorials/kubernetes-basics/>) {#learn-kubernetes-basics-kubernetes--https-kubernetes-dot-io-docs-tutorials-kubernetes-basics}


### [Kubernetes the Hard Way Using Terraform \* YouTube](<https://www.youtube.com/watch?v=00r9C8rWsK8>) {#kubernetes-the-hard-way-using-terraform-youtube--https-www-dot-youtube-dot-com-watch-v-00r9c8rwsk8}

<!--list-separator-->

-  [kelseyhightower/kubernetes-the-hard-way: Bootstrap Kubernetes the hard way on Google Cloud Platform. No scripts.](<https://github.com/kelseyhightower/kubernetes-the-hard-way>)

<!--list-separator-->

-  [aidanSoles/kubernetes-the-hard-way-terraform: 🐳 Terraform-defined implementation of Kelsey Hightower's "Kubernetes The Hard Way" tutorial.](<https://github.com/aidanSoles/kubernetes-the-hard-way-terraform>)


### [Getting Started with Kubernetes: Use kubeadm to Deploy a Cluster on Linode | Linode](<https://www.linode.com/docs/kubernetes/getting-started-with-kubernetes/>) {#getting-started-with-kubernetes-use-kubeadm-to-deploy-a-cluster-on-linode-linode--https-www-dot-linode-dot-com-docs-kubernetes-getting-started-with-kubernetes}


## internal components {#internal-components}


### architecture {#architecture}

<!--list-separator-->

-  \![](![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fcameronraysmith%2FbcV3qoK7Z-.png?alt=media&token=786cd08e-c1d4-4ca9-b663-a20a5b0b34c9))

<!--list-separator-->

-  vocabulary

    <!--list-separator-->

    -  kubectl

    <!--list-separator-->

    -  cluster

    <!--list-separator-->

    -  master

    <!--list-separator-->

    -  node

    <!--list-separator-->

    -  kubelet

    <!--list-separator-->

    -  pod

    <!--list-separator-->

    -  container


### processes {#processes}

<!--list-separator-->

-  \![](![](https://i.octopus.com/docs/deployment-examples/kubernetes-deployments/deploy-container/deploy-container.svg))

<!--list-separator-->

-  vocabulary

    <!--list-separator-->

    -  ingress

    <!--list-separator-->

    -  service

        <!--list-separator-->

        -  \![](![](https://linuxacademy.com/site-content/uploads/2019/05/Screen-Shot-2019-04-17-at-10.58.43-AM-1024x769.png))

    <!--list-separator-->

    -  deployment

    <!--list-separator-->

    -  replicaset

    <!--list-separator-->

    -  operators

        <!--list-separator-->

        -  <https://github.com/operator-framework/getting-started>

        <!--list-separator-->

        -  \![](![](https://operatorhub.io/static/images/capability-level-diagram.svg))

        <!--list-separator-->

        -  [OperatorHub.io | The registry for Kubernetes Operators](<https://operatorhub.io/what-is-an-operator>)

            <!--list-separator-->

            -  example:: <https://operatorhub.io/operator/elastic-cloud-eck>

        <!--list-separator-->

        -  [Kubernetes Operators Explained \* YouTube](<https://www.youtube.com/watch?v=i9V4oCa5f9I&list=PLOspHqNVtKABAVX4azqPIu6UfsPzSu2YN&index=8>)

        <!--list-separator-->

        -  workflow

            <!--list-separator-->

            -  1. Basic installation

            <!--list-separator-->

            -  2. Upgrades

            <!--list-separator-->

            -  3. Lifecycle

            <!--list-separator-->

            -  4. Insights

            <!--list-separator-->

            -  5. Autopilot

        <!--list-separator-->

        -  Helm

            <!--list-separator-->

            -  "1. Basic installation"

            <!--list-separator-->

            -  "2. Upgrades"

        <!--list-separator-->

        -  Go / ansible

            <!--list-separator-->

            -  all aspects


### data persistence {#data-persistence}

<!--list-separator-->

-  \![](![](https://8gwifi.org/docs/img/kube-arch.png))

<!--list-separator-->

-


## accessories {#accessories}


### package management {#package-management}

<!--list-separator-->

-  [Helm](<https://helm.sh/docs/>) is a package manager for Kubernetes.

<!--list-separator-->

-  [What is Helm? \* YouTube](<https://www.youtube.com/watch?v=fy8SHvNZGeE&list=PLOspHqNVtKABAVX4azqPIu6UfsPzSu2YN&index=12>)


### [service mesh]({{< relref "service_mesh" >}}) {#service-mesh--service-mesh-dot-md}


### context switcher {#context-switcher}

<!--list-separator-->

-  <https://github.com/ahmetb/kubectx>


### continuous development {#continuous-development}

<!--list-separator-->

-  <https://skaffold.dev/docs/>
