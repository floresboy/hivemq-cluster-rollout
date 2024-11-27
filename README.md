# HiveMQ Virtual Machine Cluster / Kamiels version

master commit 2,2 
added API listeners
added probes



This template deploys a n-Node HiveMQ cluster to Azure.

Be aware that the nodes will get a local IP adress. This migh be disassociated later and access can take place ov er a bastion host


The following resources will be deployed bis this template:
- n Virtual Machines with HiveMQ and the HiveMQ Azure Cluster Discovery Extension installed
- An Azure Storage Account used by the Extension
- An Availability Set in which the Virtual Machines are placed
- An Azure Load Balancer used to access the HiveMQ services
- A Virtual Network in which the Virtual Machines and Load Balancer are placed 
- Network Interfaces with Public IP-Addresses for the Virtual Machines
- A Network Interface with a Public IP-Address for the Load Balancer

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ffloresboy%2Fhivemq-cluster-rollout%2Frefs%2Fheads%2Fmaster%2Fazuredeploy.json)