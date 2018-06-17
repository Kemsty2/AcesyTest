## Prérequis

- Minikube installé
- Docker installé

## Liste des Commandes Que j'ai utilisé

#### Clone the repository
`git clone {repository_remote_url}`

#### Deploy minikube
`sudo minikube start`

#### Deploy minikube dashboard
`sudo minikube dashboard`

#### Write DockerFile Suits for the deployment of the stateful application
`J'ai utilisé OwnCloud, je pense qu'il est déjà configuré donc je n'ai pas écris de DockerFile`

#### Write k8s deployments file
- `Read owncloud_deployement.yaml, Fichier de deploiement basique, j'ai pas gèré la base de donnée`
- `sudo kubectl create -f . deployer owncloud`
- `sudo kubectl expose deployment owncloud-test  --type="NodePort" --port 8080`
- `sudo minikube service owncloud-test --url , pour recuperer l'adresse ip de l'application owncloud deployé`
- `sudo kubctl proxy, faire pointer mon cluster vers localhost:8001`
-  `je recupère l'adresse ip puis je lance`

#### Conclusion
- J'ai obtenu aucun resultat, ni le dashboard, ni owncloud ne veut s'afficher sur mon navigateur. 
- Si demain tu es à l'ecole, tu peux passer on fait le TP ensemble?

