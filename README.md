# aksdsexample
AKS Deamon Set Example

This is a Deamon Set example to apply a configuration that should have normaly been done when creating the Cluster/Node Pool : https://learn.microsoft.com/en-us/azure/aks/custom-node-configuration 

On this example we will change the vm.max_map_count to 262144.

# Usage :
```
kubectl apply -f https://raw.githubusercontent.com/jopalhei/aksdsexample/main/ds.yaml
```

#Note 
This is just an example on how to use the Daemon Set to apply custom configurations to the AKS Nodes.
Manually doing changes is not supported so Daemon Sets should be used : https://learn.microsoft.com/en-us/azure/aks/support-policies#shared-responsibility 
