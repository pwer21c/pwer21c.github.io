---
layout: post
title: "6. Les facteurs ordonnés"
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

<h2>Les facteurs ordonnés</h2>

<code>vitesse_vector</code> doit être converti en un facteur ordinal puisque ses niveaux ont un ordre naturel. Par défaut, la fonction <code>factor()</code> transforme <code>vitesse_vector</code> en un factor non ordonné. Pour créer un factor ordonné, vous devez ajouter deux arguments supplémentaires: <code>ordered</code> et <code>levels</code>.

<pre><code>factor(un_vector, ordered = TRUE, levels = c("Level_1", "Level_2"...))
</code></pre>

En définissant l'argument <code>ordered</code> à <code>TRUE</code> dans la fonction <code>factor()</code>, vous indiquez que le factor est ordonné. Avec l'argument levels vous donnez les valeurs du factor dans l'ordre correct, par exemple
<pre><code>levels = c("Faible", "Moyen", "Fort").
</code></pre>

L'exemple de code ci-dessus permet de définir une variable <code>factor_vitesse_vector</code> en tenant compte du fait qu'il y a un ordre spécifique pour les niveaux de facteur. Ne changez rien aux autres lignes de code, cela imprimera le facteur dans la console et générera un résumé de celui-ci.

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

# Rajoutez votre code ci dessous
factor_vitesse_vector <- factor(vitesse_vector, ordered = TRUE, levels= c("Lent", "Rapide", "Ultra-Rapide"))

# Visualisation
factor_vitesse_vector

# R affiche automatiquement le bon ordre
summary(factor_vitesse_vector)

</code>
</div>
</body>
</html>
