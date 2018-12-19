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
# Construct star_wars_matrix
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
