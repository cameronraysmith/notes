+++
title = "kubernetes on gke with terraform"
author = ["Cameron Smith"]
lastmod = 2020-09-24T23:08:37-04:00
slug = "kubernetes_on_gke_with_terraform"
draft = false
+++

## [kubernetes]({{< relref "kubernetes" >}}), [cloud computing]({{< relref "cloud_computing" >}}), [google cloud platform]({{< relref "google_cloud_platform" >}}) {#kubernetes--kubernetes-dot-md--cloud-computing--cloud-computing-dot-md--google-cloud-platform--google-cloud-platform-dot-md}


## simple setup for just a cluster {#simple-setup-for-just-a-cluster}


### create a cluster with terraform on gke {#create-a-cluster-with-terraform-on-gke}

<!--list-separator-->

-  <https://github.com/terraform-google-modules/terraform-google-kubernetes-engine>

<!--list-separator-->

-  <https://www.github.com/gruntwork-io/terraform-google-gke/tree/master/main.tf>

    <!--list-separator-->

    -  source:: <https://www.google.com/amp/s/cloudblog.withgoogle.com/products/devops-sre/deploying-a-production-grade-helm-release-on-gke-with-terraform/amp/>


### create an unmanaged cluster on linode {#create-an-unmanaged-cluster-on-linode}

<!--list-separator-->

-  <https://github.com/linode/terraform-linode-k8s>

<!--list-separator-->

-  <https://www.linode.com/docs/applications/configuration-management/terraform/how-to-provision-an-unmanaged-kubernetes-cluster-using-terraform/>


## holistic organization setup {#holistic-organization-setup}


### overview of cloud foundation toolkit: <https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/blob/master/docs/terraform.md> {#overview-of-cloud-foundation-toolkit-https-github-dot-com-googlecloudplatform-cloud-foundation-toolkit-blob-master-docs-terraform-dot-md}


### example:: integration of cloud foundation modules: <https://github.com/terraform-google-modules/terraform-example-foundation> {#example-integration-of-cloud-foundation-modules-https-github-dot-com-terraform-google-modules-terraform-example-foundation}

<!--list-separator-->

-  <https://github.com/terraform-google-modules/terraform-google-bootstrap>


### select modules from the cloud-foundation-fabric: <https://github.com/terraform-google-modules/cloud-foundation-fabric> {#select-modules-from-the-cloud-foundation-fabric-https-github-dot-com-terraform-google-modules-cloud-foundation-fabric}


### create a project: <https://github.com/terraform-google-modules/terraform-google-project-factory> {#create-a-project-https-github-dot-com-terraform-google-modules-terraform-google-project-factory}


### create a cluster: <https://github.com/terraform-google-modules/terraform-google-kubernetes-engine> {#create-a-cluster-https-github-dot-com-terraform-google-modules-terraform-google-kubernetes-engine}


## links {#links}


### <https://www.terraform.io/docs/providers/google/guides/using%5Fgke%5Fwith%5Fterraform.html> {#https-www-dot-terraform-dot-io-docs-providers-google-guides-using-gke-with-terraform-dot-html}


### <https://github.com/terraform-google-modules/terraform-google-kubernetes-engine> {#https-github-dot-com-terraform-google-modules-terraform-google-kubernetes-engine}


### <https://github.com/terraform-google-modules/terraform-google-project-factory> {#https-github-dot-com-terraform-google-modules-terraform-google-project-factory}


### <https://www.linode.com/docs/applications/configuration-management/terraform/how-to-provision-an-unmanaged-kubernetes-cluster-using-terraform/> {#https-www-dot-linode-dot-com-docs-applications-configuration-management-terraform-how-to-provision-an-unmanaged-kubernetes-cluster-using-terraform}

-   Use Terraform, the popular orchestration tool by HaschiCorp, to deploy a Kubernetes cluster on Linode. Linode’s Terraform K8s module creates a Kubernetes cluster running on the CoreOS ContainerLinux operating system. After creating a Master and worker nodes, the module connects through SSH to these instances and installs kubeadm, kubectl, and other Kubernetes binaries to /opt/bin. It also handles initializing kubeadm, joining worker nodes to the master, and configuring kubectl. For the cluster’s container networking interface, Calico is installed. Finally, a kubectl admin config file is installed to the local environment, which you can use to connect to your cluster’s API server.
