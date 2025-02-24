# 🌐 Développement Web – HTML / CSS  

## 📌 **Introduction**  

Ce document présente les bases du développement d'une **application web** *frontend ou la vue (View)*

### 🏗️ **Architecture d'une application web**  
✅ **Frontend** : Interface utilisateur développée avec **HTML, CSS et JavaScript**.  
✅ **Backend** : Gestion des données et de la logique métier avec **PHP, Java, Python**, etc.  
✅ **Modèle MVC** :  
- **Modèle (Model)** : Gestion des données (CRUD : Create, Read, Update, Delete).  
- **Vue (View)** : Interface utilisateur (HTML + CSS + JS).  
- **Contrôleur (Controller)** : Logique d’application (traitement des requêtes et gestion des actions).  


## 🖥️ **HTML : HyperText Markup Language**  

### 🔹 Définition  
HTML est un **langage de balisage** qui définit la structure et le contenu d'une page web. Il est composé d'éléments comme :  
- **Texte, images, liens, vidéos, tableaux…**  
- **Balises de structure** :  
  - `<div>` : Division qui regroupe plusieurs éléments.  
  - `<section>` : Regroupe une partie du contenu d’une page.  
  - `<article>` : Contenu autonome (blog, news…).  

### 🔹 Balises principales  
✅ **Balises en bloc** : `<div>`, `<p>`, `<section>` (prennent toute la largeur).  
✅ **Balises en ligne** : `<span>`, `<a>`, `<strong>` (ne prennent que la largeur de leur contenu).  

---

## 🎨 **CSS : Cascading Style Sheets**  

### 🎨 **1. Comment appliquer le style ?**  
1. **Sélection de tous les éléments**  
   ```css
   * { margin: 0; padding: 0; }
   ```  
2. **Cibler une balise spécifique**  
   ```css
   body { background-color: #f5f5f5; }
   ```  
3. **Cibler une classe**  
   ```css
   .header { font-size: 20px; color: blue; }
   ```  

---

### 🎯 **2. Styles de base**  

#### 📌 **2.1 Positions**  
1. **Méthode 1** : Position absolue  
   ```css
   position: absolute;
   top: 10px; right: 10px; bottom: 10px; left: 10px;
   ```  
2. **Méthode 2** : Flexbox  
   ```css
   display: flex;
   align-items: center;  /* Centrage vertical */
   justify-content: space-between;  /* Espacement */
   ```  
3. **Méthode 3** : Grid  
   ```css
   display: grid;
   grid-template-columns: repeat(4, 1fr);
   grid-column: 4 / 4;
   ```  

#### 🎨 **2.2 Couleurs**  
- `color: red;` → Couleur du texte  
- `background-color: blue;` → Couleur d’arrière-plan  
- `border-color: black;` → Couleur des bordures  

#### 📏 **2.3 Tailles (largeur & hauteur)**  
```css
width: 100%;  /* Largeur auto-adaptative */
height: auto;  /* Hauteur automatique */
```  

#### 🔠 **2.4 Style du texte**  
```css
text-align: center;
color: black;
font-size: 20px;
font-weight: bold;
font-family: Verdana, Geneva, Tahoma, sans-serif;
```  

#### 📸 **2.5 Styles d’images**  
```css
img {
   width: 100px;
   height: auto;
   border-radius: 10px;
}
```  

#### 🔗 **2.6 Styles des liens**  
```css
a {
   text-decoration: none;
   color: blue;
}
a:hover {
   color: red;
}
```  

#### 📏 **2.7 Espacement entre les balises**  
```css
margin: 10px;
padding: 10px;
```  

#### 🎨 **2.8 Arrière-plan et espacement**  
```css
margin-bottom: 10px;
margin-top: 10px;
background-color: lightgray;
```  

---

## 🚀 **Point de départ pour les développeurs**  

1️⃣ **Créer une structure HTML de base**  
   ```html
   <!DOCTYPE html>
   <html lang="fr">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Mon Projet Web</title>
       <link rel="stylesheet" href="style.css">
   </head>
   <body>
       <header class="header">Bienvenue sur mon site</header>
       <section>
           <p>Contenu principal ici.</p>
       </section>
   </body>
   </html>
   ```  

2️⃣ **Créer un fichier `style.css`**  
   ```css
   body {
       font-family: Arial, sans-serif;
       background-color: #f0f0f0;
   }
   .header {
       background-color: blue;
       color: white;
       text-align: center;
       padding: 10px;
   }
   ```  

3️⃣ **Ajout d’un script JavaScript (`script.js`)**  
   ```js
   document.addEventListener("DOMContentLoaded", function() {
       console.log("Le site est chargé !");
   });
   ```  

