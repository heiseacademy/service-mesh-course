# Retrys und Timeout

## Links

* https://linkerd.io/2.10/tasks/configuring-timeouts/ 
  
## Kommandos

* `kubectl apply -f timeout_basis.yaml`
* `kubectl apply -f loadgenerator.yaml` 
* `linkerd viz dashboard`
* `kubectl apply -f add_timeouts.yaml` 

* `linkerd viz tap -n demo deploy/frontend --to service/schedule` 

* `kubectl exec -ti deploy/frontend --container linkerd-debug -- sh`
* In der Shell des Debug Containers: `curl -i schedule:8083`

* `watch linkerd viz routes -n demo deploy/frontend --to service/schedule -o wide`

## Aktualisierungen und Anmerkungen