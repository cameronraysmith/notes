+++
title = "How can one setup an inexpensive gke kubernetes cluster with no load balancer using terraform running jupyter hub with instances a containerized jupyter notebook with multiple kernels on Arch Linux?"
author = ["Cameron Smith"]
lastmod = 2020-09-20T18:03:52-04:00
slug = "How_can_one_setup_an_inexpensive_gke_kubernetes_cluster_with_no_load_balancer_using_terraform_running_jupyter_hub_with_instances_a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux"
draft = false
+++

## [setup an inexpensive gke kubernetes cluster with no load balancer using terraform]({{< relref "setup_an_inexpensive_gke_kubernetes_cluster_with_no_load_balancer_using_terraform" >}}) running [jupyter hub]({{< relref "jupyter_hub" >}}) with instances [a containerized jupyter notebook with multiple kernels on Arch Linux]({{< relref "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux" >}})? {#setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform--setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform-dot-md--running-jupyter-hub--jupyter-hub-dot-md--with-instances-a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux--a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux-dot-md}


## An example of a single instance of jupyter lab is in [a containerized jupyter notebook with multiple kernels on Arch Linux]({{< relref "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux" >}}). I would like multiple users to be able to launch this container with scalable underlying computational infrastructure. An example of this is in [probcomp hosted jupyter hub]({{< relref "probcomp_hosted_jupyter_hub" >}}) {#an-example-of-a-single-instance-of-jupyter-lab-is-in-a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux--a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux-dot-md--dot-i-would-like-multiple-users-to-be-able-to-launch-this-container-with-scalable-underlying-computational-infrastructure-dot-an-example-of-this-is-in-probcomp-hosted-jupyter-hub--probcomp-hosted-jupyter-hub-dot-md}


## steps {#steps}

\*\*


### <span class="org-todo done DONE">DONE</span> Create [a containerized jupyter notebook with multiple kernels on Arch Linux]({{< relref "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux" >}}) {#create-a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux--a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux-dot-md}


### <span class="org-todo done DONE">DONE</span> Run [setup an inexpensive gke kubernetes cluster with no load balancer using terraform]({{< relref "setup_an_inexpensive_gke_kubernetes_cluster_with_no_load_balancer_using_terraform" >}}) {#run-setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform--setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform-dot-md}


### <span class="org-todo done DONE">DONE</span> Get [jupyter hub]({{< relref "jupyter_hub" >}}) running on the [kubernetes]({{< relref "kubernetes" >}}) cluster via integration of [use kubernetes on gke with terraform to deploy jupyter hub]({{< relref "use_kubernetes_on_gke_with_terraform_to_deploy_jupyter_hub" >}}) with  [setup an inexpensive gke kubernetes cluster with no load balancer using terraform]({{< relref "setup_an_inexpensive_gke_kubernetes_cluster_with_no_load_balancer_using_terraform" >}}) {#get-jupyter-hub--jupyter-hub-dot-md--running-on-the-kubernetes--kubernetes-dot-md--cluster-via-integration-of-use-kubernetes-on-gke-with-terraform-to-deploy-jupyter-hub--use-kubernetes-on-gke-with-terraform-to-deploy-jupyter-hub-dot-md--with-setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform--setup-an-inexpensive-gke-kubernetes-cluster-with-no-load-balancer-using-terraform-dot-md}


### <span class="org-todo done DONE">DONE</span> setup https certificates {#setup-https-certificates}


### <span class="org-todo done DONE">DONE</span> setup github group-based oauth authentication on [use kubernetes on gke with terraform to deploy jupyter hub]({{< relref "use_kubernetes_on_gke_with_terraform_to_deploy_jupyter_hub" >}}) {#setup-github-group-based-oauth-authentication-on-use-kubernetes-on-gke-with-terraform-to-deploy-jupyter-hub--use-kubernetes-on-gke-with-terraform-to-deploy-jupyter-hub-dot-md}


### <span class="org-todo done DONE">DONE</span> setup [multiple profiles to let users select their environment](<https://zero-to-jupyterhub.readthedocs.io/en/latest/customizing/user-environment.html#using-multiple-profiles-to-let-users-select-their-environment>) {#setup-multiple-profiles-to-let-users-select-their-environment--https-zero-to-jupyterhub-dot-readthedocs-dot-io-en-latest-customizing-user-environment-dot-html-using-multiple-profiles-to-let-users-select-their-environment}


### <span class="org-todo done DONE">DONE</span> Specify [a containerized jupyter notebook with multiple kernels on Arch Linux]({{< relref "a_containerized_jupyter_notebook_with_multiple_kernels_on_Arch_Linux" >}}) as the default image on this [jupyter hub]({{< relref "jupyter_hub" >}}) cluster {#specify-a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux--a-containerized-jupyter-notebook-with-multiple-kernels-on-arch-linux-dot-md--as-the-default-image-on-this-jupyter-hub--jupyter-hub-dot-md--cluster}


### <span class="org-todo todo TODO">TODO</span> Control the ability to scale the CPU-based backend {#control-the-ability-to-scale-the-cpu-based-backend}

<!--list-separator-->

-  setup a [dedicated node pool for jupyterhub users](<https://zero-to-jupyterhub.readthedocs.io/en/latest/administrator/optimization.html#using-a-dedicated-node-pool-for-users>)


### <span class="org-todo todo TODO">TODO</span> Investigate the potential for supporting GPU-based backends {#investigate-the-potential-for-supporting-gpu-based-backends}
