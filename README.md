
# Authentification-with-Kerberos

A brief description of what this project does and who it's for

Dans note cadre du projet nous avons utilisé deux machines virtuelles

Pour utiliser Kerberos nous avons deux contrainte, premièrement nous devons construire une DNS et
avoir une synchronisation d’horloge


## Synchronisation d’horloge

#### Machine 1: Serveur

#### output
![2ytxvy0x08t71](https://user-images.githubusercontent.com/80646711/236058600-7c5e47b0-08d2-43fd-a97e-fb971cf6db66.jpeg)![capture1](https://user-images.githubusercontent.com/74620773/236060565-effa6066-559b-4050-8431-545a83dcfa30.png)


#### Machine 2: Client
![capture1](https://user-images.githubusercontent.com/74620773/236060193-78ef15b5-d106-4684-a6ac-6ed18af79c2a.png)

#### output
## Configuration du DNS

#### Machine 1

#### output

#### Machine 2

#### output

### Verification de connexion

ici nous avons vérifié si les 2 machines se sont connecté entre elle

#### Machine 1

#### output
#### output


#### Machine 2

#### output
#### output
Une fois que nous avons vu que tout marche  et que notre environnement du travail a été préparer, nous somme enfin prêt pour l’installation de Kerberos et utiliser ces services
## Installation de Kerberos

#### Output

Dans les captures d’ecran ci-dessous c’est la premiere interface qui apparait lors de installation :c’est la configuration de keberos authentification

#### Output
#### Output
#### Output

Une fois que nous avons terminé l’installation, nous allons jeter un coup-œil au niveau des fichiers de configurations
Ici nous avons  les éléments qu’on a configurer lors de l’installations de Kerberos qui est en quelque sort le moteur ou le noyau

#### Output
#### Output
Apres l’installation, on va attribué un mot de passe pour le noyau avec la commande suivante :
#### Output
Verification
#### Output
Par la suite on va accéder au fichier kadm5.acl afin de pourvoir ajouter quelques modifications
#### Output
Ensuite on va créer des principaux
#### Output
Créer un utilisateur user :
#### Output
Afficher user qu’on vient de créer 
#### Output
Voir les information du user :
#### Output
Créer un ticket pour le service qui est l’angle host et on va le tester :
#### Output
Un aperçu pour voir comment on crée un ticket :
#### Output
Créer un host pour pouvoir ensuite l’authentifier ce service :
#### Output
Demarage des systèmes kerberos
#### Output
Apres on va passer a la creation de keytab et ajouter un algorithme de chiffrement :
#### Output
Verification du fichier kadm5.keytab
#### Output
#### Output
Une autre manière de créer un host :
#### Output

