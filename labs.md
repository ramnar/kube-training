# Kubernetes Labs

## YAML BASICS

1.  Create a yaml file containing the following properties -
    training - k8s, days - 2, participants - 10, room - coral, location - bangalore.
2.  Enhance the above yaml file to include the participant names in the training.
3.  Enhance the above yaml file to include the following curriculum topics and number of hours taken.
    yaml basics - 1hr, Pods - 2hrs, ReplicaSet - 2hrs, Deployment - 2hrs, Microservices - 3hrs

## POD

1.  Create a pod for nginx using yaml file.
2.  Check if the above pod is created successfully.
3.  Add a label env=dev to the yaml file and redeploy the pod.
4.  Try out the kubectl describe command on the above pod.
5.  In which node is the above pod running.
6.  Delete the above created pod.

## REPLICA SET

1.  Create a replicaset for nginx with three replicas using yaml file.
2.  Delete one pod and see what happens.
3.  Add a label env=dev to the pods of the replicaset.
4.  Increase the number of replicas to 4 in the above replicaset.
5.  View details of the above replicaset.
6.  Delete the above replicaset.

## DEPLOYMENT

1.  Create a deployment for nginx with three replicas using yaml file.
2.  View the pods and replica sets created.
3.  Add a label env=dev to the pods and update the deployment.
4.  Increase the number of replicas to 4 in the above replica set.
5.  View details of the above deployment.
6.  Delete the above deployment.
7.  RollingUpdate.

## SERVICE

1.  Create a deployment for web application. Try to access the application from browser
2.  Create a service of type ClusterIP for the above deployment. Do curl.
3.  Create another service of type NodePort for the above deployment.
4.  Access the above application from browser.

## MICROSERVICES

TODO

  

