# gcloud_k8s_cluster_kubespray

## Prerequisites:

- 3 Ubuntu 18.04 instances

## Brief:

In this article we will create a cluster comprising of 1 master, 1 node, 1 bastion host (for the sake of simplicity and time). This will be achieved in a cloud independent fashion using the open-source deployment tool *kubespray*.

This will be done on google cloud, a high-level cloud; this too is for the sake of simplicity. However, as will be demonstarted, the cloud provider is not important. Kubespray operates by way of ansible playbooks (written in python) that provision the necessary components onto the machines, qualifying them as *nodes*. So, there is a pre-existing common framework that integrates itself effortlessly into the machines hardware; kubespray does not need to know who or what is providing the hypervisor for the machines soon-to-be nodes.

## Guide:

`ssh-keygen -t rsa`
