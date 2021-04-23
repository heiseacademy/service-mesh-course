# Retrys und Timeout

## Links

* https://linkerd.io/2.10/tasks/configuring-retries/
* https://linkerd.io/2019/02/22/how-we-designed-retries-in-linkerd-2-2/

## Kommandos

* `kubectl apply -f retry_basis.yaml`
* `kubectl apply -f loadgenerator.yaml`
* `linkerd viz dashboard`

* `kubectl apply -f add_failures_speaker.yaml` 
* `watch kubectl get po -n demo`
* `watch linkerd viz routes -n demo ns/demo --to service/speakers -o wide` 

* `kubectl apply -f add_retries.yaml`
* `watch linkerd viz routes -n demo ns/demo --to service/speakers -o wide` 

## Aktualisierungen und Anmerkungen
