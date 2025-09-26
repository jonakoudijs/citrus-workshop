# Opdracht 3

Activeer de ingress controller:
```sh
minikube addons enable ingress
```

---

Bekijk `opdracht-3.yaml` onder **manifests/** en pas dit toe:
```sh
kubectl apply -f manifests/opdracht-3.yaml
```

Bekijk het ingress object:
```sh
kubectl get ingress -n opdracht-3
```