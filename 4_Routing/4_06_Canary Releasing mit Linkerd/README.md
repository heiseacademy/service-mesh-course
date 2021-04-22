# Canary Release

## Links

* https://martinfowler.com/bliki/CanaryRelease.html
* https://flagger.app/ 
  
## Kommandos

* `kubectl apply -f canary.yaml`
* `kubectl -n demo port-forward service/frontend-proxy 8080:8080` 
* `kubectl edit trafficsplit canary`

## Aktualisierungen und Anmerkungen