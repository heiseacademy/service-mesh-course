# Netzwerkumleitung durch linkerd

## Links

* https://linkerd.io/2/features/cni/

## Kommandos

  * `kubectl apply -f nginx-iptables.yaml`
  * `kubectl exec -ti nginx<tab> -- sh` (bei diesem Kommando den Podnamen durch Shellcompletion mittels `<tab>` geben lassen)
  * `iptables -L -t nat -n`

## Aktualisierungen und Anmerkungen

Das `Dockerfile` in diesem Verzeichnis enthält die Definition des Containers, den wir für die Experimente nutzen. 