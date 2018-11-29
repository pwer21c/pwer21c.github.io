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


# Poker and roulette winnings from Monday to Friday:
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

# Which days did you make money on poker?
selection_vector <- poker_vector > 0

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

#Imprimer les jours de gagnants pour le poker
poker_winning_days

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

#Gagnants au poker ?
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
