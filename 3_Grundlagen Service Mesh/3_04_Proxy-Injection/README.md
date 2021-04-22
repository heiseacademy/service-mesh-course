# Sidecar-Proxy Injection

## Links

## Kommandos

* `cat nginx.yaml | linkerd inject -`
* `cat nginx.yaml| linkerd inject --manual -| less`
* `linkerd inject nginx.yaml | kubectl apply -f -`
* `linkerd stat deployments` 
* `kubectl delete -f nginx.yaml`

* `kubectl get deploy -n linkerd` 
* `kubectl apply -f nginx.yaml`
* `kubectl get namespace default -o yaml | linkerd inject -` 
* `kubectl get namespace default -o yaml | linkerd inject -| kubectl apply -f -`
* `kubectl get pod`

## Aktualisierungen und Anmerkungen
