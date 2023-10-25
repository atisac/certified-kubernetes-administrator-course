# Kubernetes Security Primitives
  - Take me to [Video Tutorial](https://kodekloud.com/topic/kubernetes-security-primitives/)
  
In this section, we will take a look at Kubernetes security primitives

## Secure Hosts

 ![sech](../../images/sech.PNG)
  
  Root access disabled.
  Password-based authentication should be disabled.
  
## Secure Kubernetes

The kube-API server is the center of all operations within Kubernetes.
We interact with it through the kubectl utility or accessing the API directly and through that you can do almost any operations on the cluster.
So that's the first line of defense. Controlling the access to the API server itself 

- We need to make two types of decisions.
  - Who can access it?
  - What can they do?
 
  ![seck](../../images/seck.PNG)
  
## Authentication
- Who can access the API Server is defined by the Authentication mechanisms.
- There are different ways to authenticate to the API server.
     - Files - username and passwords
     - files - username and tokens
     - certificates
     - External authentication providers like LDAP
     - finally for machines we create Service account
  
## Authorization
- Once they gain access to the cluster, what they can do is defined by authorization mechanisms.
   - RBAC (role based access control) authorization, where users are associated with groups with specific permissions.
   - ABAC, attribute-based access control
   - Node Authorization
   - webhook mode

## TLS Certificates
- All communication with the cluster, between the various components such as the ETCD Cluster, kube-controller-manager, scheduler, api server, as well as those running on the working nodes such as the kubelet and Kubeproxy is secured using TLS encryption.

 ![tls](../../images/tls.PNG)
 
## Network Policies
What about communication between applications within the cluster? 
By default, all pods can access all other pods within the cluster. you can restrict access between them using network policies.

  ![np](../../images/np.PNG)
  
