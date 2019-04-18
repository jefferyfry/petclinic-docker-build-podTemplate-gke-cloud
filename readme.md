# PetClinic Docker Build Pod Template Example for GKE

This is an example of running an existing Jenkins 2 master on a VM with a GKE cluster using the [Kubernetes plugin](https://github.com/jenkinsci/kubernetes-plugin). This allows running an agent pod template on the cluster to handle pipeline tasks. See the [podTemplate folder](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gke/tree/master/podTemplate) and the [Jenkinsfile](https://github.com/jefferyfry/spring-petclinic-docker-build-podTemplate-gke/blob/master/Jenkinsfile) for details. This pipeline runs a maven build, docker build, pushes the image to docker hub and then deploys the application to the same cluster. The petclinic application is then externally accessible via the load balancer IP.



