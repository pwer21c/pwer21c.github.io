---
layout: post
title: "3. Calcul du box-office mondial"
category: posts
oderis: 3
group: matrix

---
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Calcul du box-office mondial</h2>


Pour calculer le total des recettes pour les trois films « Star Wars »,  vous devez utiliser la somme de la colonne des recettes des Etat-Unis et de la colonne des recettes non-américaines.

Dans R, la fonction <code>rowSums()</code> calcule facilement les totaux pour chaque ligne d’une matrice. Cette fonction crée un nouveau vecteur:

<pre><code>
rowSums(my-matrix)
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
# Construire star_wars_matrix
box_office <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
star_wars_matrix <- matrix(box_office, nrow = 3, byrow = TRUE,
                                     dimnames = list(c("A New Hope", "The Empire Strikes Back", "Return of the Jedi"),
                                                     c("US", "non-US")))

# Calcul du box-office mondial
worldwide_vector <- rowSums(star_wars_matrix)

</code>
</div>
</body>
</html>

<h2>Ajout d'une colonne pour le box-office mondial</h2>

Vous pouvez ajouter une colonne ou plusieurs colonnes à une matrice avec la fonction <code>cbind ()</code>, qui fusionne des matrices et / ou des vecteurs par colonne. Par exemple:

<pre><code>
big_matrix <- cbind(matrix1, matrix2, vector1 ...)
</code></pre>

Ajoutez worldwide_vector en tant que nouvelle colonne à star_wars_matrix et affectez le résultat à all_wars_matrix. Utilisez la fonction <code>cbind ()</code>.

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
# Construire star_wars_matrix
box_office <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
star_wars_matrix <- matrix(box_office, nrow = 3, byrow = TRUE,
                                     dimnames = list(c("A New Hope", "The Empire Strikes Back", "Return of the Jedi"),
                                                     c("US", "non-US")))

# Calcul du box-office mondial
worldwide_vector <- rowSums(star_wars_matrix)

# Ajouter la nouvelle variable worldwide_vector à star_wars_matrix
all_wars_matrix <- cbind(star_wars_matrix, worldwide_vector)

</code>
</div>
</body>
</html>

<h2>Ajouter une ligne</h2>

Utilisez <code>rbind ()</code> pour coller ensemble star_wars_matrix et star_wars_matrix2, dans cet ordre. Attribuez la matrice résultante à all_wars_matrix.

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
# Construire star_wars_matrix et star_wars_matrix2
box_office <- c(460.998, 314.4, 290.475, 247.900, 309.306, 165.8)
star_wars_matrix <- matrix(box_office, nrow = 3, byrow = TRUE,
                                     dimnames = list(c("A New Hope", "The Empire Strikes Back", "Return of the Jedi"),
                                                     c("US", "non-US")))


box_office2 <- c(474.5, 552.5, 310.7 , 338.7, 380.3 , 468.5)
star_wars_matrix2 <- matrix(box_office2, nrow = 3, byrow = TRUE,
                                     dimnames = list(c("The Phantom Menace", "Attack of the Clones", "Revenge of the Sith"),
                                                     c("US", "non-US")))

# Combinez les deux trilogies de Star Wars dans une matrice
all_wars_matrix <- rbind(star_wars_matrix,star_wars_matrix2)


</code>
</div>
</body>
</html>
