# DApp - Application de Vote Blockchain

## 🔧 Equipe : Team _MetaMask_

### ⭐ Répartition du travail
- **LECLERCQ Tom** : Développement du smart contract, tests et liaison back/front.
- **BRUNEL Bastien** : Développement du smart contract, tests et mise en place de Git.
- **BEAUREPAIRE Paul** : Conception et développement du front-end de l'application.

---

## 🔍 Explication du projet
Nous avons développé une application de vote sur la blockchain en respectant les critères demandés pour l'interface web.

### 🔄 Fonctionnalités supplémentaires ajoutées
1. **Modification de vote** : Les utilisateurs peuvent modifier leur vote tant que l'administrateur n'a pas fermé la session de vote.
2. **Système de quorum dynamique** : Un quorum minimal de participation est requis parmi les utilisateurs de la whitelist. Tant que ce quorum n'est pas atteint sur une des propositions, l'application empêche de passer à l'étape suivante.

### 🔬 Tests
Nous avons mis en place des tests automatisés pour vérifier la fiabilité et la sécurité du système.

---

## 🎥 Démonstration
Une vidéo de démonstration est disponible à l'adresse suivante : **[Insérer le lien ici]**

---

## 🛠️ Guide d'installation et d’utilisation

### 💻 Back-end
#### Compilation du projet
```sh
npx hardhat compile


Lien de la vidéo démonstrative : 
### Back-end
compiler le projet : 
```sh
npx hardhat compile```
si erreur permission denied :
```sh
chmod +x node_modules/.bin/hardhat && npx hardhat compile```
Lancer la blokchain :
```sh
npm hardhat node```
Déployer le smart sur la blokchain
```sh
npx hardhat run ignition/modules/deploy.ts --network localhost```
Changer l'adresse du contrat dans le fichier front/app/page.tsx
### Front-end
lancer le projet
```sh
npm run dev```
si permission denied : 
```sh
sudo npm install -g next```
### Metamask
ajouter le réseau local dans metamask
```Network Name: Hardhat
New RPC URL: http://127.0.0.1:8545/ 
Chain ID: 31337 ```
Importer des comptes locaux dans metamask

