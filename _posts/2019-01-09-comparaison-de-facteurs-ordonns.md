---
layout: post
title: "7. Comparaison de facteurs ordonnés"
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

<h2>Comparaison de facteurs ordonnés</h2>

Le statisticien numéro 2 entre dans votre bureau et commence à se plaindre que le statisticien numéro 5 ralentit l'ensemble du projet. Puisque vous savez que le statisticien numéro 2 a la réputation d'être un malin, vous décidez tout d'abord de vérifier si sa déclaration est correcte.

Le fait que <code>factor_vitesse_vector</code> est maintenant ordonné permet de comparer les différents éléments (les statisticiens dans ce cas). Vous pouvez faire assez simplement cela en utilisant les opérateurs connus.

<h3>Exercice</h3>
Vérifiez si le statisticien numéro 2 est plus rapide que statisticien numéro 5 et assignez le résultat à <code>la_comparaison</code>. N'oubliez pas l'opérateur <code>></code> permet de vérifier si un élément est plus grand que l'autre.

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
vitesse_vector <- c("Rapide", "Lent", "Lent", "Rapide", "Ultra-Rapide")
factor_vitesse_vector <- factor(vitesse_vector, ordered = TRUE, levels = c("Lent", "Rapide", "Ultra-Rapide"))

# Votre code
la_comparaison <- factor_vitesse_vector[2] > factor_vitesse_vector[5]

# Est-ce que le statisticien 2 est plus rapide que le 5 ?
la_comparaison

</code>
</div>
</body>
</html>
