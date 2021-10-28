# PetClinic Docker Build Pod Template Example for GKE

[![CIS](https://app.soluble.cloud/api/v1/public/badges/cb2d43a1-2f89-461d-8f12-ea0a569189ce.svg)](https://app.soluble.cloud/repos/details/github.com/jefferyfry/spring-petclinic-docker-build-podtemplate-gke)  [![IaC](https://app.soluble.cloud/api/v1/public/badges/5d4b775f-7875-495f-8fec-2cf706bce708.svg)](https://app.soluble.cloud/repos/details/github.com/jefferyfry/spring-petclinic-docker-build-podtemplate-gke)  

This is an example of running an existing Jenkins 2 master on a VM with a GKE cluster using the [Kubernetes plugin](https://github.com/jenkinsci/kubernetes-plugin). This allows running an agent pod template on the cluster to handle pipeline tasks. See the [podTemplate folder](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gke/tree/master/podTemplate) and the [Jenkinsfile](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gke/blob/master/Jenkinsfile) for details. This pipeline runs a maven build, docker build, pushes the image to docker hub and then deploys the application to the same cluster. The petclinic application is then externally accessible via the load balancer IP.



