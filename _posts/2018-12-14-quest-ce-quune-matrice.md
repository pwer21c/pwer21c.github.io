---
layout: post
title: "1. Qu'est ce qu'une matrice?"
category: posts
oderis: 1
group: matrix
---
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Qu'est ce qu'une matrice?</h2>

Dans R, une matrice est un ensemble d'éléments du même type de données (numérique, caractère ou logique) organisés en un nombre fixe de lignes et de colonnes. Comme vous ne travaillez qu'avec des lignes et des colonnes, une matrice est appelée bidimensionnelle.

Vous pouvez construire une matrice en R avec la fonction <code>matrix ()</code>. Prenons l'exemple suivant:

<pre><code>
  matrix(1:9, byrow = TRUE, nrow = 3)
</code></pre>

Dans la fonction matrix ():

- Le premier argument est la collection d'éléments que R organisera dans les lignes et les colonnes de la matrice. Ici, nous utilisons 1: 9 qui est un raccourci pour c (1, 2, 3, 4, 5, 6, 7, 8, 9).
- L'argument byrow indique que la matrice est remplie par les lignes. Si nous voulons que la matrice soit remplie par les colonnes, il suffit de placer byrow = FALSE.
- Le troisième argument, nrow, indique que la matrice doit comporter trois lignes.

Construction d'une matrice à 3 rangées contenant les nombres de 1 à 9

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<style>
.dcl__index-module__console--2YAI1, .dcl__index-module__editor--m_p4P {font-size: 15px !important; }
.lm_header .lm_tab .lm_title {font-size: 15px !important;}
.dcl__Button-module__extra-small--2toEt, .dcl__Button-module__small--1VJc5 {font-size: 15px;}
</style>
</head>
        <body>
        	<script type="text/javascript" src="//cdn.datacamp.com/dcl-react.js.gz"></script>
			<div data-datacamp-exercise data-lang="r">
        	<code data-type="sample-code">
#Construction d'une matrice à 3 rangées contenant les nombres de 1 à 9
matrix(1:9, byrow = TRUE, nrow = 3)

</code>
</div>
</body>
</html>
