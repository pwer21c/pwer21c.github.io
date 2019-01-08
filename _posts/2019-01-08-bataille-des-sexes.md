---
layout: post
title: "5. Bataille des sexes"
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

<h2>Bataille des sexes</h2>

Dans <code>factor_enquete_vector</code>, nous avons un facteur à deux niveaux : Masculin et Féminin. Mais comment R compare t'il ces valeurs l'une par rapport à l'autre ? En d'autres termes, pour R qu'est-ce qui est le plus grand, Masculin ou Féminin ?

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
enquete_vector <- c("M", "F", "F", "M", "M")
factor_enquete_vector <- factor(enquete_vector)
levels(factor_enquete_vector) <- c("Feminin", "Masculin")

# Masculin
factor_enquete_vector[1]

# Féminin
factor_enquete_vector[2]

# Guerre des sexe : Masculin est il plus grand que Féminin ?
factor_enquete_vector[1] > factor_enquete_vector[2]

</code>
</div>
</body>
</html>
