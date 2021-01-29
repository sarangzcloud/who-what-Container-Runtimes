# who-what-Container-Runtimes




Just Some info, before we begin

1. Container runtime/execution engine:

Also referred to commonly as the “container runtime,” this is any piece of software that is used to create, start and stop containers. Examples here include Docker Engine, Containerd, CRI-O etc.



2. runC: 

A tool for spawning and running containers based on Open Containers Initiative (OCI) runtime specification.



3. Containerd: 

A daemon that manages the lifecycle of containers on hosts, typically using runC. You can find more details about how runC and Containerd interact with each other in this blog post by Michael Crosby.



4. Docker Engine builds on top of Containerd which builds on top of runC.





Who is going with which container runtime?

1. AWS --containerd

https://aws.amazon.com/blogs/containers/under-the-hood-fargate-data-plane/



2. Azure -- Containerd default for AKS K8s v1.19 onwards.(earlier < v1.19 Moby-- Upstream Docker)

https://docs.microsoft.com/en-us/azure/aks/cluster-configuration



3. Redhat / Openshift / OKD

CRI-O is an open source, community-driven container engine.

Its primary goal is to replace the Docker service as the container engine for Kubernetes implementations, such as OpenShift Container Platform.

https://www.openshift.com/blog/whats-inside-openshift-4



4. GCP -- cos with containerd for GKE.

https://cloud.google.com/kubernetes-engine/docs/concepts/node-images



5. Bottlerocket -- Containerd

https://github.com/bottlerocket-os/bottlerocket



6 . Ubuntu -- Charmed Kubernetes -- Containerd

https://ubuntu.com/kubernetes/docs/container-runtime



7. Rancher -- Containerd

https://rancher.com/containerd-for-rancher-and-rancheros



IBM and Oracle ? -- WIP.







