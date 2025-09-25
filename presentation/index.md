---
theme: gaia
_class: lead
paginate: true
---

<style>
section {
  background: #FFEC0A;
  color: #000;
}
h1 {
  color: #000;
}
</style>

![bg left:40% 80%](https://images.icon-icons.com/2699/PNG/512/kubernetes_logo_icon_168359.png)

# **Kubernetes Workshop**

https://github.com/jonakoudijs/citrus-workshop


---

# Wat is een container?

- Lichtgewicht, geïsoleerde omgeving voor applicaties
- Bevat alles wat nodig is om een app te draaien
- Consistent gedrag op elke omgeving
- Een image is een blauwdruk voor containers

<br/><br/>

> https://www.docker.com/resources/what-container

<!-- Containers zorgen ervoor dat een applicatie altijd hetzelfde werkt, ongeacht laptop, server. -->
<!-- Dit maakt ze ideaal voor moderne softwareontwikkeling. -->

---

# Verschil VM en Container

![width:1000px](img/vm-docker-comparison.png)

---

# Waarom Kubernetes?

- Automatische schaalbaarheid en herstel
- Efficiënt beheer van containers

<!-- Het zorgt ervoor dat applicaties automatisch kunnen schalen en herstellen bij fouten. -->
<!-- Zie het als een dirigent die je instructies geeft en die vervolgens constant jouw eindresultaat probeert uit te voeren. -->

---

# Wat is een Kubernetes cluster?

- Bestaat uit een Control Plane (Master) en Worker Nodes
- Control Plane: regelt en coördineert alles
- Worker Nodes: draaien de containers
- Controllers: bewaken en sturen bij

---

# Control Plane + Workers

![width:1000px](img/cluster-diagram-1.jpg)

---

# Cluster componenten

![width:1000px](img/cluster-diagram-2.jpg)

<!-- Op elke master en worker node zijn een aantal processen verantwoordelijk voor een stukje van Kubernetes. -->

---
# Kubernetes objecten

![bg left:50% 90%](img/kubernetes-objects.png)




- Pod
- Ingress
- Service
- Deployment
- Configmap / Secret
- Namespace

<!-- Pod: 1 of meerdere containers -->
<!-- Ingress: regelt toegang van buitenaf (bijv. via HTTP) -->
<!-- Service: maakt communicatie naar en tussen containers mogelijk -->
<!-- Deployment: definieert hoe en hoeveel containers moeten draaien -->
<!-- ConfigMap & Secret: beheren configuratie en gevoelige data -->
<!-- Namespace: logische verdeling van Kubernetes objecten. Scheiding van teams en verschillende omgevingen. -->