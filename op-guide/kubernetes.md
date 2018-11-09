---
title: TiDB Deployment on Kubernetes
summary: Use TiDB Operator to quickly deploy a TiDB cluster on Kubernetes
category: operations
---

# TiDB Deployment on Kubernetes

[TiDB Operator](https://github.com/pingcap/tidb-operator) manages TiDB clusters on [Kubernetes](https://kubernetes.io) 
and automates tasks related to operating a TiDB cluster. It makes TiDB a truly cloud-native database.

> **Warning:** Currently, TiDB Operator is work in progress [WIP] and is NOT ready for production. Use at your own risk.

<main class="tabs">
  <input id="tabGoogle" type="radio" name="tabs" checked>
  <label for="tabGoogle" class="label__png">GCP</label>
  <input id="tabLocal" type="radio" name="tabs">
  <label for="tabLocal" class="label__png">Local</label>
  <section id="GoogleContent">
    <h3>Google Kubernetes Engine (GKE)</h3>
    <p>The TiDB Operator tutorial for GKE runs directly in the Google Cloud Shell.</p>
    <a href="https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/pingcap/tidb-operator&tutorial=docs/google-kubernetes-tutorial.md"><img src="https://gstatic.com/cloudssh/images/open-btn.png"/></a>
  </section>
  <section id="LocalContent">
  <h3>Local installation using Docker in Docker</h3>
  <p>Docker in Docker (DinD) runs Docker containers as virtual machines and runs another layer of Docker containers inside the first layer of Docker containers. <code>kubeadm-dind-cluster</code> uses this technology to run the Kubernetes cluster in Docker containers. TiDB Operator uses a modified DinD script to manage the DinD Kubernetes cluster.</p>

  <a href="https://github.com/pingcap/tidb-operator/blob/master/docs/local-dind-tutorial.md">Continue reading tutorial on GitHub<span class="continue__arrow"></span></a>
  </section>
</main>