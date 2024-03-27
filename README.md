# nvidia-driver-k8s

Enable nvidia GPU on Kubernetes using an Ansible playbook. 

My specific version of the GPU is P2000.
The OS is Rocky Linux 9.3


# Installing NVIDIA GPU DRIVER on BARE METAL K8s Nodes
```
ansible-playbook -i <IP_ADDRESS>, nvidia-baremetal-node.yml
```

# Then install on control node
```
ansible-playbook -i <IP_ADDRESS>, nvidia-kubernetes-control.yml
```
