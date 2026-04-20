# wms-logistique[README.md](https://github.com/user-attachments/files/26886777/README.md)
# WMS Firebase

Cette version remplace Node.js + Pinggy par **GitHub Pages + Firebase**.

## Ce que cette version garde
- Accueil avec 2 choix : **WMS** ou **Passer commande**
- Articles persistants
- Commandes persistantes
- Réinitialisation de la démo
- Signal sonore quand une commande urgente/réelle arrive
- QR code HTTPS sur la page d'accueil
- Scan manuel des SKU
- Compatible GitHub Pages

## Ce qu'il faut faire

### 1. Créer un projet Firebase
Va sur https://firebase.google.com/ et crée un projet.

### 2. Activer Firestore
Dans Firebase Console :
- Build
- Firestore Database
- Create database
- Start in test mode

### 3. Récupérer la config Web
Dans Project settings > General > Your apps > Web app

Tu auras un bloc comme :

```js
const firebaseConfig = {
  apiKey: "...",
  authDomain: "...",
  projectId: "...",
  storageBucket: "...",
  messagingSenderId: "...",
  appId: "..."
};
```

### 4. Remplacer dans `index.html`
Remplace les valeurs :
- `A_REMPLACER`
- `A_REMPLACER`
- etc.

### 5. Publier sur GitHub
Dépose `index.html` dans un repo GitHub puis active GitHub Pages.

## Important
Cette version utilise Firestore pour garder les articles et commandes en mémoire dans le temps.
