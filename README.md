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
HTML est un **langage de balisage** qui définit la structure et le contenu d'une page web. Il est composé d'éléments comme : Sigma (Section(sous-section(div(element))))...
- **Texte, images, liens, vidéos, tableaux…**  
   - `<p>` : Paragraphe de texte  
      ```html
      <p>Ceci est un paragraphe</p>
      ```
   - `<img>` : Image  
      ```html
      <img src="image.jpg" alt="Description">
      ```
   - `<a>` : Lien hypertexte  
      ```html
      <a href="https://www.example.com">Visiter le site</a>
      ```
   - `<video>` : Vidéo  
      ```html
      <video src="video.mp4" controls></video>
      ```
   - `<table>` : Tableau  
      ```html
      <table>
        <tr><td>Cellule 1</td></tr>
      </table>
      ```  
- **Balises de structure** :  
  - `<div>` : Division qui regroupe plusieurs éléments.  
  - `<section>` : Regroupe une partie du contenu d’une page.   

### 🔹 NB :  
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
1. **Position absolue**
   ```css
   position: absolute;
   top: 10px; right: 10px; bottom: 10px; left: 10px;
   ```  
2. **Flexbox**
   ```css
   /* Positionnée un élément a l’intérieur d’une div */
   display: flex;
   align-items: center;  /* Centrage vertical / div */
   align-content: center; /* Centrage Horizontal / div */
   justify-content: space-between;  /* Espacement  */
   ```  
3. **Grid**
   ```css
   display: grid;
   grid-template-columns: repeat(4, 1fr);
   grid-column: 4 / 4; /*position de lelement*/
   /*Vous pouvez faire grid-template-row ou grid-row  */
   /*grid-column: 2 / span 2; prendre 2 colonnes à partir de la colonne 2 */
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
margin: 10px; espacement hors conteneur
padding: 10px; espacement dans conteneur
```  

#### 🎨 **2.8 Arrière-plan et espacement**  
```css
margin-bottom: 10px;
margin-top: 10px;
background-color: lightgray;
```  

---
