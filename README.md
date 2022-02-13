<h1 align="center">FCFS 6 - Kubernetes Challenge</h1>

## Running the app

First you need to install [Kind](https://kind.sigs.k8s.io/), then:

```bash
$ kind create cluster --config=kind.yml
$ kubectl cluster-info --context kind-imersao-fsfc6

$ kubectl apply -f deployment.yml
$ kubectl apply -f service.yml

$ kubectl port-forward service/nginx-service 80

#run on http://localhost:80
```
