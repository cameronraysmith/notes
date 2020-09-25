+++
title = "setup an inexpensive gke kubernetes cluster with no load balancer using terraform"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:42-04:00
slug = "setup_an_inexpensive_gke_kubernetes_cluster_with_no_load_balancer_using_terraform"
draft = false
+++

## [cloud computing]({{< relref "cloud_computing" >}}), [google cloud platform]({{< relref "google_cloud_platform" >}}), [kubernetes]({{< relref "kubernetes" >}}), [terraform]({{< relref "terraform" >}}) {#cloud-computing--cloud-computing-dot-md--google-cloud-platform--google-cloud-platform-dot-md--kubernetes--kubernetes-dot-md--terraform--terraform-dot-md}


## affordable {#affordable}


## <https://www.terraform.io/docs/providers/google/guides/getting%5Fstarted.html> {#https-www-dot-terraform-dot-io-docs-providers-google-guides-getting-started-dot-html}


## introduction to terraform and gcp: 3 f1-micro preemptible VMs each with 10GB of storage at $5/mo {#introduction-to-terraform-and-gcp-3-f1-micro-preemptible-vms-each-with-10gb-of-storage-at-5-mo}


### <https://github.com/kasuboski/cheap-managed-kubernetes> {#https-github-dot-com-kasuboski-cheap-managed-kubernetes}


### [Cheap Managed Kubernetes with Terraform \* YouTube](<https://www.youtube.com/watch?v=gcwn3ETSvm8&t=25s>) {#cheap-managed-kubernetes-with-terraform-youtube--https-www-dot-youtube-dot-com-watch-v-gcwn3etsvm8-and-t-25s}


## terraform with one stable and free f1-micro instance and 2 preemptible f1-micro instances using XXX for load balancing {#terraform-with-one-stable-and-free-f1-micro-instance-and-2-preemptible-f1-micro-instances-using-xxx-for-load-balancing}


### <https://dev.to/verkkokauppacom/how-to-kubernetes-for-cheap-on-google-cloud-1aei> {#https-dev-dot-to-verkkokauppacom-how-to-kubernetes-for-cheap-on-google-cloud-1aei}


### <https://github.com/nkoson/gke-tutorial> {#https-github-dot-com-nkoson-gke-tutorial}


### notes {#notes}

<!--list-separator-->

-  use us-central1-f

    <!--list-separator-->

    -  <https://cloud.google.com/compute/docs/regions-zones>

<!--list-separator-->

-  create IAM default service account and download json key then check path specification

<!--list-separator-->

-  initialize terraform and bring up the cloud infrastructure.

    <!--list-separator-->

    -  need to check the organization and workspace names in terraform and update them in the code as well

<!--list-separator-->

-  check compute engine and clusters as well as the terraform site to make sure the deployment succeeded

<!--list-separator-->

-
