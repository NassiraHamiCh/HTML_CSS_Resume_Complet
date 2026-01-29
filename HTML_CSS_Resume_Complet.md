# 🌐 HTML & CSS - Résumé Détaillé Complet

## 📚 Table des matières

### HTML
1. [Structure de base HTML](#1-structure-de-base-html)
2. [Balises de texte](#2-balises-de-texte)
3. [Listes](#3-listes)
4. [Liens et navigation](#4-liens-et-navigation)
5. [Images et médias](#5-images-et-médias)
6. [Tableaux](#6-tableaux)
7. [Formulaires](#7-formulaires)
8. [Balises sémantiques](#8-balises-sémantiques)
9. [Attributs globaux](#9-attributs-globaux)
10. [HTML5 avancé](#10-html5-avancé)

### CSS
11. [Intégration CSS](#11-intégration-css)
12. [Sélecteurs](#12-sélecteurs)
13. [Propriétés de texte](#13-propriétés-de-texte)
14. [Couleurs et arrière-plans](#14-couleurs-et-arrière-plans)
15. [Box Model](#15-box-model)
16. [Positionnement](#16-positionnement)
17. [Flexbox](#17-flexbox)
18. [Grid](#18-grid)
19. [Responsive Design](#19-responsive-design)
20. [Transitions et Animations](#20-transitions-et-animations)
21. [Pseudo-classes et Pseudo-éléments](#21-pseudo-classes-et-pseudo-éléments)
22. [Variables CSS](#22-variables-css)
23. [Techniques avancées](#23-techniques-avancées)

---

# HTML

## 1. Structure de base HTML

### 1.1 Document HTML minimal
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ma Page Web</title>
</head>
<body>
    <h1>Bienvenue</h1>
    <p>Ceci est ma première page.</p>
</body>
</html>
```

### 1.2 Balises de métadonnées
```html
<head>
    <!-- Encodage des caractères -->
    <meta charset="UTF-8">
    
    <!-- Responsive design -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- Description pour SEO -->
    <meta name="description" content="Description de ma page">
    
    <!-- Mots-clés -->
    <meta name="keywords" content="html, css, web">
    
    <!-- Auteur -->
    <meta name="author" content="Votre Nom">
    
    <!-- Titre de la page -->
    <title>Titre de la page</title>
    
    <!-- Favicon -->
    <link rel="icon" href="favicon.ico">
    
    <!-- CSS externe -->
    <link rel="stylesheet" href="style.css">
    
    <!-- JavaScript externe -->
    <script src="script.js" defer></script>
</head>
```

### 1.3 Commentaires
```html
<!-- Ceci est un commentaire HTML -->

<!--
    Commentaire
    sur plusieurs
    lignes
-->
```

---

## 2. Balises de texte

### 2.1 Titres
```html
<h1>Titre niveau 1 (le plus important)</h1>
<h2>Titre niveau 2</h2>
<h3>Titre niveau 3</h3>
<h4>Titre niveau 4</h4>
<h5>Titre niveau 5</h5>
<h6>Titre niveau 6 (le moins important)</h6>
```

### 2.2 Paragraphes et texte
```html
<!-- Paragraphe -->
<p>Ceci est un paragraphe de texte.</p>

<!-- Saut de ligne -->
<p>Première ligne<br>Deuxième ligne</p>

<!-- Ligne horizontale -->
<hr>

<!-- Texte préformaté -->
<pre>
    Texte     avec espaces
    et     retours à la ligne
    préservés
</pre>

<!-- Citation bloc -->
<blockquote cite="https://source.com">
    Ceci est une citation longue.
</blockquote>

<!-- Citation courte -->
<p>Il a dit : <q>Bonjour</q></p>

<!-- Code -->
<code>let x = 10;</code>

<!-- Bloc de code -->
<pre><code>
function hello() {
    console.log("Hello");
}
</code></pre>
```

### 2.3 Formatage du texte
```html
<!-- Gras (important) -->
<strong>Texte important</strong>
<b>Texte en gras (visuel)</b>

<!-- Italique (emphase) -->
<em>Texte avec emphase</em>
<i>Texte en italique (visuel)</i>

<!-- Souligné -->
<u>Texte souligné</u>

<!-- Barré -->
<s>Texte barré</s>
<del>Texte supprimé</del>

<!-- Petit -->
<small>Petit texte</small>

<!-- Marqué/surligné -->
<mark>Texte surligné</mark>

<!-- Exposant et indice -->
<p>E = mc<sup>2</sup></p>
<p>H<sub>2</sub>O</p>

<!-- Abréviation -->
<abbr title="HyperText Markup Language">HTML</abbr>

<!-- Citation d'œuvre -->
<cite>Le Petit Prince</cite>

<!-- Définition -->
<dfn>HTTP</dfn> signifie HyperText Transfer Protocol

<!-- Texte inséré -->
<ins>Texte ajouté</ins>

<!-- Variable -->
<var>x</var> + <var>y</var> = 10

<!-- Résultat de calcul -->
<samp>Erreur 404 : Page non trouvée</samp>

<!-- Entrée clavier -->
<kbd>Ctrl</kbd> + <kbd>C</kbd>
```

---

## 3. Listes

### 3.1 Liste non ordonnée
```html
<ul>
    <li>Élément 1</li>
    <li>Élément 2</li>
    <li>Élément 3</li>
</ul>

<!-- Styles de puces -->
<ul style="list-style-type: circle;">
    <li>Cercle</li>
</ul>

<ul style="list-style-type: square;">
    <li>Carré</li>
</ul>

<ul style="list-style-type: none;">
    <li>Sans puce</li>
</ul>
```

### 3.2 Liste ordonnée
```html
<ol>
    <li>Premier</li>
    <li>Deuxième</li>
    <li>Troisième</li>
</ol>

<!-- Commencer à un numéro spécifique -->
<ol start="5">
    <li>Cinquième</li>
    <li>Sixième</li>
</ol>

<!-- Types de numérotation -->
<ol type="A">  <!-- A, B, C -->
    <li>Alpha</li>
</ol>

<ol type="a">  <!-- a, b, c -->
    <li>Alpha minuscule</li>
</ol>

<ol type="I">  <!-- I, II, III -->
    <li>Romain majuscule</li>
</ol>

<ol type="i">  <!-- i, ii, iii -->
    <li>Romain minuscule</li>
</ol>

<!-- Ordre inversé -->
<ol reversed>
    <li>Trois</li>
    <li>Deux</li>
    <li>Un</li>
</ol>
```

### 3.3 Liste de définitions
```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
    
    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
    
    <dt>JavaScript</dt>
    <dd>Langage de programmation web</dd>
</dl>
```

### 3.4 Listes imbriquées
```html
<ul>
    <li>Fruits
        <ul>
            <li>Pomme</li>
            <li>Banane</li>
        </ul>
    </li>
    <li>Légumes
        <ul>
            <li>Carotte</li>
            <li>Tomate</li>
        </ul>
    </li>
</ul>
```

---

## 4. Liens et navigation

### 4.1 Liens de base
```html
<!-- Lien externe -->
<a href="https://www.google.com">Google</a>

<!-- Lien dans un nouvel onglet -->
<a href="https://www.google.com" target="_blank">Google (nouvel onglet)</a>

<!-- Lien relatif -->
<a href="page2.html">Page 2</a>
<a href="../index.html">Retour à l'accueil</a>

<!-- Lien email -->
<a href="mailto:contact@example.com">Envoyer un email</a>

<!-- Lien téléphone -->
<a href="tel:+33123456789">Appeler</a>

<!-- Lien de téléchargement -->
<a href="document.pdf" download>Télécharger PDF</a>

<!-- Lien avec titre (tooltip) -->
<a href="page.html" title="Aller à la page">Lien</a>
```

### 4.2 Ancres (liens internes)
```html
<!-- Créer une ancre -->
<h2 id="section1">Section 1</h2>

<!-- Lien vers l'ancre -->
<a href="#section1">Aller à la section 1</a>

<!-- Lien vers une ancre sur une autre page -->
<a href="page2.html#section3">Section 3 de page 2</a>

<!-- Retour en haut de page -->
<a href="#">Retour en haut</a>
```

### 4.3 Attributs de liens
```html
<!-- target -->
<a href="url" target="_blank">  <!-- Nouvel onglet -->
<a href="url" target="_self">   <!-- Même fenêtre (défaut) -->
<a href="url" target="_parent"> <!-- Frame parent -->
<a href="url" target="_top">    <!-- Fenêtre complète -->

<!-- rel (relation) -->
<a href="url" rel="nofollow">      <!-- Ne pas suivre pour SEO -->
<a href="url" rel="noopener">      <!-- Sécurité nouvel onglet -->
<a href="url" rel="noreferrer">    <!-- Ne pas envoyer referrer -->
<a href="url" rel="external">      <!-- Lien externe -->
```

---

## 5. Images et médias

### 5.1 Images
```html
<!-- Image de base -->
<img src="image.jpg" alt="Description de l'image">

<!-- Image avec dimensions -->
<img src="image.jpg" alt="Description" width="300" height="200">

<!-- Image responsive (s'adapte au conteneur) -->
<img src="image.jpg" alt="Description" style="max-width: 100%; height: auto;">

<!-- Image avec titre (tooltip) -->
<img src="image.jpg" alt="Description" title="Titre de l'image">

<!-- Image cliquable -->
<a href="page.html">
    <img src="image.jpg" alt="Description">
</a>
```

### 5.2 Images responsive avancées
```html
<!-- srcset : différentes résolutions -->
<img src="image-400.jpg"
     srcset="image-400.jpg 400w,
             image-800.jpg 800w,
             image-1200.jpg 1200w"
     sizes="(max-width: 600px) 400px,
            (max-width: 900px) 800px,
            1200px"
     alt="Description">

<!-- Picture : différents formats -->
<picture>
    <source media="(min-width: 800px)" srcset="large.jpg">
    <source media="(min-width: 400px)" srcset="medium.jpg">
    <img src="small.jpg" alt="Description">
</picture>

<!-- WebP avec fallback -->
<picture>
    <source srcset="image.webp" type="image/webp">
    <source srcset="image.jpg" type="image/jpeg">
    <img src="image.jpg" alt="Description">
</picture>
```

### 5.3 Figure et légende
```html
<figure>
    <img src="image.jpg" alt="Description">
    <figcaption>Légende de l'image</figcaption>
</figure>
```

### 5.4 Audio
```html
<!-- Lecteur audio -->
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    <source src="audio.ogg" type="audio/ogg">
    Votre navigateur ne supporte pas l'audio.
</audio>

<!-- Attributs audio -->
<audio controls autoplay loop muted>
    <source src="audio.mp3" type="audio/mpeg">
</audio>
```

### 5.5 Vidéo
```html
<!-- Lecteur vidéo -->
<video controls width="640" height="360">
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    Votre navigateur ne supporte pas la vidéo.
</video>

<!-- Attributs vidéo -->
<video controls autoplay loop muted poster="thumbnail.jpg">
    <source src="video.mp4" type="video/mp4">
    <track src="subtitles_fr.vtt" kind="subtitles" srclang="fr" label="Français">
</video>
```

### 5.6 Iframe
```html
<!-- Intégrer une page externe -->
<iframe src="https://www.example.com" width="600" height="400"></iframe>

<!-- YouTube -->
<iframe width="560" height="315" 
        src="https://www.youtube.com/embed/VIDEO_ID" 
        frameborder="0" 
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
</iframe>

<!-- Google Maps -->
<iframe src="https://www.google.com/maps/embed?pb=..." 
        width="600" 
        height="450" 
        style="border:0;" 
        allowfullscreen="">
</iframe>
```

---

## 6. Tableaux

### 6.1 Tableau simple
```html
<table>
    <tr>
        <th>Nom</th>
        <th>Âge</th>
        <th>Ville</th>
    </tr>
    <tr>
        <td>Alice</td>
        <td>25</td>
        <td>Paris</td>
    </tr>
    <tr>
        <td>Bob</td>
        <td>30</td>
        <td>Lyon</td>
    </tr>
</table>
```

### 6.2 Tableau avec structure complète
```html
<table>
    <caption>Liste des étudiants</caption>
    <thead>
        <tr>
            <th>Nom</th>
            <th>Prénom</th>
            <th>Note</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dupont</td>
            <td>Jean</td>
            <td>15</td>
        </tr>
        <tr>
            <td>Martin</td>
            <td>Marie</td>
            <td>17</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="2">Moyenne</td>
            <td>16</td>
        </tr>
    </tfoot>
</table>
```

### 6.3 Fusion de cellules
```html
<table>
    <tr>
        <!-- Fusion horizontale -->
        <td colspan="2">Cellule fusionnée sur 2 colonnes</td>
        <td>Cellule 3</td>
    </tr>
    <tr>
        <td>Cellule 1</td>
        <!-- Fusion verticale -->
        <td rowspan="2">Cellule fusionnée sur 2 lignes</td>
        <td>Cellule 3</td>
    </tr>
    <tr>
        <td>Cellule 1</td>
        <td>Cellule 3</td>
    </tr>
</table>
```

### 6.4 Groupement de colonnes
```html
<table>
    <colgroup>
        <col style="background-color: #f0f0f0;">
        <col span="2" style="background-color: #e0e0e0;">
    </colgroup>
    <tr>
        <th>Colonne 1</th>
        <th>Colonne 2</th>
        <th>Colonne 3</th>
    </tr>
    <tr>
        <td>Donnée 1</td>
        <td>Donnée 2</td>
        <td>Donnée 3</td>
    </tr>
</table>
```

---

## 7. Formulaires

### 7.1 Structure de formulaire
```html
<form action="/submit" method="POST">
    <!-- Champs du formulaire -->
    <button type="submit">Envoyer</button>
</form>

<!-- Attributs de form -->
<form action="/submit"           <!-- URL de soumission -->
      method="POST"              <!-- GET ou POST -->
      enctype="multipart/form-data"  <!-- Pour upload fichiers -->
      autocomplete="on"          <!-- Autocomplétion -->
      novalidate>                <!-- Désactiver validation HTML5 -->
</form>
```

### 7.2 Champs de texte
```html
<!-- Texte simple -->
<label for="nom">Nom :</label>
<input type="text" id="nom" name="nom" placeholder="Votre nom">

<!-- Email -->
<label for="email">Email :</label>
<input type="email" id="email" name="email" required>

<!-- Mot de passe -->
<label for="mdp">Mot de passe :</label>
<input type="password" id="mdp" name="mdp">

<!-- Numéro -->
<label for="age">Âge :</label>
<input type="number" id="age" name="age" min="0" max="120" step="1">

<!-- Téléphone -->
<label for="tel">Téléphone :</label>
<input type="tel" id="tel" name="tel" pattern="[0-9]{10}">

<!-- URL -->
<label for="site">Site web :</label>
<input type="url" id="site" name="site">

<!-- Recherche -->
<input type="search" name="q" placeholder="Rechercher...">

<!-- Zone de texte multiligne -->
<label for="message">Message :</label>
<textarea id="message" name="message" rows="5" cols="40"></textarea>
```

### 7.3 Champs de sélection
```html
<!-- Cases à cocher -->
<input type="checkbox" id="option1" name="option1" value="yes">
<label for="option1">Option 1</label>

<input type="checkbox" id="option2" name="option2" value="yes" checked>
<label for="option2">Option 2 (cochée par défaut)</label>

<!-- Boutons radio -->
<input type="radio" id="choix1" name="choix" value="1">
<label for="choix1">Choix 1</label>

<input type="radio" id="choix2" name="choix" value="2" checked>
<label for="choix2">Choix 2</label>

<!-- Liste déroulante -->
<label for="pays">Pays :</label>
<select id="pays" name="pays">
    <option value="">-- Sélectionner --</option>
    <option value="fr">France</option>
    <option value="be">Belgique</option>
    <option value="ch" selected>Suisse</option>
</select>

<!-- Liste déroulante avec groupes -->
<select name="continent">
    <optgroup label="Europe">
        <option value="fr">France</option>
        <option value="de">Allemagne</option>
    </optgroup>
    <optgroup label="Asie">
        <option value="jp">Japon</option>
        <option value="cn">Chine</option>
    </optgroup>
</select>

<!-- Sélection multiple -->
<select name="langues" multiple size="4">
    <option value="fr">Français</option>
    <option value="en">Anglais</option>
    <option value="es">Espagnol</option>
    <option value="de">Allemand</option>
</select>
```

### 7.4 Champs spéciaux
```html
<!-- Date -->
<input type="date" name="date" min="2024-01-01" max="2024-12-31">

<!-- Heure -->
<input type="time" name="heure">

<!-- Date et heure -->
<input type="datetime-local" name="datetime">

<!-- Mois -->
<input type="month" name="mois">

<!-- Semaine -->
<input type="week" name="semaine">

<!-- Couleur -->
<input type="color" name="couleur" value="#ff0000">

<!-- Curseur (range) -->
<input type="range" name="volume" min="0" max="100" value="50" step="10">

<!-- Fichier -->
<input type="file" name="fichier">

<!-- Fichiers multiples -->
<input type="file" name="fichiers" multiple>

<!-- Types de fichiers acceptés -->
<input type="file" name="image" accept="image/*">
<input type="file" name="pdf" accept=".pdf">

<!-- Champ caché -->
<input type="hidden" name="user_id" value="12345">
```

### 7.5 Boutons
```html
<!-- Bouton de soumission -->
<button type="submit">Envoyer</button>
<input type="submit" value="Envoyer">

<!-- Bouton de réinitialisation -->
<button type="reset">Réinitialiser</button>
<input type="reset" value="Réinitialiser">

<!-- Bouton générique -->
<button type="button" onclick="alert('Cliqué')">Cliquer</button>
<input type="button" value="Cliquer" onclick="alert('Cliqué')">

<!-- Bouton image -->
<input type="image" src="submit.png" alt="Envoyer">
```

### 7.6 Groupement de champs
```html
<form>
    <fieldset>
        <legend>Informations personnelles</legend>
        
        <label for="nom">Nom :</label>
        <input type="text" id="nom" name="nom">
        
        <label for="prenom">Prénom :</label>
        <input type="text" id="prenom" name="prenom">
    </fieldset>
    
    <fieldset>
        <legend>Contact</legend>
        
        <label for="email">Email :</label>
        <input type="email" id="email" name="email">
    </fieldset>
</form>
```

### 7.7 Validation HTML5
```html
<!-- Champ requis -->
<input type="text" name="nom" required>

<!-- Longueur min/max -->
<input type="text" name="nom" minlength="3" maxlength="20">

<!-- Pattern (regex) -->
<input type="text" name="code" pattern="[A-Z]{3}[0-9]{3}">

<!-- Min/Max pour nombres -->
<input type="number" name="age" min="18" max="100">

<!-- Attributs de validation -->
<input type="email" name="email" required 
       pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$"
       title="Entrez une adresse email valide">
```

### 7.8 Autocomplete et datalist
```html
<!-- Datalist (suggestions) -->
<label for="navigateur">Navigateur :</label>
<input list="navigateurs" name="navigateur" id="navigateur">
<datalist id="navigateurs">
    <option value="Chrome">
    <option value="Firefox">
    <option value="Safari">
    <option value="Edge">
</datalist>

<!-- Autocomplete -->
<input type="text" name="nom" autocomplete="name">
<input type="email" name="email" autocomplete="email">
<input type="tel" name="tel" autocomplete="tel">
```

---

## 8. Balises sémantiques

### 8.1 Structure de page
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Page sémantique</title>
</head>
<body>
    <!-- En-tête de page -->
    <header>
        <h1>Mon Site</h1>
        <nav>
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#about">À propos</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Contenu principal -->
    <main>
        <!-- Article -->
        <article>
            <header>
                <h2>Titre de l'article</h2>
                <p>Publié le <time datetime="2024-01-29">29 janvier 2024</time></p>
            </header>
            
            <p>Contenu de l'article...</p>
            
            <footer>
                <p>Auteur : Jean Dupont</p>
            </footer>
        </article>
        
        <!-- Section -->
        <section>
            <h2>Section de contenu</h2>
            <p>Contenu de la section...</p>
        </section>
    </main>
    
    <!-- Barre latérale -->
    <aside>
        <h3>Informations complémentaires</h3>
        <p>Contenu de la sidebar...</p>
    </aside>
    
    <!-- Pied de page -->
    <footer>
        <p>&copy; 2024 Mon Site. Tous droits réservés.</p>
    </footer>
</body>
</html>
```

### 8.2 Balises sémantiques de contenu
```html
<!-- Article -->
<article>
    <h2>Titre de l'article</h2>
    <p>Contenu indépendant et autonome</p>
</article>

<!-- Section -->
<section>
    <h2>Section thématique</h2>
    <p>Regroupement thématique de contenu</p>
</section>

<!-- Navigation -->
<nav>
    <ul>
        <li><a href="#">Lien 1</a></li>
        <li><a href="#">Lien 2</a></li>
    </ul>
</nav>

<!-- Aside (contenu complémentaire) -->
<aside>
    <h3>En savoir plus</h3>
    <p>Informations complémentaires...</p>
</aside>

<!-- En-tête -->
<header>
    <h1>Titre principal</h1>
    <p>Sous-titre ou description</p>
</header>

<!-- Pied de page -->
<footer>
    <p>Copyright 2024</p>
    <address>contact@example.com</address>
</footer>

<!-- Détails avec résumé -->
<details>
    <summary>Cliquez pour plus de détails</summary>
    <p>Contenu caché par défaut</p>
</details>

<!-- Boîte de dialogue -->
<dialog open>
    <p>Ceci est une boîte de dialogue</p>
    <button>Fermer</button>
</dialog>
```

### 8.3 Autres balises sémantiques
```html
<!-- Date/Heure -->
<time datetime="2024-01-29T14:30">29 janvier 2024 à 14h30</time>

<!-- Adresse -->
<address>
    123 Rue de la Paix<br>
    75001 Paris<br>
    <a href="mailto:contact@example.com">contact@example.com</a>
</address>

<!-- Progression -->
<progress value="70" max="100">70%</progress>

<!-- Mesure/Jauge -->
<meter value="0.6" min="0" max="1">60%</meter>
<meter value="75" min="0" max="100" low="30" high="80" optimum="90">75%</meter>
```

---

## 9. Attributs globaux

### 9.1 Attributs d'identification
```html
<!-- ID unique -->
<div id="header">En-tête</div>

<!-- Classes (multiples possibles) -->
<p class="important highlight">Texte important</p>

<!-- Titre (tooltip) -->
<span title="Information supplémentaire">Survolez-moi</span>
```

### 9.2 Attributs de style et comportement
```html
<!-- Style inline -->
<p style="color: red; font-size: 18px;">Texte rouge</p>

<!-- Langue -->
<p lang="en">This is English</p>
<p lang="fr">Ceci est en français</p>

<!-- Direction du texte -->
<p dir="rtl">نص عربي من اليمين إلى اليسار</p>

<!-- Contenu éditable -->
<div contenteditable="true">Vous pouvez éditer ce texte</div>

<!-- Glisser-déposer -->
<div draggable="true">Élément déplaçable</div>

<!-- Caché -->
<div hidden>Contenu caché</div>

<!-- Tabindex (ordre de tabulation) -->
<input type="text" tabindex="1">
<input type="text" tabindex="2">

<!-- Accesskey (raccourci clavier) -->
<button accesskey="s">Enregistrer (Alt+S)</button>
```

### 9.3 Attributs data
```html
<!-- Données personnalisées -->
<div data-user-id="12345" data-role="admin">Utilisateur</div>

<!-- Accès en JavaScript -->
<script>
    let elem = document.querySelector('[data-user-id]');
    console.log(elem.dataset.userId);  // "12345"
    console.log(elem.dataset.role);    // "admin"
</script>
```

---

## 10. HTML5 avancé

### 10.1 Canvas
```html
<canvas id="myCanvas" width="400" height="200">
    Votre navigateur ne supporte pas canvas
</canvas>

<script>
    let canvas = document.getElementById('myCanvas');
    let ctx = canvas.getContext('2d');
    ctx.fillStyle = 'red';
    ctx.fillRect(10, 10, 100, 50);
</script>
```

### 10.2 SVG inline
```html
<svg width="100" height="100">
    <circle cx="50" cy="50" r="40" fill="blue" />
    <rect x="10" y="10" width="30" height="30" fill="red" />
</svg>
```

### 10.3 Template
```html
<template id="mon-template">
    <div class="card">
        <h3></h3>
        <p></p>
    </div>
</template>

<script>
    let template = document.getElementById('mon-template');
    let clone = template.content.cloneNode(true);
    // Modifier et insérer le clone
</script>
```

---

# CSS

## 11. Intégration CSS

### 11.1 CSS inline (dans la balise)
```html
<p style="color: red; font-size: 18px;">Texte rouge</p>
```

### 11.2 CSS interne (dans <head>)
```html
<head>
    <style>
        p {
            color: blue;
            font-size: 16px;
        }
    </style>
</head>
```

### 11.3 CSS externe (fichier séparé) - **RECOMMANDÉ**
```html
<head>
    <link rel="stylesheet" href="style.css">
</head>
```

```css
/* style.css */
p {
    color: green;
    font-size: 14px;
}
```

### 11.4 Import CSS
```css
/* Dans un fichier CSS */
@import url('autre-style.css');
@import url('https://fonts.googleapis.com/css2?family=Roboto');
```

---

## 12. Sélecteurs

### 12.1 Sélecteurs de base
```css
/* Sélecteur universel */
* {
    margin: 0;
    padding: 0;
}

/* Sélecteur de type (balise) */
p {
    color: black;
}

h1 {
    font-size: 32px;
}

/* Sélecteur de classe */
.important {
    font-weight: bold;
}

.highlight {
    background-color: yellow;
}

/* Sélecteur d'ID */
#header {
    background-color: navy;
}

/* Sélecteur d'attribut */
[type="text"] {
    border: 1px solid gray;
}

[href^="https"] {  /* Commence par */
    color: green;
}

[href$=".pdf"] {  /* Se termine par */
    color: red;
}

[href*="google"] {  /* Contient */
    color: blue;
}

[title~="important"] {  /* Mot dans liste */
    font-weight: bold;
}

[lang|="en"] {  /* Langue */
    font-style: italic;
}
```

### 12.2 Combinateurs
```css
/* Descendant (espace) */
div p {
    color: red;  /* Tous les <p> dans un <div> */
}

/* Enfant direct (>) */
div > p {
    color: blue;  /* Seulement les <p> enfants directs */
}

/* Frère adjacent (+) */
h1 + p {
    font-size: 18px;  /* Le <p> immédiatement après <h1> */
}

/* Frères généraux (~) */
h1 ~ p {
    color: gray;  /* Tous les <p> après <h1> */
}
```

### 12.3 Sélecteurs multiples
```css
/* Virgule : plusieurs sélecteurs */
h1, h2, h3 {
    font-family: Arial, sans-serif;
}

/* Combinaison de classes */
.important.highlight {
    color: red;  /* Éléments avec LES DEUX classes */
}

/* Élément avec classe */
p.important {
    font-weight: bold;  /* <p> avec classe "important" */
}
```

---

## 13. Propriétés de texte

### 13.1 Police de caractères
```css
/* Famille de police */
p {
    font-family: Arial, Helvetica, sans-serif;
    font-family: 'Times New Roman', serif;
    font-family: 'Courier New', monospace;
}

/* Taille */
p {
    font-size: 16px;      /* Pixels */
    font-size: 1em;       /* Relatif au parent */
    font-size: 1rem;      /* Relatif à la racine */
    font-size: 100%;      /* Pourcentage */
    font-size: larger;    /* Mot-clé */
}

/* Poids (gras) */
p {
    font-weight: normal;   /* 400 */
    font-weight: bold;     /* 700 */
    font-weight: 100;      /* Très fin */
    font-weight: 900;      /* Très gras */
}

/* Style */
p {
    font-style: normal;
    font-style: italic;
    font-style: oblique;
}

/* Variante */
p {
    font-variant: normal;
    font-variant: small-caps;  /* PETITES MAJUSCULES */
}

/* Shorthand (raccourci) */
p {
    font: italic bold 16px/1.5 Arial, sans-serif;
    /*    style weight size/height family */
}
```

### 13.2 Formatage du texte
```css
/* Couleur */
p {
    color: red;
    color: #FF0000;
    color: rgb(255, 0, 0);
    color: rgba(255, 0, 0, 0.5);  /* Avec transparence */
    color: hsl(0, 100%, 50%);
}

/* Alignement */
p {
    text-align: left;
    text-align: right;
    text-align: center;
    text-align: justify;
}

/* Décoration */
p {
    text-decoration: none;
    text-decoration: underline;
    text-decoration: overline;
    text-decoration: line-through;
    text-decoration: underline wavy red;  /* Style ligne couleur */
}

/* Transformation */
p {
    text-transform: none;
    text-transform: uppercase;     /* MAJUSCULES */
    text-transform: lowercase;     /* minuscules */
    text-transform: capitalize;    /* Première Lettre Majuscule */
}

/* Indentation */
p {
    text-indent: 20px;     /* Première ligne */
    text-indent: -20px;    /* Négatif (retrait gauche) */
}

/* Espacement des lettres */
p {
    letter-spacing: 2px;
    letter-spacing: -1px;
}

/* Espacement des mots */
p {
    word-spacing: 5px;
}

/* Hauteur de ligne */
p {
    line-height: 1.5;      /* Relatif */
    line-height: 24px;     /* Absolu */
    line-height: 150%;     /* Pourcentage */
}

/* Ombre du texte */
p {
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    /*          h   v  blur color */
    text-shadow: 0 0 10px red, 0 0 20px blue;  /* Multiples */
}

/* Direction du texte */
p {
    direction: ltr;  /* Left to right */
    direction: rtl;  /* Right to left */
}

/* Espaces blancs */
p {
    white-space: normal;    /* Par défaut */
    white-space: nowrap;    /* Pas de retour à la ligne */
    white-space: pre;       /* Préserve espaces et retours */
    white-space: pre-wrap;  /* Préserve + retour auto */
}

/* Débordement de texte */
p {
    overflow: hidden;
    text-overflow: ellipsis;  /* ... */
    white-space: nowrap;
}

/* Césure */
p {
    word-wrap: break-word;     /* Coupe les mots longs */
    word-break: break-all;     /* Coupe n'importe où */
    hyphens: auto;             /* Césure automatique */
}
```

---

## 14. Couleurs et arrière-plans

### 14.1 Couleurs
```css
/* Formats de couleurs */
.element {
    color: red;                    /* Nom */
    color: #FF0000;                /* Hexadécimal */
    color: #F00;                   /* Hex court */
    color: rgb(255, 0, 0);         /* RGB */
    color: rgba(255, 0, 0, 0.5);   /* RGBA (transparence) */
    color: hsl(0, 100%, 50%);      /* HSL */
    color: hsla(0, 100%, 50%, 0.5); /* HSLA */
}

/* Couleurs courantes */
black, white, red, green, blue, yellow, orange, purple, pink, gray
```

### 14.2 Arrière-plans
```css
/* Couleur de fond */
div {
    background-color: lightblue;
    background-color: rgba(0, 0, 255, 0.3);
}

/* Image de fond */
div {
    background-image: url('image.jpg');
}

/* Répétition */
div {
    background-repeat: repeat;      /* Répète (défaut) */
    background-repeat: repeat-x;    /* Horizontalement */
    background-repeat: repeat-y;    /* Verticalement */
    background-repeat: no-repeat;   /* Pas de répétition */
}

/* Position */
div {
    background-position: center;
    background-position: top right;
    background-position: 50% 50%;
    background-position: 10px 20px;
}

/* Taille */
div {
    background-size: auto;          /* Taille originale */
    background-size: cover;         /* Couvre tout */
    background-size: contain;       /* Contenu visible */
    background-size: 100% 100%;     /* Étire */
    background-size: 300px 200px;   /* Dimensions fixes */
}

/* Attachement (scroll) */
div {
    background-attachment: scroll;  /* Défile (défaut) */
    background-attachment: fixed;   /* Fixe (parallax) */
}

/* Origine */
div {
    background-origin: padding-box;  /* Défaut */
    background-origin: border-box;
    background-origin: content-box;
}

/* Découpage */
div {
    background-clip: border-box;    /* Défaut */
    background-clip: padding-box;
    background-clip: content-box;
    background-clip: text;          /* Texte uniquement */
}

/* Shorthand (raccourci) */
div {
    background: url('img.jpg') no-repeat center/cover fixed;
    /*         image          repeat   pos   size  attach */
}

/* Multiples arrière-plans */
div {
    background: 
        url('img1.png') no-repeat top left,
        url('img2.png') no-repeat bottom right,
        linear-gradient(to bottom, #fff, #000);
}
```

### 14.3 Dégradés
```css
/* Dégradé linéaire */
div {
    background: linear-gradient(to right, red, blue);
    background: linear-gradient(45deg, red, yellow, green);
    background: linear-gradient(to bottom, 
                red 0%, yellow 50%, green 100%);
}

/* Dégradé radial */
div {
    background: radial-gradient(circle, red, blue);
    background: radial-gradient(ellipse at center, red, yellow, green);
    background: radial-gradient(circle at top left, red 20%, blue 80%);
}

/* Dégradé conique */
div {
    background: conic-gradient(red, yellow, green, blue, red);
    background: conic-gradient(from 90deg, red, yellow, green);
}
```

---

## 15. Box Model

### 15.1 Dimensions
```css
div {
    /* Largeur */
    width: 300px;
    width: 50%;
    width: auto;
    min-width: 200px;
    max-width: 500px;
    
    /* Hauteur */
    height: 200px;
    height: 100%;
    height: auto;
    min-height: 150px;
    max-height: 400px;
}

/* Box-sizing */
* {
    box-sizing: content-box;  /* Défaut (padding/border en +) */
    box-sizing: border-box;   /* Inclut padding/border (RECOMMANDÉ) */
}
```

### 15.2 Marges (margin)
```css
div {
    /* Toutes les marges */
    margin: 20px;
    
    /* Vertical | Horizontal */
    margin: 10px 20px;
    
    /* Top | Horizontal | Bottom */
    margin: 10px 20px 30px;
    
    /* Top | Right | Bottom | Left */
    margin: 10px 20px 30px 40px;
    
    /* Individuellement */
    margin-top: 10px;
    margin-right: 20px;
    margin-bottom: 30px;
    margin-left: 40px;
    
    /* Centrage horizontal */
    margin: 0 auto;
    
    /* Marges négatives */
    margin-top: -10px;
}
```

### 15.3 Espacement interne (padding)
```css
div {
    /* Même syntaxe que margin */
    padding: 20px;
    padding: 10px 20px;
    padding: 10px 20px 30px;
    padding: 10px 20px 30px 40px;
    
    padding-top: 10px;
    padding-right: 20px;
    padding-bottom: 30px;
    padding-left: 40px;
}
```

### 15.4 Bordures
```css
div {
    /* Bordure simple */
    border: 1px solid black;
    /*     width style color */
    
    /* Styles de bordure */
    border-style: solid;
    border-style: dotted;    /* Points */
    border-style: dashed;    /* Tirets */
    border-style: double;    /* Double ligne */
    border-style: groove;    /* 3D creux */
    border-style: ridge;     /* 3D relief */
    border-style: inset;     /* 3D enfoncé */
    border-style: outset;    /* 3D sorti */
    border-style: none;
    
    /* Largeur */
    border-width: 1px;
    border-width: thin;
    border-width: medium;
    border-width: thick;
    
    /* Couleur */
    border-color: red;
    
    /* Bordures individuelles */
    border-top: 2px solid red;
    border-right: 1px dashed blue;
    border-bottom: 3px dotted green;
    border-left: 1px solid black;
    
    /* Coins arrondis */
    border-radius: 10px;
    border-radius: 50%;          /* Cercle */
    border-radius: 10px 20px;    /* TL/BR | TR/BL */
    border-radius: 10px 20px 30px 40px;  /* TL TR BR BL */
    
    border-top-left-radius: 10px;
    border-top-right-radius: 20px;
    border-bottom-right-radius: 30px;
    border-bottom-left-radius: 40px;
}
```

### 15.5 Ombres
```css
div {
    /* Ombre de boîte */
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.3);
    /*         h   v   blur spread color */
    
    /* Ombre interne */
    box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.5);
    
    /* Multiples ombres */
    box-shadow: 
        5px 5px 10px rgba(0, 0, 0, 0.3),
        -5px -5px 10px rgba(255, 255, 255, 0.5);
}
```

### 15.6 Débordement
```css
div {
    overflow: visible;   /* Déborde (défaut) */
    overflow: hidden;    /* Caché */
    overflow: scroll;    /* Scrollbars toujours */
    overflow: auto;      /* Scrollbars si nécessaire */
    
    /* Séparément */
    overflow-x: hidden;
    overflow-y: scroll;
}
```

---

## 16. Positionnement

### 16.1 Display
```css
div {
    display: block;        /* Prend toute la largeur */
    display: inline;       /* Largeur du contenu, pas de dimensions */
    display: inline-block; /* Largeur contenu + dimensions possibles */
    display: none;         /* Invisible et ne prend pas de place */
    display: flex;         /* Flexbox */
    display: grid;         /* Grid */
    display: table;        /* Comme tableau */
}

/* Visibilité */
div {
    visibility: visible;
    visibility: hidden;    /* Invisible mais prend de la place */
}
```

### 16.2 Position
```css
div {
    position: static;      /* Normale (défaut) */
    position: relative;    /* Relatif à sa position normale */
    position: absolute;    /* Relatif au parent positionné */
    position: fixed;       /* Relatif à la fenêtre */
    position: sticky;      /* Hybride relative/fixed */
}

/* Décalages (avec position) */
div {
    top: 10px;
    right: 20px;
    bottom: 30px;
    left: 40px;
}

/* Exemples */
.relative {
    position: relative;
    top: 10px;      /* Décalé de 10px vers le bas */
    left: 20px;     /* Décalé de 20px vers la droite */
}

.absolute {
    position: absolute;
    top: 0;
    right: 0;       /* Coin supérieur droit du parent */
}

.fixed {
    position: fixed;
    bottom: 20px;
    right: 20px;    /* Toujours visible (ex: bouton scroll) */
}

.sticky {
    position: sticky;
    top: 0;         /* Colle en haut lors du scroll */
}
```

### 16.3 Z-index (superposition)
```css
div {
    z-index: 1;     /* Ordre de superposition */
    z-index: 999;   /* Plus haut = devant */
    z-index: -1;    /* Négatif = derrière */
}

/* Nécessite position autre que static */
.element {
    position: relative;
    z-index: 10;
}
```

### 16.4 Float et Clear
```css
/* Float (ancien système de mise en page) */
img {
    float: left;    /* Flotte à gauche */
    float: right;   /* Flotte à droite */
    float: none;    /* Pas de flottement */
}

/* Clear (annuler float) */
.footer {
    clear: left;    /* Annule float left */
    clear: right;   /* Annule float right */
    clear: both;    /* Annule tous les floats */
}

/* Clearfix (technique) */
.clearfix::after {
    content: "";
    display: table;
    clear: both;
}
```

---

## 17. Flexbox

### 17.1 Conteneur Flex
```css
.container {
    display: flex;
    
    /* Direction */
    flex-direction: row;            /* Horizontal → (défaut) */
    flex-direction: row-reverse;    /* Horizontal ← */
    flex-direction: column;         /* Vertical ↓ */
    flex-direction: column-reverse; /* Vertical ↑ */
    
    /* Retour à la ligne */
    flex-wrap: nowrap;   /* Une seule ligne (défaut) */
    flex-wrap: wrap;     /* Plusieurs lignes */
    flex-wrap: wrap-reverse;
    
    /* Shorthand direction + wrap */
    flex-flow: row wrap;
    
    /* Alignement horizontal (axe principal) */
    justify-content: flex-start;    /* Début (défaut) */
    justify-content: flex-end;      /* Fin */
    justify-content: center;        /* Centre */
    justify-content: space-between; /* Espace entre */
    justify-content: space-around;  /* Espace autour */
    justify-content: space-evenly;  /* Espace égal */
    
    /* Alignement vertical (axe secondaire) */
    align-items: stretch;      /* Étire (défaut) */
    align-items: flex-start;   /* Haut */
    align-items: flex-end;     /* Bas */
    align-items: center;       /* Centre */
    align-items: baseline;     /* Ligne de base */
    
    /* Alignement des lignes (wrap) */
    align-content: stretch;
    align-content: flex-start;
    align-content: flex-end;
    align-content: center;
    align-content: space-between;
    align-content: space-around;
    
    /* Espacement */
    gap: 20px;           /* Espacement entre items */
    row-gap: 10px;       /* Espacement vertical */
    column-gap: 20px;    /* Espacement horizontal */
}
```

### 17.2 Items Flex
```css
.item {
    /* Ordre */
    order: 0;      /* Par défaut */
    order: 1;      /* Plus tard */
    order: -1;     /* Plus tôt */
    
    /* Grossissement */
    flex-grow: 0;  /* Ne grandit pas (défaut) */
    flex-grow: 1;  /* Grandit également */
    flex-grow: 2;  /* Grandit 2x plus */
    
    /* Rétrécissement */
    flex-shrink: 1;  /* Rétrécit (défaut) */
    flex-shrink: 0;  /* Ne rétrécit pas */
    
    /* Taille de base */
    flex-basis: auto;   /* Automatique */
    flex-basis: 200px;  /* Largeur de base */
    flex-basis: 30%;    /* Pourcentage */
    
    /* Shorthand grow shrink basis */
    flex: 0 1 auto;     /* Défaut */
    flex: 1;            /* grow: 1, shrink: 1, basis: 0 */
    flex: 1 1 200px;
    
    /* Alignement individuel */
    align-self: auto;
    align-self: flex-start;
    align-self: flex-end;
    align-self: center;
    align-self: stretch;
}
```

### 17.3 Exemples Flexbox
```css
/* Centrage parfait */
.center {
    display: flex;
    justify-content: center;
    align-items: center;
}

/* Navigation horizontale */
.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

/* Grille responsive */
.grid {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

.grid-item {
    flex: 1 1 300px;  /* Min 300px, grandit/rétrécit */
}

/* Colonnes égales */
.columns {
    display: flex;
}

.column {
    flex: 1;  /* Toutes égales */
}
```

---

## 18. Grid

### 18.1 Conteneur Grid
```css
.container {
    display: grid;
    
    /* Colonnes */
    grid-template-columns: 200px 200px 200px;  /* 3 colonnes fixes */
    grid-template-columns: 1fr 1fr 1fr;        /* 3 colonnes égales */
    grid-template-columns: 1fr 2fr 1fr;        /* 2e colonne 2x plus large */
    grid-template-columns: repeat(3, 1fr);     /* Répétition */
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  /* Responsive */
    
    /* Lignes */
    grid-template-rows: 100px 200px 100px;
    grid-template-rows: repeat(3, 150px);
    grid-template-rows: auto 1fr auto;  /* Header | Content | Footer */
    
    /* Espacement */
    gap: 20px;               /* Vertical et horizontal */
    row-gap: 10px;           /* Vertical */
    column-gap: 20px;        /* Horizontal */
    grid-gap: 20px;          /* Ancienne syntaxe */
    
    /* Alignement horizontal */
    justify-items: start;    /* Début */
    justify-items: end;      /* Fin */
    justify-items: center;   /* Centre */
    justify-items: stretch;  /* Étire (défaut) */
    
    /* Alignement vertical */
    align-items: start;
    align-items: end;
    align-items: center;
    align-items: stretch;
    
    /* Alignement de la grille */
    justify-content: start;
    justify-content: end;
    justify-content: center;
    justify-content: space-between;
    justify-content: space-around;
    justify-content: space-evenly;
    
    align-content: start;
    align-content: end;
    align-content: center;
    align-content: space-between;
    align-content: space-around;
}
```

### 18.2 Items Grid
```css
.item {
    /* Position dans la grille */
    grid-column-start: 1;
    grid-column-end: 3;      /* Occupe colonnes 1 et 2 */
    
    /* Shorthand */
    grid-column: 1 / 3;      /* De 1 à 3 (non inclus) */
    grid-column: 1 / span 2; /* Commence à 1, s'étend sur 2 */
    grid-column: 1 / -1;     /* De 1 à la fin */
    
    /* Lignes */
    grid-row: 1 / 3;
    grid-row: 2 / span 2;
    
    /* Shorthand row / column */
    grid-area: 1 / 1 / 3 / 3;
    /*        row-start / col-start / row-end / col-end */
    
    /* Alignement individuel */
    justify-self: start;
    justify-self: end;
    justify-self: center;
    justify-self: stretch;
    
    align-self: start;
    align-self: end;
    align-self: center;
    align-self: stretch;
}
```

### 18.3 Grid avec zones nommées
```css
.container {
    display: grid;
    grid-template-columns: 200px 1fr 200px;
    grid-template-rows: auto 1fr auto;
    grid-template-areas:
        "header  header  header"
        "sidebar content aside"
        "footer  footer  footer";
    gap: 10px;
}

.header  { grid-area: header; }
.sidebar { grid-area: sidebar; }
.content { grid-area: content; }
.aside   { grid-area: aside; }
.footer  { grid-area: footer; }
```

### 18.4 Exemples Grid
```css
/* Grille simple 3 colonnes */
.grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

/* Grille responsive auto */
.grid-auto {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
}

/* Layout dashboard */
.dashboard {
    display: grid;
    grid-template-columns: 250px 1fr;
    grid-template-rows: 60px 1fr 40px;
    height: 100vh;
    gap: 10px;
}
```

---

## 19. Responsive Design

### 19.1 Media Queries
```css
/* Mobile first (défaut petit écran) */
.container {
    width: 100%;
}

/* Tablette (768px et plus) */
@media screen and (min-width: 768px) {
    .container {
        width: 750px;
    }
}

/* Desktop (1024px et plus) */
@media screen and (min-width: 1024px) {
    .container {
        width: 1000px;
    }
}

/* Desktop large (1200px et plus) */
@media screen and (min-width: 1200px) {
    .container {
        width: 1170px;
    }
}

/* Desktop extra large (1400px et plus) */
@media screen and (min-width: 1400px) {
    .container {
        width: 1320px;
    }
}
```

### 19.2 Breakpoints courants
```css
/* Extra small (phones, <576px) */
@media (max-width: 575.98px) { }

/* Small (landscape phones, ≥576px) */
@media (min-width: 576px) { }

/* Medium (tablets, ≥768px) */
@media (min-width: 768px) { }

/* Large (desktops, ≥992px) */
@media (min-width: 992px) { }

/* Extra large (large desktops, ≥1200px) */
@media (min-width: 1200px) { }

/* Extra extra large (≥1400px) */
@media (min-width: 1400px) { }
```

### 19.3 Types de media queries
```css
/* Largeur */
@media (min-width: 768px) { }
@media (max-width: 1024px) { }
@media (min-width: 768px) and (max-width: 1024px) { }

/* Hauteur */
@media (min-height: 600px) { }
@media (max-height: 800px) { }

/* Orientation */
@media (orientation: portrait) { }   /* Vertical */
@media (orientation: landscape) { }  /* Horizontal */

/* Type de média */
@media print { }        /* Impression */
@media screen { }       /* Écran */
@media speech { }       /* Synthèse vocale */

/* Combinaisons */
@media screen and (min-width: 768px) and (orientation: landscape) { }

/* Plusieurs conditions */
@media (min-width: 768px), print { }
```

### 19.4 Unités responsive
```css
/* Unités relatives */
.element {
    /* em : relatif au parent */
    font-size: 1.5em;
    
    /* rem : relatif à la racine (<html>) */
    font-size: 1.5rem;
    
    /* Pourcentage */
    width: 50%;
    
    /* Viewport width */
    width: 50vw;     /* 50% de la largeur viewport */
    font-size: 5vw;
    
    /* Viewport height */
    height: 100vh;   /* 100% de la hauteur viewport */
    
    /* vmin/vmax */
    font-size: 5vmin;  /* 5% du plus petit (width ou height) */
    font-size: 5vmax;  /* 5% du plus grand */
}

/* Recommandations */
html {
    font-size: 16px;  /* Base pour rem */
}

body {
    font-size: 1rem;  /* 16px */
}

h1 {
    font-size: 2rem;  /* 32px */
}
```

### 19.5 Images responsive
```css
img {
    max-width: 100%;
    height: auto;
    display: block;
}

/* Image de fond responsive */
.hero {
    background-image: url('image.jpg');
    background-size: cover;
    background-position: center;
    height: 100vh;
}
```

---

## 20. Transitions et Animations

### 20.1 Transitions
```css
.button {
    background-color: blue;
    transition: background-color 0.3s ease;
}

.button:hover {
    background-color: red;
}

/* Propriétés de transition */
.element {
    transition-property: all;          /* Propriété à animer */
    transition-duration: 0.3s;         /* Durée */
    transition-timing-function: ease;  /* Courbe */
    transition-delay: 0.1s;            /* Délai */
    
    /* Shorthand */
    transition: all 0.3s ease 0.1s;
    /*         prop dur  curve delay */
    
    /* Multiples transitions */
    transition: 
        background-color 0.3s ease,
        transform 0.5s ease-in-out,
        opacity 0.2s linear;
}

/* Timing functions */
.element {
    transition-timing-function: linear;
    transition-timing-function: ease;         /* Défaut */
    transition-timing-function: ease-in;
    transition-timing-function: ease-out;
    transition-timing-function: ease-in-out;
    transition-timing-function: cubic-bezier(0.1, 0.7, 1.0, 0.1);
}
```

### 20.2 Transforms
```css
.element {
    /* Translation (déplacement) */
    transform: translate(50px, 100px);  /* X, Y */
    transform: translateX(50px);
    transform: translateY(100px);
    transform: translate3d(50px, 100px, 0);
    
    /* Rotation */
    transform: rotate(45deg);
    transform: rotateX(45deg);   /* Axe X */
    transform: rotateY(45deg);   /* Axe Y */
    transform: rotateZ(45deg);   /* Axe Z */
    transform: rotate3d(1, 1, 0, 45deg);
    
    /* Échelle (agrandissement) */
    transform: scale(1.5);       /* 150% */
    transform: scale(2, 0.5);    /* X: 200%, Y: 50% */
    transform: scaleX(2);
    transform: scaleY(0.5);
    
    /* Inclinaison (skew) */
    transform: skew(20deg, 10deg);  /* X, Y */
    transform: skewX(20deg);
    transform: skewY(10deg);
    
    /* Origine de transformation */
    transform-origin: center;        /* Défaut */
    transform-origin: top left;
    transform-origin: 50% 50%;
    transform-origin: 100px 200px;
    
    /* Multiples transformations */
    transform: translate(50px, 100px) rotate(45deg) scale(1.2);
}

/* Exemple hover */
.card {
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-10px) scale(1.05);
}
```

### 20.3 Animations
```css
/* Définir une animation */
@keyframes slide-in {
    from {
        transform: translateX(-100%);
        opacity: 0;
    }
    to {
        transform: translateX(0);
        opacity: 1;
    }
}

/* Ou avec pourcentages */
@keyframes bounce {
    0% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-20px);
    }
    100% {
        transform: translateY(0);
    }
}

/* Appliquer l'animation */
.element {
    animation-name: slide-in;
    animation-duration: 1s;
    animation-timing-function: ease-out;
    animation-delay: 0.5s;
    animation-iteration-count: 1;         /* Nombre de fois */
    animation-direction: normal;
    animation-fill-mode: forwards;        /* État final conservé */
    animation-play-state: running;
    
    /* Shorthand */
    animation: slide-in 1s ease-out 0.5s 1 normal forwards;
    /*        name    dur curve   delay count dir  fill */
    
    /* Multiples animations */
    animation: 
        slide-in 1s ease-out,
        fade-in 0.5s linear 0.5s;
}

/* Propriétés d'animation */
.element {
    animation-iteration-count: infinite;  /* Infini */
    animation-direction: reverse;         /* Inverse */
    animation-direction: alternate;       /* Aller-retour */
    animation-fill-mode: none;            /* Défaut */
    animation-fill-mode: forwards;        /* Garde état final */
    animation-fill-mode: backwards;       /* Applique état initial */
    animation-fill-mode: both;            /* Les deux */
}
```

### 20.4 Exemples d'animations
```css
/* Rotation continue */
@keyframes spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
}

.spinner {
    animation: spin 2s linear infinite;
}

/* Pulsation */
@keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.1); }
}

.pulse {
    animation: pulse 1s ease-in-out infinite;
}

/* Fade in */
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

.fade-in {
    animation: fadeIn 0.5s ease-in;
}

/* Slide up */
@keyframes slideUp {
    from {
        transform: translateY(100%);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

.slide-up {
    animation: slideUp 0.6s ease-out;
}
```

---

## 21. Pseudo-classes et Pseudo-éléments

### 21.1 Pseudo-classes de lien
```css
/* États des liens */
a:link { color: blue; }           /* Non visité */
a:visited { color: purple; }      /* Visité */
a:hover { color: red; }           /* Survol */
a:active { color: orange; }       /* Cliqué */
a:focus { outline: 2px solid; }   /* Focus (clavier) */
```

### 21.2 Pseudo-classes d'interaction
```css
button:hover { background: blue; }
button:active { background: darkblue; }
button:focus { outline: 2px solid blue; }
button:disabled { opacity: 0.5; cursor: not-allowed; }

input:focus { border-color: blue; }
input:valid { border-color: green; }
input:invalid { border-color: red; }
input:required { border-left: 3px solid red; }
input:optional { border-left: 3px solid gray; }
input:checked { background: blue; }  /* Checkbox/radio */
```

### 21.3 Pseudo-classes structurelles
```css
/* Premier/Dernier enfant */
li:first-child { color: red; }
li:last-child { color: blue; }

/* Premier/Dernier de type */
p:first-of-type { font-weight: bold; }
p:last-of-type { font-style: italic; }

/* Énième enfant */
li:nth-child(2) { color: green; }        /* 2e élément */
li:nth-child(odd) { background: #f0f0f0; }   /* Impairs (1, 3, 5...) */
li:nth-child(even) { background: #fff; }     /* Pairs (2, 4, 6...) */
li:nth-child(3n) { color: red; }        /* Tous les 3 (3, 6, 9...) */
li:nth-child(3n+1) { color: blue; }     /* 1, 4, 7, 10... */
li:nth-child(-n+3) { font-weight: bold; }  /* 3 premiers */

/* Énième de type */
p:nth-of-type(2) { color: orange; }

/* Depuis la fin */
li:nth-last-child(2) { color: purple; }
p:nth-last-of-type(1) { margin-bottom: 0; }

/* Enfant unique */
p:only-child { color: red; }
p:only-of-type { font-weight: bold; }

/* Vide */
div:empty { display: none; }
```

### 21.4 Autres pseudo-classes
```css
/* Négation */
li:not(.special) { color: gray; }
input:not([type="submit"]) { border: 1px solid gray; }

/* Racine */
:root { --main-color: blue; }

/* Cible d'ancre */
:target { background: yellow; }

/* Langue */
:lang(fr) { quotes: "«" "»"; }
```

### 21.5 Pseudo-éléments
```css
/* Premier/Dernier caractère */
p::first-letter {
    font-size: 2em;
    font-weight: bold;
    float: left;
}

/* Première ligne */
p::first-line {
    font-weight: bold;
    color: blue;
}

/* Avant/Après */
.element::before {
    content: "→ ";
    color: blue;
}

.element::after {
    content: " ←";
    color: red;
}

/* Icône avec ::before */
.icon-home::before {
    content: "🏠 ";
}

/* Sélection de texte */
::selection {
    background: yellow;
    color: black;
}

::-moz-selection {  /* Firefox */
    background: yellow;
    color: black;
}

/* Placeholder */
input::placeholder {
    color: #999;
    opacity: 1;
}
```

---

## 22. Variables CSS

### 22.1 Définition et utilisation
```css
/* Définir dans :root (globales) */
:root {
    --primary-color: #007bff;
    --secondary-color: #6c757d;
    --font-size: 16px;
    --spacing: 20px;
    --border-radius: 5px;
}

/* Utiliser */
.button {
    background-color: var(--primary-color);
    font-size: var(--font-size);
    padding: var(--spacing);
    border-radius: var(--border-radius);
}

/* Valeur par défaut */
.element {
    color: var(--text-color, black);  /* black si --text-color inexistante */
}
```

### 22.2 Variables locales
```css
.card {
    --card-spacing: 15px;
    padding: var(--card-spacing);
}

.card-header {
    padding: calc(var(--card-spacing) / 2);
}
```

### 22.3 Calculs avec variables
```css
:root {
    --base-size: 16px;
}

.title {
    font-size: calc(var(--base-size) * 2);     /* 32px */
}

.subtitle {
    font-size: calc(var(--base-size) * 1.5);   /* 24px */
}

.small {
    font-size: calc(var(--base-size) * 0.875); /* 14px */
}
```

### 22.4 Thèmes avec variables
```css
/* Thème clair */
:root {
    --bg-color: white;
    --text-color: black;
    --border-color: #ddd;
}

/* Thème sombre */
[data-theme="dark"] {
    --bg-color: #1a1a1a;
    --text-color: #f0f0f0;
    --border-color: #444;
}

/* Utilisation */
body {
    background-color: var(--bg-color);
    color: var(--text-color);
}

.card {
    border: 1px solid var(--border-color);
}
```

---

## 23. Techniques avancées

### 23.1 Centrage
```css
/* Méthode 1: Flexbox */
.center-flex {
    display: flex;
    justify-content: center;
    align-items: center;
}

/* Méthode 2: Grid */
.center-grid {
    display: grid;
    place-items: center;
}

/* Méthode 3: Position absolute */
.center-absolute {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

/* Méthode 4: Margin auto (horizontal) */
.center-horizontal {
    width: 300px;
    margin: 0 auto;
}

/* Méthode 5: Text-align (inline) */
.center-text {
    text-align: center;
}
```

### 23.2 Overlay/Modal
```css
.overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.7);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
}

.modal {
    background: white;
    padding: 30px;
    border-radius: 10px;
    max-width: 500px;
    width: 90%;
    max-height: 80vh;
    overflow-y: auto;
}
```

### 23.3 Sticky Footer
```css
/* Méthode Flexbox */
body {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

main {
    flex: 1;
}

footer {
    margin-top: auto;
}

/* Méthode Grid */
body {
    display: grid;
    grid-template-rows: auto 1fr auto;
    min-height: 100vh;
}
```

### 23.4 Cards/Grille responsive
```css
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
}

.card {
    background: white;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
}
```

### 23.5 Reset CSS
```css
/* Reset basique */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Reset complet */
*, *::before, *::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    font-size: 16px;
    scroll-behavior: smooth;
}

body {
    line-height: 1.6;
    font-family: Arial, sans-serif;
}

img {
    max-width: 100%;
    display: block;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}
```

### 23.6 Utilitaires courants
```css
/* Espacement */
.m-0 { margin: 0; }
.m-1 { margin: 0.25rem; }
.m-2 { margin: 0.5rem; }
.m-3 { margin: 1rem; }
.m-4 { margin: 1.5rem; }
.m-5 { margin: 3rem; }

.mt-3 { margin-top: 1rem; }
.mb-3 { margin-bottom: 1rem; }
.mx-auto { margin-left: auto; margin-right: auto; }

.p-0 { padding: 0; }
.p-3 { padding: 1rem; }

/* Texte */
.text-left { text-align: left; }
.text-center { text-align: center; }
.text-right { text-align: right; }

.text-bold { font-weight: bold; }
.text-italic { font-style: italic; }

/* Display */
.d-none { display: none; }
.d-block { display: block; }
.d-flex { display: flex; }
.d-grid { display: grid; }

/* Couleurs */
.text-primary { color: #007bff; }
.text-danger { color: #dc3545; }
.text-success { color: #28a745; }

.bg-primary { background-color: #007bff; }
.bg-light { background-color: #f8f9fa; }
```

---

## 📌 Bonnes pratiques HTML/CSS

### Conventions de nommage
```css
/* BEM (Block Element Modifier) */
.card { }
.card__title { }
.card__body { }
.card--featured { }

/* Classes descriptives */
.container
.row
.column
.button
.button-primary
.button-secondary
```

### Organisation CSS
```css
/* 1. Reset/Normalize */
* { box-sizing: border-box; }

/* 2. Variables */
:root {
    --primary: #007bff;
}

/* 3. Typographie */
body { font-family: Arial; }
h1 { font-size: 2rem; }

/* 4. Layout */
.container { max-width: 1200px; }

/* 5. Composants */
.button { }
.card { }

/* 6. Utilities */
.text-center { }

/* 7. Media queries */
@media (min-width: 768px) { }
```

### Performance
```css
/* Éviter les sélecteurs trop complexes */
/* ❌ Mauvais */
div > ul > li > a { }

/* ✅ Bon */
.nav-link { }

/* Regrouper les propriétés */
.element {
    /* Positionnement */
    position: relative;
    top: 0;
    left: 0;
    
    /* Box model */
    width: 100%;
    padding: 20px;
    margin: 10px;
    
    /* Visuel */
    background: white;
    border: 1px solid #ddd;
    
    /* Typographie */
    font-size: 16px;
    color: black;
}
```

---

## 🎯 Exercices recommandés

**Niveau débutant:**
1. Page CV avec HTML sémantique
2. Formulaire de contact stylisé
3. Navigation responsive

**Niveau intermédiaire:**
1. Grille de cartes avec Flexbox
2. Layout complet avec Grid
3. Menu hamburger animé

**Niveau avancé:**
1. Site multi-pages responsive
2. Dashboard avec animations
3. Thème sombre/clair avec variables

---

## 📚 Ressources

- MDN Web Docs : https://developer.mozilla.org
- CSS Tricks : https://css-tricks.com
- Can I Use : https://caniuse.com
- Flexbox Froggy : https://flexboxfroggy.com
- Grid Garden : https://cssgridgarden.com

---

**🌐 Bon apprentissage HTML & CSS !**
