---
layout: post
title: "2. Test de Student pour un échantillon"
category: posts
group: inference
---

<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>


<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"></script>

<h2>Test de Student pour un échantillon</h2>

On pèse 15 pots de confiture, et on obtient les valeurs (en grammes)

253  247,4  247  246  251  255  244  245  243,5  254,5  243,6  247,3  249  248,6  247,2

Vous souhaitiez vérifier si la moyenne est différente de 250

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
# vos données
poids<-c(253,247.4,247,246,251,255,244,245,243.5,254.5,243.6,247.3,249,248.6 , 247.2)
# Nous voulons savoir si le poids moyen des souris diffère de 25 g (test bilatéral)?
res <- t.test(poids, mu = 25,alternative = "two.sided")
# Printing the results
res

</code>
</div>
</body>
</html>

<pre><code>
	One Sample t-test

data:  poids
t = 230.14, df = 14, p-value < 2.2e-16
alternative hypothesis: true mean is not equal to 25
95 percent confidence interval:
 246.0605 250.2195
sample estimates:
mean of x
   248.14
</code></pre>

<b>Dans le résultat ci-dessus:</b>

t est la valeur statistique du test t (t = 230,14),
df est le degré de liberté (df = 14),
La valeur p est le niveau de signification du test t (valeur p = 2.2 ^ {- 16}).
conf.int est l' intervalle de confiance de la moyenne à 95% (conf.int = [246.0605 ;250.2195]);
estimations de l’échantillon est la valeur moyenne de l’échantillon (moyenne = 248,14).

<b>Interprétation du résultat</b>

La valeur p du test est 2.2 ^ {- 16}, ce qui est inférieur au niveau de signification alpha = 0,05. Nous pouvons en conclure que le poids moyen des confitures est significativement différent de 250 g avec une valeur p = 2.2 ^ {- 16}.
