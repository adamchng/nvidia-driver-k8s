# nvidia-driver-k8s

Enable Nvidia GPU on Kubernetes using an Ansible playbook. 

My specific version of the GPU is P2000.

The OS is Rocky Linux 9.3

# Initial Steps
First download the Nvidia Driver for Linux to /usr/local/src. The version we are using is: NVIDIA-Linux-x86_64-525.105.17.run. 

If you are not using the same version, please update this in the nvidia_driver variable in nvidia-baremetal-node.yml.

# Installing NVIDIA GPU DRIVER on BARE METAL K8s Nodes
```
ansible-playbook -i <IP_ADDRESS>, nvidia-baremetal-node.yml
```

# Then install on control node
```
ansible-playbook -i <IP_ADDRESS>, nvidia-kubernetes-control.yml
```
