---
layout: post
title: "Calculer le gain total"
category: posts
oderis: 2
group: vector
---

<h2>Calculer le gain total</h2>

Vous pouvez nommer les éléments d’un vecteur. Surtout, pour les variables poker et roulette, vous avez bien nommé les éléments de deux vecteur.
Dans ce cours, vous allez répondre aux questions suivantes :

- Quel a été votre bénéfice ou votre perte en une semaine ?
- Au total, avez-vous perdu de l’argent au cours de la semaine ?
- Gagnez/perdez-vous de l’argent au poker ou à la roulette ?

Pour obtenir les réponses, vous devez faire des calculs arithmétiques sur des vecteurs.
Il est important de savoir que si vous additionnez deux vecteurs dans R, cela prend la somme par élément. Par exemple, les trois instructions suivantes sont complètement équivalentes:

<pre><code>c(1, 2, 3) + c(4, 5, 6)
c(1 + 4, 2 + 5, 3 + 6)
c(5, 7, 9)</code></pre>

Vous pouvez également faire les calculs avec des variables représentant des vecteurs:

<pre><code>a <- c(1, 2, 3) 
b <- c(4, 5, 6)
c <- a + b</code></pre>

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
A_vector <- c(1, 2, 3)
B_vector <- c(4, 5, 6)

#Prendre la somme de A_vector et B_vector
total_vector <- A_vector+B_vector
  
#Imprimer total_vector
total_vector
             
</code>
</div>
</body>
</html>
