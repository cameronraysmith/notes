+++
title = "service mesh"
author = ["Cameron Smith"]
lastmod = 2020-09-24T23:13:51-04:00
slug = "service_mesh"
draft = false
+++

## [kubernetes]({{< relref "kubernetes" >}}), [cloud computing]({{< relref "cloud_computing" >}}) {#kubernetes--kubernetes-dot-md--cloud-computing--cloud-computing-dot-md}


## a [service mesh](<https://en.wikipedia.org/wiki/Service%5Fmesh>) is a dedicated infrastructure layer for facilitating service-to-service communications between [microservices](<https://en.wikipedia.org/wiki/Microservices>), often using a [sidecar](<https://en.wikipedia.org/w/index.php?title=Sidecar%5Fsoftware%5Farchitecture>) [proxy](https://en.wikipedia.org/wiki/Proxy%5Fpattern). {#a-service-mesh--https-en-dot-wikipedia-dot-org-wiki-service-mesh--is-a-dedicated-infrastructure-layer-for-facilitating-service-to-service-communications-between-microservices--https-en-dot-wikipedia-dot-org-wiki-microservices--often-using-a-sidecar--https-en-dot-wikipedia-dot-org-w-index-dot-php-title-sidecar-software-architecture--proxy-dot}


## [servicemesh.es | Service Mesh Comparison](https://servicemesh.es/) {#servicemesh-dot-es-service-mesh-comparison}


### istio and linkerd are most popular. it appears that istio is more configurable while linkerd is potentially easier to get up and running. {#istio-and-linkerd-are-most-popular-dot-it-appears-that-istio-is-more-configurable-while-linkerd-is-potentially-easier-to-get-up-and-running-dot}


## example:: <https://istio.io/latest/docs/concepts/what-is-istio/> {#example-https-istio-dot-io-latest-docs-concepts-what-is-istio}


### ![](https://istio.io/latest/docs/ops/deployment/architecture/arch.svg) {#img}


### [Istio Service Mesh Explained](https://www.youtube.com/watch?v=6zDrLvpfCK4) {#istio-service-mesh-explained}

<!--list-separator-->

-  resources for installation and configuration

    <!--list-separator-->

    -  gateway

    <!--list-separator-->

    -  virtual service

    <!--list-separator-->

    -  destination rules

<!--list-separator-->

-  asdf

    <!--list-separator-->

    -  pilot

    <!--list-separator-->

    -  citadel

    <!--list-separator-->

    -  galley

    <!--list-separator-->

    -  being moved to proxy plane

        <!--list-separator-->

        -  telemetry

        <!--list-separator-->

        -  policy


### course:: [istio service mesh for kubernetes](https://www.youtube.com/playlist?list=PLNFIflbQ6VNtTBQEgIbgH0-oQ8NIBkMiJ) {#course-istio-service-mesh-for-kubernetes}

<!--list-separator-->

-  tools demonstrated

    <!--list-separator-->

    -  kiali

        <!--list-separator-->

        -  [Installing Istio and Kiali on Minikube (in a few minutes)](https://www.youtube.com/watch?v=0Ho1twJ9Udg)

    <!--list-separator-->

    -  jaeger ui

    <!--list-separator-->

    -  grafana


### install as standalone "operators" {#install-as-standalone-operators}

<!--list-separator-->

-  <https://istio.io/latest/docs/setup/install/standalone-operator/#prerequisites>

<!--list-separator-->

-  can use [terraform]({{< relref "terraform" >}}) "helm"
