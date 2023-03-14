<h1 align="center">
<br>
  <a href="README.md"><img src="docs/images/cluster-k8s.png" alt="Cluster diagram"></a>
  <br>
    <br>
  Bootstrapping Kubenetes Cluster with kubeadm on Virtual Box
  <br>
</h1>

<h4 align="center">🦖 Detail explain step-by-step for beginner.</h4>
<p align="center">Reference to K8s documentation - section <a href="https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/">Bootstrapping clusters with kubeadm.</a><br>This tutorial walks you through setting up Kubernetes Cluster on a local machine using VirtualBox.<br>We will use Vagrant to automate provisioning VirtualBox's VM.</p>

<p align="center">
  <a href="https://www.vagrantup.com/">
    <img src="https://img.shields.io/badge/-Vagrant-1868F2?logo=vagrant&logoColor=white" alt="Vagrant">
  </a>
  <a href="https://www.virtualbox.org/">
    <img src="https://img.shields.io/badge/-VirtualBox-183A61?logo=VirtualBox&logoColor=white" alt="Kubernetes">
  </a>
  <a href="https://kubernetes.io/">
    <img src="https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white" alt="Kubernetes">
  </a>
  <a href="https://containerd.io/">
    <img src="https://img.shields.io/badge/-containerd-575757?logo=containerd&logoColor=white" alt="containerd">
  </a>
    <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg??style=flat&logo=appveyor" alt="Licence MIT">
  </a>
</p>

<p align="center">
  <a href="README.md">🇺🇸</a>
  <a href="">🇻🇳</a>
</p>

### Before you begin
* 🖥️ Cluster diagram: 1 Control Plan & 2 Node.
* 💿 Instructions for Linux disto based on Debian and Red Hat. (I will use Ubuntu)
* ⚙️ System resources: at least 2 GB of RAM and 2 CPUs per machine.
* 🌐 Full network connectivity between all machines in the cluster (public or private network is fine).
* 📮 Unique hostname, MAC address, and product_uuid for every node.
* 🛠 Must disable [swap](https://github.com/kubernetes/kubernetes/issues/53533) in order for the kubelet to work properly.
* ➡️ Certain ports will be open on your machines. See [here](https://kubernetes.io/docs/reference/networking/ports-and-protocols/) for more details.
* 🔐 The client certificates generated by kubeadm will be expired after 1 year. See [here](https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-certs/) for more details.

### Step-by-step tutorial

- [ ] [Provision VirtualBox's VM with Vagrant](docs/Provision-VirtualBoxVM-with-Vagrant.md)
- [ ] [Installing a container runtime (containerd) on all virtual machines](docs/Installing-a-container-runtime.md)
- [ ] [Installing kubeadm, kubelet and kubectl on all virtual machines](docs/Installing-kubeadm-kubelet-kubectl.md)
- [ ] [Boostraping control plane and node](docs/Configuring-a-cgroup-driver.md)
