# Opdracht 2

Maak als eerst de namespace aan:
```sh
kubectl create namespace opdracht-2
```
Controleer of de namespace is aangemaakt:
```sh
kubectl get namespaces
```

---

Start een pod met nginx:
```sh
kubectl run nginx --image=nginx --restart=Never --port=80 -n opdracht-2
```

Bekijk of de pod is gestart:
```sh
kubectl get pods -n opdracht-2
```

Stuur verkeer door naar de pod (voor test doeleinden):
```sh
kubectl port-forward pod/nginx 8080:80 -n opdracht-2
```

Verwijder de pod:
```sh
kubectl delete pod nginx -n opdracht-2
```

---

Bekijk `opdracht-2.yaml` onder **manifests/** en pas dit toe:
```sh
kubectl apply -f manifests/opdracht-2.yaml
```

Bekijk of de pod is gestart:
```sh
kubectl get pods -n opdracht-2
```

Verwijder de pod:
```sh
kubectl delete pod nginx -n opdracht-2
```