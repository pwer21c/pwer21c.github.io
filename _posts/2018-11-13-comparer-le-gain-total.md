---
layout: post
title: "Comparer le gain total"
category: posts
oderis: 3
group: vector
---

<h2>Comparer le gain total</h2>

- Calculez total_poker et total_roulette comme l'exercice précédent. Utilisez la fonction sum ().
- Vérifiez si vos gains totaux au poker sont supérieurs à ceux de la roulette en utilisant une comparaison. 
- Imprimez simplement le résultat de cette comparaison. 
- Quelle est votre conclusion ? Est-ce que vous voulez concenter sur la roulette ou le poker ?

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

#Gagnants au poker du lundi au vendredi
poker_vector <- c(140, -50, 20, -120, 240)
roulette_vector <- c(-24, -50, 100, -350, 10)
days_vector <- c("Lundi", "Mardi", "Mercredi", "Jeudi", "Vendredi")
names(poker_vector) <- days_vector
names(roulette_vector) <- days_vector

#Calculez total_poker et total_roulette 
total_poker <-sum(poker_vector)
total_roulette <-sum(roulette_vector)

#Vérifiez si vos gains totaux au poker sont supérieurs à ceux de la roulette 
total_poker > total_roulette

</code>
</div>
</body>
</html>