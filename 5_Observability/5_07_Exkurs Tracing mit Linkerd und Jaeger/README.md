## Exkurs Distributed Tracing

## Links

* https://linkerd.io/2019/08/09/service-mesh-distributed-tracing-myths/ 
* https://linkerd.io/2/tasks/distributed-tracing/  

## Kommandos

* `kubectl get deploy -n linkerd-jaeger`
* `kubectl apply -f tracing.yaml`
* `kubectl port-forward service/frontend-proxy 8080:8080`
* `linkerd jaeger dashboard`

## Aktualisierungen und Anmerkungen
