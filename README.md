# Kubenetes
KubeAdmin_worker_Setup

This repository has installation steps for Kubenetes for both master (control plane nodes) and all worker nodes

#After installation for Master initialise control plane as root user
# Initialize Kubernetes control plane by running the below commond as root user.

sudo kubeadm init

To connect worker nodes to master, run control plane join token

kubeadm join 172.31.10.12:6443 --token cdm6fo.dhbrxyleqe5suy6e \
        --discovery-token-ca-cert-hash sha256:1fc51686afd16c46102c018acb71ef9537c1226e331840e7d401630b96298e7d
