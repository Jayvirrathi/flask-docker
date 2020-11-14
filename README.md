## Docker Kubernetes nodejs


### Docker Image
```
docker build . -t jayvirrathi/flask:v1

docker push jayvirrathi/flask:v1
```

### Docker run
```
docker run -p 5001:5000 -d jayvirrathi/flask:v1
```

### Kubernetes cmd
```
kubectl create ns example-app

kubectl apply -n example-app -f .\deployment\deployment.yaml

kubectl apply -n example-app -f .\deployment\service.yaml

kubectl -n example-app get svc
```


### Kubernetes cmd for Debugging
```
kubectl get ns

kubectl -n example-app get deploy

kubectl -n example-app get pods

kubectl -n example-app get logs podname
```



