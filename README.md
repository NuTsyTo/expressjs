# ExpressJS

Ce repos contient une appli express.js de type " Hello world " pour tester le déploiement.

## Installation

```bash
git clone https://github.com/NuTsyTo/expressjs
cd expressjs
npm install
```

## Utilisation

```bash
node app.js
```

[https://localhost:3000] (https://localhost:3000)

## Déploiement sur render.com

Prérequis : Avoir un compte Github

- (optionnel) Créer ou Forker un repository sur Github si nécessaire.
- Créer un compte sur [https://render.com/](https://render.com/)
- Créer un nouveau web service en cliquant sur l'icône « + »
- Choisissez l'option « Build and deploy from a Git repository »
- Cliquez sur « Connect account » dans la section « Github » à droite 
  Vous vous retrouvez sur le site de Github
- Tapez votre mot de passe Github
- Sélectionner le repository que vous voulez publier
- Confirmer les permissions accordés
  Vous revenez sur le site de Render
- Cliquez sur le bouton « Connect » du repository que vous voulez publier
- Remplissez les champs avec les données suivantes : 

```
Name: [sous-domaine-de-votre-appli]
Region: Frankfurt (EU Central)
Branch: main
Root Directory: <nc>
Build Command: npm install
Start Command: node app.js
Instance Type: Free
```

Remplacez `[sous-domaine-de-votre-appli]` par le sous-domaine souhaité.
Exemple: `foo` donnera `https://foo.onrender.com`

- Validez la configuration puis visitez le lien quand le build est temriné

### Mise à jour sur render.com

- Mettez le code à jour en local
- Commitez votre code avec `git add` et `git commit`
- Poussez votre code sur github avec `git push`
- Vérifiez que le code est à jour sur render.com
