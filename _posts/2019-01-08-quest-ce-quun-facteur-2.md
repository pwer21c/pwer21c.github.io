---
layout: post
title: "2. Qu'est ce qu'un facteur (2)"
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

<h2>Qu'est ce qu'un facteur et pourquoi devrais-je en utiliser ? (2)</h2>

Il existe deux types de variables nominales : les variables non ordonnées et les variables ordonnées.

Une variable non ordonnée est une variable catégorielle sans ordre implicite. Cela signifie qu'il est impossible de dire qu' une valeur est supérieure à l'autre. Par exemple, pensez à la variable catégorielle <code>animals_vector</code> avec les catégories <code>"Elephant"</code>, <code>"Girafe"</code>, <code>"Singe"</code> et <code>"Cheval"</code>. Ici, il est impossible de dire qui est au-dessus ou au-dessous de l'autre.

En revanche, les variables ordinales ont un ordre naturel. Considérons par exemple la variable catégorielle <code>temperature_vector</code> avec les catégories: <code>"Faible"</code>, <code>"Moyen"</code> et <code>"Fort"</code>. Ici, il est évident que <code>"Moyen"</code> se situe au-dessus de <code>"Faible"</code>, et <code>"Fort"</code> se situe au-dessus de <code>"Moyen"</code>.

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
animals_vector <- c("Elephant", "Girafe", "Singe", "Cheval")
temperature_vector <- c("Fort", "Faible", "Fort","Faible", "Moyen")

factor_animaux_vector <- factor(animals_vector)
factor_animaux_vector
factor_temperature_vector <- factor(temperature_vector, order = TRUE, levels = c("Faible", "Moyen", "Fort"))
factor_temperature_vector

</code>
</div>
</body>
</html>
