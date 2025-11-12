# 📝 Mon Blog React - Projet de Formation MERN

> **Cours MERN - Semaine 6** : Introduction à React et Vite  
> **École Polytechnique de Sousse** - 5ème année

---

## 🎯 Objectif du Projet

Ce projet est une application de blog simple développée avec **React** et **Vite**, créée dans le cadre de l'apprentissage des fondamentaux de React. L'application affiche une liste d'articles de blog avec un en-tête et un pied de page.

---

## 🚀 Technologies Utilisées

- **React 18** - Bibliothèque JavaScript pour construire des interfaces utilisateur
- **Vite** - Outil de build ultra-rapide pour le développement frontend
- **JSX** - Syntaxe pour écrire du HTML dans JavaScript
- **JavaScript ES6+** - Version moderne de JavaScript

---

## 📂 Structure du Projet

```
mon-blog-react/
├── public/                  # Fichiers statiques
├── src/
│   ├── components/          # Composants React réutilisables
│   │   ├── Header.jsx      # En-tête de l'application
│   │   ├── Article.jsx     # Carte d'article individuel
│   │   └── Footer.jsx      # Pied de page
│   ├── App.jsx             # Composant principal
│   ├── main.jsx            # Point d'entrée de l'application
│   └── index.css           # Styles globaux
├── package.json            # Dépendances et scripts
├── vite.config.js          # Configuration Vite
└── README.md               # Documentation du projet
```

---

## 🎨 Composants Créés

### 1. **Header.jsx** - En-tête de l'Application
- **Props** : `title`, `subtitle`
- **Description** : Affiche le titre principal et le sous-titre de l'application
- **Style** : Fond bleu (#3b82f6), texte blanc, centré avec bordures arrondies

### 2. **Article.jsx** - Carte d'Article
- **Props** : `title`, `author`, `content`
- **Description** : Affiche un article de blog avec son titre, auteur et contenu
- **Style** : Fond violet clair (#8C88F4FF), bordures, padding généreux

### 3. **Footer.jsx** - Pied de Page
- **Props** : `author`, `year`
- **Description** : Affiche les informations de copyright et l'année actuelle
- **Style** : Texte centré, bordure supérieure, couleur grise

---

## 📊 Données de l'Application

L'application affiche **4 articles** sur les thèmes suivants :
1. **Introduction à React** - par Alice
2. **Qu'est-ce que Vite ?** - par Bob
3. **Les Composants en React** - par Charlie
4. **Le JSX en Pratique** - par Alice

---

## 🔑 Concepts React Implémentés

### ✅ **1. Composants**
Création de composants fonctionnels réutilisables :
```jsx
function Header({ title, subtitle }) {
  return <header>...</header>;
}
```

### ✅ **2. Props**
Passage de données du parent vers les enfants :
```jsx
<Article title="Introduction à React" author="Alice" content="..." />
```

### ✅ **3. JSX**
Syntaxe HTML dans JavaScript avec interpolation de variables :
```jsx
<h2>{title}</h2>
<p>Par {author}</p>
```

### ✅ **4. Listes avec .map()**
Affichage dynamique d'une liste d'articles avec la méthode `.map()` :
```jsx
{articles.map((article) => (
  <Article key={article.id} {...article} />
))}
```

### ✅ **5. La Prop `key`**
**Rôle de la prop `key` :**  
La prop `key` est essentielle lorsqu'on affiche des listes en React. Elle permet à React d'identifier de manière unique chaque élément de la liste. Cela optimise les performances en permettant à React de savoir exactement quel élément a changé, a été ajouté ou supprimé, sans avoir à re-créer tous les éléments de la liste à chaque mise à jour.

**Pourquoi c'est important :**
- Améliore les performances de rendu
- Évite les bugs lors des mises à jour de liste
- Permet à React de conserver l'état des composants correctement

---

## 🛠️ Installation et Lancement

### **Prérequis**
- Node.js (version 16 ou supérieure)
- npm ou yarn

### **Étapes d'installation**

1. **Créer le projet avec Vite**
```bash
npm create vite@latest mon-blog-react -- --template react
```

2. **Se déplacer dans le dossier**
```bash
cd mon-blog-react
```

3. **Installer les dépendances**
```bash
npm install
```

4. **Lancer le serveur de développement**
```bash
npm run dev
```

5. **Ouvrir dans le navigateur**
```
http://localhost:5173
```

---

## 📸 Aperçu de l'Application

L'application affiche :
- ✅ Un en-tête bleu avec le titre "Mon Blog React"
- ✅ Un compteur d'articles disponibles
- ✅ 4 cartes d'articles avec fond violet clair
- ✅ Un pied de page avec copyright et mentions

---

## 📝 Travail Réalisé

### **Étape 1** : Création du projet avec Vite ✅
- Initialisation du projet React avec template Vite

### **Étape 2** : Nettoyage de la structure ✅
- Suppression du contenu par défaut de `App.jsx`
- Création du dossier `src/components/`

### **Étape 3** : Création des composants ✅
- Composant `Header.jsx` avec titre et sous-titre
- Composant `Article.jsx` avec props dynamiques
- Composant `Footer.jsx` avec année dynamique

### **Étape 4** : Intégration dans App.jsx ✅
- Import des composants
- Création d'un tableau d'articles
- Affichage dynamique avec `.map()`
- Utilisation de la prop `key`

### **Étape 5** : Styles inline ✅
- Design responsive avec maxWidth
- Flexbox pour la mise en page
- Couleurs personnalisées (bleu, violet, gris)

---

## 🎓 Compétences Acquises

- ✅ Création d'un projet React avec Vite
- ✅ Création de composants fonctionnels
- ✅ Utilisation des props pour passer des données
- ✅ Écriture de JSX
- ✅ Affichage de listes dynamiques avec `.map()`
- ✅ Compréhension du rôle de la prop `key`
- ✅ Structuration d'une application React
- ✅ Utilisation de styles inline en JSX

---

## 🚀 Prochaines Étapes

Dans les prochaines séances, nous apprendrons à :
- Utiliser le **State** avec `useState` pour rendre l'application interactive
- Gérer les **événements** (clics, soumission de formulaires)
- Ajouter des **fonctionnalités dynamiques** (like, commentaires)
- Utiliser le **CSS Modules** pour une meilleure organisation des styles

---

## 👨‍💻 Auteur

**Étudiant(e)** - École Polytechnique de Sousse  
**Formation** : MERN Stack - Semaine 6  
**Date** : Novembre 2025

---

## 📄 Licence

Ce projet est réalisé dans un cadre éducatif.  
© 2025 École Polytechnique Sousse - Tous droits réservés

---

## 🌟 Points Forts du Projet

- ✅ Code propre et bien structuré
- ✅ Composants réutilisables
- ✅ Respect des bonnes pratiques React
- ✅ Design simple et élégant
- ✅ Application fonctionnelle et responsive

---

**🎉 Félicitations ! Vous avez créé votre première application React complète !**
