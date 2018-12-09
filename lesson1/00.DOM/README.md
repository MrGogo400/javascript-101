# Document Object Model

+ [w3school](https://www.w3schools.com/js/js_htmldom_eventlistener.asp)
+ [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
+ [JavaScript.info](http://javascript.info/dom-nodes)


## Trouver un node

Utilisez: `getElementById`, `getElementsByClassName`, `getElementsByTagName`, `querySelector`, `querySelectorAll`

+ Trouvez toutes les balises `div` du document. Loggez le deuxième élément s'il est présent.
+ Trouvez toutes les balises `p` avec la classe 'my-paragraph' du document. Loggez le premier élément s'il est présent.
+ Trouvez la balise `span` avec l'id 'js-unique-el'. Loggez-là. Inspéctez les propriétés de cet objet [Element](https://developer.mozilla.org/en-US/docs/Web/API/Element)
+ Trouvez toutes les balises `p` qui se trouvent dans un div. 
+ Trouvez toutes les balises `span` qui sont précédées par un div. 

```html
<div>
  <p class="main-paragraph">Paragraph 1</p>
</div>
<div>
  <p class="secondary-paragraph">Paragraph 2</p>
</div>
<span></span>
<div>
  <p class="secondary-paragraph">Paragraph 3</p>
</div>
<p class="secondary-paragraph">Paragraph 3</p>
<span id="js-unique-el"></span>
```

> **Bonne pratique :** si vous créez une classe ou un id pour manipuler les éléments avec JS, prefixez leurs noms avec 'js-', comme `.js-my-class`


## Inspécter un node

Utilisez la console pour regarder toutes les propriétés et méthodes associés à un node.
Console > Séléctionner un élément > Elements > Properties

![Quick DOM Inspector](https://i.ibb.co/X7bW84V/DOM-inspector.png)


## Modifier un node

Ajoutez le texte 'I am the first paragraph' au premier paragraphe du document.
Ajoutez le HTML `<span>Hello</span>` au deuxième paragraphe du document.
Modifiez les attributs `width` à 50% et `height` à 'auto' de l'image.
Ajoutez un attribut `alt` pas vide à l'image.
Donnez la couleur 'blue' au premier paragraphe du div et la taille de police '1.5rem'.

```html
<p class="first-p"></p>
<p class="second-p"></p>
<img src="path/to/image.jpg" width="10" height="10">
<div><p>I'm inside of a div</p></div>

```

## Supprimer un node

Supprimez le paragraphe qui se trouve dans un div.
Supprimez le span.

```html
<p>I will not be deleted</p>
<div>
  <p>I will be deleted</p>
</div>
<span>I will be deleted</span>
```

## Créez un node

Créez un div et insérez le dans la balise `body`.
Créez une balise `ul` avec 5 `li`s dedans et insérez la dans un div dans body. N'hésitez pas à utiliser la boucle `for` pour ne pas répéter la même ligne de code 5 fois.

---

Créez une balise `script` qui télécharge la librairy jQuery `https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js` en manière asynchrone.

## Pour aller plus loin

Recréez le HTML suivant uniquement avec JavaScript.

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Page Title</title>
</head>
<body>
  <!-- from here -->
  <main>
    <h1>Main title</h1>
    <p>Here goes the <strong>description</strong></p>
  
    <img src="path/to/image.jpg" alt="My image" width="30%">
  </main>

  <div class="cookies" style="background-color:#fdfdfd; border-radius: 4px;">
    <p>Hello, this site uses cookies! <span class="cookie-icon" data-custom-id="35"></span></p>
  </div>

  <footer>
    <ul class="links">
      <li>Link 1</li>
      <li>Link 2</li>
      <li>Link 3</li>
      <li>Link 4</li>
      <li>Link 5</li>
      <li>Link 6</li>
      <li>Link 7</li>
      <li>Link 8</li>
      <li>Link 9</li>
      <li>Link 10</li>
      <li>Link 11</li>
      <li>Link 12</li>
      <li>Link 13</li>
    </ul>
  </footer>

  <!-- till here -->
</body>
</html>
```

## Reading List

+ [Eloquent JavaScript > DOM](https://eloquentjavascript.net/14_dom.html)

