# mTLS mit Linkerd

## Links

* https://linkerd.io/2.10/tasks/securing-your-service/
* https://linkerd.io/2.10/tasks/using-the-debug-container/ 

## Kommandos

* `kubectl apply -f basic_with_profiles.yaml`
* `kubectl apply -f loadgenerator.yaml`

* `linkerd viz edges -n demo deployment` 
* `linkerd viz tap -n demo deploy`

* `kubectl get -n demo deploy frontend -o yaml| linkerd inject --enable-debug-sidecar -| kubectl apply -f -`
* `watch kubectl get -n demo pod`
* tshark Output aus den Logs: `kubectl -n demo logs deploy/frontend linkerd-debug -f |less`

* `kubectl apply -f unmeshed.yaml`
* Diagnose Container verbinden -> `kubectl exec -ti deploy/unmeshed -- sh`
* `linkerd viz dashboard &`
* Im Container `curl -i speakers:8081`

## Aktualisierungen und Anmerkungen
