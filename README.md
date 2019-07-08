# Setup-Amplify-Mesh-Governance

A Wiki page created as a quick start guide to building an Amplify Central managed Service Mesh hosted on a Kubernetes Cluster. 
We are providing this initial outline for AWS/EC2 plus Kubernetes, other k8s infrastructure will be coming in the future.

Read our [setup wiki](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki) to build, prepare and deploy Amplify Mesh Governance. 

Notes: 
- These steps are based on having a Linux client available to install the required tools to manage an AWS EC2 instance.
- The AMPLIFY Central Mesh Governance feature is currently only enabled for the primary (ie, original) API Admin account for your organization.  It will not be visible if your role is API Developer or Consumer.

## Prepare your client and Kubernetes cluster

If you already have the tools needed to manage an EC2 instance on Amazon Web Services (AWS) then skip to Step 2.

[Step 1](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-1.-Install-required-tools-to-manage-the-AWS-EC2-instance). Install required tools to manage the EC2 instance (AWS CLI, Kubectl, Kops, Helm).
Here is a link to pull a docker client image that has the tools already in place: [Link](https://github.com/u1i/amplify-cli) 

If you already have a Kubernetes cluster within an AWS/EC2 environment then skip to Step 3.

[Step 2](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-2.-Create-a-Kubernetes-cluster-with-Kops). Create a kops cluster within the AWS/EC2 Kubernetes Environment and setup DNS.

## Prepare your cluster for the Axway Mesh Agents

- We have options for exposing an HTTP or HTTPS mesh gateway to host the APIs proxied on the cluster.
- And we have HTTPS options with different levels of certificate trust (and outline the impacts of those).

[Step 3](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-3.-Prepare-Kubernetes-cluster-for-Amplify-Central-Service-Mesh-Agents). Prepare Kubernetes cluster for Amplify Central Service Mesh Agents.

## Add the Axway Mesh Agents

[Step 4](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-4.-Create-an-Amplify-Central-environment-and-connect-your-Kubernetes-cluster-to-it). Create an Amplify Central environment and connect your Kubernetes cluster to it.

## Manage your OnPrem cluster

[Step 5](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-5.-Remove-the-Axway-Mesh-and-Agents-from-your-Cluster)  Later, remove the Axway Mesh and Agents from your cluster.

[Step 6](https://github.com/Axway/Setup-Amplify-Mesh-Governance/wiki/Step-6.--Delete-the-Cluster).  Later, delete the Cluster when no longer needed.
