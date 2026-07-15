# Examen final EDW2

## Identification

- Prénom : Nawel
- Nom : Labiedh

## Liens publics

- [Dépôt GitHub](https://github.com/nawellabiedh/edw2-examen-final-nawel-labiedh)
- [Site déployé sur N0C](https://e2596222.webdevmaisonneuve.ca/edw2-examen-final-nawel-labiedh/)

## Étapes réalisées

1. J'ai cloné le projet fourni avec Git.
2. J'ai modifié la page d'accueil pour ajouter mon nom.
3. J'ai créé un dépôt public sur mon compte GitHub.
4. J'ai ajouté un nouveau remote nommé `rendu`.
5. J'ai envoyé mon projet vers mon dépôt GitHub.
6. Je me suis connecté à N0C en SSH avec le port 5022.
7. J'ai récupéré mon dépôt sur N0C avec `git clone`.
8. J'ai déplacé le projet dans le dossier `public_html`.
9. J'ai testé le site dans le navigateur.

## Commandes Git utilisées

| Commande | Rôle |
| --- | --- |
| `git clone` | Récupérer une copie du projet sur mon ordinateur. |
| `git status` | Vérifier l'état des fichiers dans le dépôt. |
| `git add` | Préparer les fichiers pour le prochain commit. |
| `git commit` | Enregistrer une version du projet. |
| `git remote add` | Ajouter un nouveau remote vers mon dépôt GitHub. |
| `git remote -v` | Vérifier la liste des remotes configurés. |
| `git push` | Envoyer les commits vers GitHub. |

## Déploiement sur N0C

Je me suis connecté à N0C avec SSH en utilisant la commande `ssh -p 5022 mpwdebqghn@209.16.158.126`. Ensuite, j'ai récupéré mon dépôt public GitHub avec `git clone` dans le dossier `public_html`. J'ai vérifié le site dans le navigateur à l'adresse `https://e2596222.webdevmaisonneuve.ca/edw2-examen-final-nawel-labiedh/` et j'ai confirmé que ma page d'accueil affichait mon nom.

## Réponses théoriques

### Question 1 — Client et serveur

Un client est un ordinateur ou un appareil qui envoie une requête, par exemple un navigateur web. Un serveur est une machine qui reçoit cette requête et renvoie une réponse, comme une page web. Le navigateur agit comme client : il envoie la demande au serveur, qui lui retourne le contenu du site.

### Question 2 — Adresse IP, domaine et sous-domaine

Une adresse IP est un identifiant numérique unique pour chaque appareil connecté à un réseau. Un domaine est un nom facile à retenir qui remplace une adresse IP. Un sous-domaine est un sous-ensemble d'un domaine existant.

| Type | Description | Exemple |
| --- | --- | --- |
| Adresse IP | Identifiant numérique d'un appareil | 209.16.158.126 |
| Domaine | Nom principal d'un site web | google.com |
| Sous-domaine | Sous-ensemble d'un domaine | mail.google.com |

### Question 3 — Ports réseau

Un port réseau est un numéro qui identifie un service ou une application spécifique sur un serveur. Il permet de diriger le bon trafic vers le bon service.

| Port | Service associé | Utilité |
| ---: | --- | --- |
| 22 | SSH | Connexion sécurisée à distance |
| 80 | HTTP | Transfert de pages web non sécurisé |
| 443 | HTTPS | Transfert de pages web sécurisé |

### Question 4 — HTTP et HTTPS

HTTP est un protocole de transfert de données non sécurisé. HTTPS est la version sécurisée qui chiffre les données grâce à un certificat SSL. HTTPS est important pour un site public car il protège les données des utilisateurs et inspire confiance.

### Question 5 — SSH et N0C

SSH est un protocole qui permet de se connecter à distance à un serveur de manière sécurisée. Je l'utilise pour me connecter à N0C afin de déployer mon projet et gérer les fichiers sur le serveur.

### Question 6 — Dépôt GitHub public

Un dépôt GitHub public facilite le déploiement sur N0C car on peut le cloner directement sur le serveur avec `git clone` sans avoir besoin d'ajouter de clé SSH ou de configuration supplémentaire. Le serveur peut accéder au dépôt librement.

## Difficultés rencontrées

J'ai rencontré un problème avec le nom de domaine pour accéder à mon site sur N0C. Le domaine `node35-ca.n0c.com` ne fonctionnait pas dans le navigateur. J'ai trouvé la bonne adresse `e2596222.webdevmaisonneuve.ca` en testant le fichier `test.php` existant sur le serveur.
