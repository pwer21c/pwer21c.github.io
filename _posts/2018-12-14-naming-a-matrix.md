---
layout: post
title: "Nomer une matrice"
category: posts
oderis: 2
group: matrix
---
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Analyser les matrices</h2>


Dans les exercices suivants, vous analyserez les numéros de billetterie de la franchise Star Wars.

Le premier élément de chaque vecteur indique les recettes au box-office américain, le second élément concerne le box-office non américain (source: Wikipedia).

<pre><code>
# Le premier élément: USA, le seconde : Non-USA
new_hope <- c(460.998, 314.4)
</code></pre>

Dans cet exercice, vous combinerez toutes ces figures en un seul vecteur

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
# Box office Star Wars: En millions!
# Le premier élément: USA, le seconde : Non-USA
new_hope <- c(460.998, 314.4)
empire_strikes <- c(290.475, 247.900)
return_jedi <- c(309.306, 165.8)

# Ajoutez votre code ci-dessous pour construire une matrice
star_wars_matrix <- matrix(c(new_hope, empire_strikes, return_jedi), nrow = 3, byrow = TRUE)

</code>
</div>
</body>
</html>

<h2>Nommer une matrice</h2>

Pour vous aider à vous souvenir de ce qui est stocké dans star_wars_matrix, vous pouvez ajouter des noms pour les lignes et les colonnes d'une matrice.

<pre><code>
rownames(my_matrix) <- row_names_vector
colnames(my_matrix) <- col_names_vector
</code></pre>

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
# Box office Star Wars: En millions!
# Le premier élément: USA, le seconde : Non-USA
new_hope <- c(460.998, 314.4)
empire_strikes <- c(290.475, 247.900)
return_jedi <- c(309.306, 165.8)

# Construire une matrice
star_wars_matrix <- matrix(c(new_hope, empire_strikes, return_jedi), nrow = 3, byrow = TRUE)

# Ajoutez votre code ici pour que les lignes et les colonnes de star_wars_matrix aient un nom!
colnames(star_wars_matrix) <- c("US", "non-US")
rownames(star_wars_matrix) <- c("A New Hope", "The Empire Strikes Back", "Return of the Jedi")
</code>
</div>
</body>
</html>
