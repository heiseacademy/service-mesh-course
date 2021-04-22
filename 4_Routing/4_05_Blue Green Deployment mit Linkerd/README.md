# Blue Green Deployment

## Links

* https://martinfowler.com/bliki/BlueGreenDeployment.html 
  
## Kommandos

* `kubectl apply -f blue_green.yaml`
* `kubectl -n demo port-forward service/frontend-proxy 8080:8080` -> Altes Design
* `kubectl -n demo port-forward service/test-service 8080:8080` - >  Neues design!

* `kubectl apply -f switch_to_green.yaml`
* `kubectl -n demo port-forward service/frontend-proxy 8080:8080`

* `kubectl apply -f blue_green.yaml`
* `kubectl -n demo port-forward service/frontend-proxy 8080:8080` die alte Version ist wieder sichtbar

## Aktualisierungen und Anmerkungen