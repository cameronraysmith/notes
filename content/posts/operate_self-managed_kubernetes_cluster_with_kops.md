+++
title = "operate self-managed kubernetes cluster with kops"
author = ["Cameron Smith"]
lastmod = 2020-09-20T17:37:23-04:00
slug = "operate_self-managed_kubernetes_cluster_with_kops"
draft = false
+++

## [kubernetes]({{< relref "kubernetes" >}}) cluster with [kops]({{< relref "kops" >}}) {#kubernetes--kubernetes-dot-md--cluster-with-kops--kops-dot-md}


## notes {#notes}


### use \*.k8s.local for gossip DNS which exposes the load balancer external ip to the public internet {#use-dot-k8s-dot-local-for-gossip-dns-which-exposes-the-load-balancer-external-ip-to-the-public-internet}


### create a self-managed cluster on gce from a yaml file {#create-a-self-managed-cluster-on-gce-from-a-yaml-file}

<!--list-separator-->

-  \`kops create -f cloud.yaml\`

<!--list-separator-->

-  cloud.yaml

    <!--list-separator-->

    -  \`\`\`clojure

        apiVersion: kops.k8s.io/v1alpha2
        kind: Cluster
        metadata:
          creationTimestamp: null
          name: cloud.k8s.local
        spec:
          api:
            loadBalancer:
              type: Public
          authorization:
            rbac: {}
          channel: stable
          cloudProvider: gce
          configBase: gs://quarere-clusters/cloud.k8s.local
          etcdClusters:


### cpuRequest: 200m {#cpurequest-200m}

etcdMembers:


### instanceGroup: master-us-central1-f {#instancegroup-master-us-central1-f}

  name: f
memoryRequest: 100Mi
name: main


### cpuRequest: 100m {#cpurequest-100m}

etcdMembers:


### instanceGroup: master-us-central1-f {#instancegroup-master-us-central1-f}

    name: f
  memoryRequest: 100Mi
  name: events
iam:
  allowContainerRegistry: true
  legacy: false
kubelet:
  anonymousAuth: false
kubernetesApiAccess:


### 0.0.0.0/0 {#0-dot-0-dot-0-dot-0-0}

kubernetesVersion: 1.17.6
masterPublicName: api.cloud.k8s.local
networking:
  kubenet: {}
nonMasqueradeCIDR: 100.64.0.0/10
project: quarere
sshAccess:


### 0.0.0.0/0 {#0-dot-0-dot-0-dot-0-0}

subnets:


### name: us-central1 {#name-us-central1}

  region: us-central1
  type: Public
topology:
  dns:
    type: Public
  masters: public
  nodes: public
addons:


### manifest: <https://raw.githubusercontent.com/kubernetes/kops/master/addons/kubernetes-dashboard/v2.0.1.yaml> {#manifest-https-raw-dot-githubusercontent-dot-com-kubernetes-kops-master-addons-kubernetes-dashboard-v2-dot-0-dot-1-dot-yaml}


### manifest: prometheus-operator {#manifest-prometheus-operator}

---

apiVersion: kops.k8s.io/v1alpha2
kind: InstanceGroup
metadata:
  creationTimestamp: null
  labels:
    kops.k8s.io/cluster: cloud.k8s.local
  name: master-us-central1-f
spec:
  image: cos-cloud/cos-stable-77-12371-114-0
  machineType: n1-standard-1
  maxSize: 1
  minSize: 1
  nodeLabels:
    kops.k8s.io/instancegroup: master-us-central1-f
  role: Master
  subnets:


### us-central1 {#us-central1}

zones:


### us-central1-f {#us-central1-f}

---

apiVersion: kops.k8s.io/v1alpha2
kind: InstanceGroup
metadata:
  creationTimestamp: null
  labels:
    kops.k8s.io/cluster: cloud.k8s.local
  name: nodes
spec:
  image: cos-cloud/cos-stable-77-12371-114-0
  machineType: n1-standard-1
  maxSize: 2
  minSize: 1
  preemptible: true
  nodeLabels:
    kops.k8s.io/instancegroup: nodes
  role: Node
  subnets:


### us-central1 {#us-central1}

zones:


### us-central1-f\`\`\` {#us-central1-f}


### load dashboard with \`kubectl proxy\`, [kubernetes docs web ui dashboard proxy](<https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/#command-line-proxy>) and \`dashboardlogin.sh\` {#load-dashboard-with-kubectl-proxy-kubernetes-docs-web-ui-dashboard-proxy--https-kubernetes-dot-io-docs-tasks-access-application-cluster-web-ui-dashboard-command-line-proxy--and-dashboardlogin-dot-sh}


### install jupyterhub with \`installjupyterhub.sh\` {#install-jupyterhub-with-installjupyterhub-dot-sh}


## questions {#questions}


### how can the kops cluster be setup to use preemptible nodes? {#how-can-the-kops-cluster-be-setup-to-use-preemptible-nodes}

<!--list-separator-->

-  it appears\`


### how can the kops cluster be setup for autoscaling {#how-can-the-kops-cluster-be-setup-for-autoscaling}


### how to complete the "configure jupyterhub" post-installation steps in this context {#how-to-complete-the-configure-jupyterhub-post-installation-steps-in-this-context}
