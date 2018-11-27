---
layout: post
title: "sélection de vecteur: le bon moment"
category: posts
oderis: 4
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

<h2>Sélection de vecteur: le bon moment</h2>

Assigne les résultats de poker de mercredi à la variable "poker_mercredi"

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

# Définir une nouvelle variable basée sur une sélection
poker_mercredi <- poker_vector[3]

</code>
</div>
</body>
</html>

Pour sélectionner plusieurs éléments d'un vecteur, vous pouvez ajouter des crochets à la fin de celui-ci.
Vous pouvez indiquer entre les crochets quels éléments doivent être sélectionnés.
Par exemple: supposons que vous souhaitiez sélectionner le premier et le cinquième jour de la semaine: utilisez le vecteur c (1, 5) entre les crochets. Par exemple, le code ci-dessous sélectionne les premier et
cinquième éléments de poker_vector:

<pre><code>poker_vector[c(1,5)]
</code></pre>

Attribuez les résultats de poker de mardi, mercredi et jeudi à la variable poker_milleu_semaine

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

# Définir une nouvelle variable basée sur une sélection
poker_milleu_semaine <- poker_vector[c(2,3,4)]

</code>
</div>
</body>
</html>

Attribuez à la variable « roulette_selection_vector » les résultats de la roulette du mardi au vendredi.
Essayez d'utiliser la syntaxe ":", cela vous facilite les choses au lieu de [c(2,3,4)] :

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

# Définir une nouvelle variable basée sur une sélection
poker_selection_vector <- roulette_vector[2:5]

</code>
</div>
</body>
</html>
