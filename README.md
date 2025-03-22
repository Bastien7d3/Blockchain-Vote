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
Une vidéo de démonstration est disponible à l'adresse suivante : **[https://youtu.be/bp6QqcsULPs](https://youtu.be/bp6QqcsULPs)**

---

# 🛠️ Guide d'installation et d’utilisation

## 💻 Back-end
### Compilation du projet
```sh
npx hardhat compile
```

Si une erreur "permission denied" survient :
```sh
chmod +x node_modules/.bin/hardhat && npx hardhat compile
```

### Lancer la blockchain locale
```sh
npx hardhat node
```

### Déployer le smart contract sur la blockchain locale
```sh
npx hardhat run ignition/modules/deploy.ts --network localhost
```

Après le déploiement, modifier l'adresse du contrat dans le fichier `front/app/page.tsx`.

## Front-end

### Lancer le projet
```sh
npm run dev
```

Si une erreur "permission denied" survient :
```sh
sudo npm install -g next
```

## Configuration de Metamask

### Ajouter le réseau local dans Metamask
- **Nom du réseau** : Hardhat
- **Nouvelle URL RPC** : `http://127.0.0.1:8545/`
- **Chain ID** : `31337`

### Importer des comptes locaux dans Metamask
Utilisez les clés privées générées par Hardhat pour importer des comptes locaux dans Metamask.
