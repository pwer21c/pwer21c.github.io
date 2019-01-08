---
layout: post
title: "1. Qu'est ce qu'un facteur"
category: posts
group: factor
---

<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Qu'est ce qu'un facteur et pourquoi devrais-je en utiliser ?</h2>

Le terme de <code>factor</code> se réfère à un type de données statistiques utilisé pour stocker les variables nominales (on dit aussi qualitatives ou catégorielles). La différence entre une variable catégorielle et une variable continue, c'est qu'une variable catégorielle ne peut contenir qu'un nombre limité de catégories. Une variable continue, quant à elle, peut correspondre à un nombre infini de valeurs.

Il est important que R sache s'il traite une variable continue ou une variable catégorielle, car les modèles statistiques, que vous allez développer dans l'avenir traitent les deux types différemment. (Vous verrez plus tard pourquoi c'est le cas.)

La variable 'Sexe' en est un bon exemple d'une variable qualitative. Un individu humain peut être 'Masculin' ou 'Féminin', faisant abstraction des intersexués. 'Masculin' et 'Féminin' sont, de manière simplifiée, les deux valeurs de la variable qualitative 'Genre' et chaque valeur de cette variable ne peut contenir que 'Masculin' et 'Féminin'.

Pour créer des <code>factor</code> dans R, utilisez la fonction <code>factor()</code>. La première chose que vous devez faire est de créer un vecteur qui contient toutes les observations qui appartiennent à un nombre limité de catégories. Par exemple, <code>genre_vector</code> contient le sexe de 5 personnes différentes :

<pre><code>genre_vector <- c("Masculin","Feminin","Feminin","Masculin","Masculin")
</code></pre>

Il est clair ici qu'il y a 2 catégories, ou dans R des 'factor levels', il s' agit de "Masculin" et "Feminin".

La fonction <code>factor()</code> va encoder le vecteur comme un factor :

<pre><code>factor_genre_vector <- factor(genre_vector)
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
genre_vector <- c("Masculin", "Feminin", "Feminin", "Masculin", "Masculin")

# Fabriquez factor_genre_vector en utilisant 'factor()'
factor_genre_vector <- factor(genre_vector)
factor_genre_vector

</code>
</div>
</body>
</html>
