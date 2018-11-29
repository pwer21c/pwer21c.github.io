---
layout: post
title: "sélection par comparaison"
category: posts
oderis: 5
group: vector
---
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Sélection par comparaison</h2>

En utilisant des opérateurs de comparaison, nous pouvons aborder la question précédente de manière plus proactive.
Les opérateurs de comparaison (logiques) connus de R sont:

- <code><</code> pour moins de
- <code>></code> pour plus de
- <code><=</code> pour inférieur ou égal à
- <code>>=</code> pour supérieur ou égal à
- <code>==</code> pour égaux les uns aux autres
- <code>!=</code> pour  pas égal les uns aux autres

Comme indiqué dans l'exercice précédent, indiquer <code>6> 5</code> renvoie VRAI. La bonne chose à propos de R est que vous pouvez utiliser ces opérateurs de comparaison également sur des vecteurs.
Par exemple:

<pre><code>
  > c(4, 5, 6) > 5
  [1] FALSE FALSE TRUE
</code></pre>

Cette commande teste pour chaque élément du vecteur si la condition indiquée par l'opérateur de comparaison est TRUE ou FALSE.

- Vérifiez quels éléments de poker_vector sont positifs (c'est-à-dire> 0) et attribuez-les à selection_vector.
- Imprimez selection_vector afin que vous puissiez l'inspecter. L'impression vous indique si vous avez gagné (VRAI) ou perdu (FAUX) de l'argent pour chaque jour.

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
#Gagnants au poker et à la roulette du lundi au vendredi
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Quels jours as-tu gagné de l'argent au poker?
selection_vector <- poker_vector >0

#Imprimer la variable "selection_vector"
selection_vector

</code>
</div>
</body>
</html>

Dans les exercices précédents que vous avez utilisés
<code>selection_vector <- poker_vector > 0</code> pour trouver les jours où vous avez eu un retour positif au poker.
Maintenant, vous voudriez savoir non seulement les jours sur lesquels vous avez gagné, mais aussi combien vous avez gagné ces jours-là.
Vous pouvez sélectionner les éléments souhaités en mettant selection_vector entre les crochets qui suivent poker_vector:

<pre><code>poker_vector[selection_vector]</code></pre>

Utilisez selection_vector entre crochets pour affecter les montants que vous avez gagnés les jours les plus rentables à la variable poker_winning_days.

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
#Gagnants au poker et à la roulette du lundi au vendredi
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Quels jours as-tu gagné de l'argent au poker?
selection_vector <- poker_vector >0

#Utilisez selection_vector entre crochets pour
#affecter les montants que vous avez gagnés
#les jours les plus rentables à la variable poker_winning_days.


</code>
<code data-type="solution">
#Gagnants au poker et à la roulette du lundi au vendredi
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

#Quels jours as-tu gagné de l'argent au poker?
selection_vector <- poker_vector >0

#Utilisez selection_vector entre crochets pour
#affecter les montants que vous avez gagnés
#les jours les plus rentables à la variable poker_winning_days.

poker_winning_days <- poker_vector[selection_vector]
poker_winning_days
  </code>
	<code data-type="sct">
		test_object("poker_vector")
    success_msg("Bravo !")
	</code>
	<div data-type="hint">
    Utiliser les vecteurs poker_vector et selection_vector
  </div>

</div>
</body>
</html>
