## Interacting With Applications in AKS using AGIC(Azure Application Gateway Ingress Controller)

### Description

- Will create an architecture that will allow to access the applications 
  behind Application Gateway in Azure.
- Applications will be running on AKS (Azure Kubernetes Service)
- AKS will be running in a private subnet that can not be accessed from outside.

### Steps to Follow

- Create a VNet in Azure under your subscription.
- Create a subnet for AKS, you can create this subnet while creating the
  cluster as well.
- Once cluster is created use the network option in cluster to enable the
  Application Gateway add-on.
- Once add-on is enabled, you will see an application gateway created with a public IP.
- You can use this public IP to point to your domain.
- expose your services with the help of kubernetes ingress.

### Broad Architecture and Various Components

![](AKS-With-AGIC/diagram/aks-with-agic.excalidraw.png)
