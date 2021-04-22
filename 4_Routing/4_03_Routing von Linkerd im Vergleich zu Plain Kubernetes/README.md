# Vergleich zu Plain Kubernetes

## Links

* https://linkerd.io/2/reference/service-profiles/

## Kommandos

* `kubectl get services -n demo`
* `linkerd profile -n demo --open-api speaker.yaml speakers`
* `linkerd profile -n demo --open-api speaker.yaml speakers | kubectl apply -f -`
* `linkerd profile -n demo --template schedule | less`

## Aktualisierungen und Anmerkungen