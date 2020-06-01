# HTTP Infrastructure

```
Author : Sacha Perdrizat, Pablo Mercado
```

## Step 6 Extra: LoadBalancing

Dans cette étape bonus nous allons configurer un Loadbalancer pour permettre la répartition des requêtes à travers plusieurs noeud applicatif.

### Traefik
Nous allons pour ce faire changer notre infrastructure dès maintenant pour découvrir un nouveau reverse proxy ``Traefik``. Traefik possède beaucoup de fonctionnalités très pertinentes pour la gestion des noeud, la principal étant qu'il est conçu pour s'intégrer très simplement avec docker (la configuration des noeud est automatique). Nous aurons besoin d'un autre outil docker-compose.

### docker-compose
Très brièvement, docker-compose nous permet de définir dans un fichier ``docker-compose.yml`` un équivalent des commande que nous écrirons au lancement d'un container, cela nous épargne la tâche d'avoir à stocker le lancement du container dans un script mais surtout il est possible de définir plusieurs lancement de container dans le même fichier.
