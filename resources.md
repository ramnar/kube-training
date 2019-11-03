## Sample Pod Yaml Definition

```shell
apiVersion: v1
kind: Pod
metadata:
  name: mypod
  labels:
    app: nginx
spec:
  containers:
  - name: mycontainer 
    image: nginx
```

## Sample Replicaset Yaml Definition

```shell
apiVersion: apps/v1
kind: ReplicaSet
metadata:
  name: myreplicaset
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app:: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: mycontainer
        image: nginx
```

## Sample Deployment Yaml Definition

```shell
apiVersion: apps/v1
kind: Deployment
metadata:
  name: mydeployment
  labels:
    app: nginx
spec:
  replicas: 3
  selector:
    matchLabels:
      app:: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: mycontainer
        image: nginx
```


## Sample ClusterIP Service Yaml Definition

```shell
apiVersion: v1
kind: Service
metadata:
  name: myservice
spec:
  selector:
    app: nginx
  type: ClusterIP 
  ports:
    - protocol: TCP
      port: 80
      targetPort: 9376


```

## Sample NodePort Service Yaml Definition

```shell
apiVersion: v1
kind: Service
metadata:
  name: my-service
spec:
  selector:
    app: nginx
  type: NodePort 
  ports:
    - protocol: TCP
      port: 80
      targetPort: 9376



```
