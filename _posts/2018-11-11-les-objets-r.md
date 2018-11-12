---
layout: post
title: "Les objets R"
category: posts
oderis: 4
group: initr
---
<p>Tout dans le langage R est un objet : les variables contenant des données, les fonctions, les opérateurs, même le symbole représentant le nom d’un objet est lui-même un objet. Les objets possèdent au minimum un mode et une longueur et certains peuvent être dotés d’un ou plusieurs attributs</p>
<p></p>
<p><iframe scrolling="yes" src="https://catalogue-ent2.univ-paris8.fr/datacamp/sbang/ch3_1.html" width="100%" height="330px" frameborder="0"></iframe></p>

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
            # Le mode d’un objet est obtenu avec la fonction mode :
			v <- c(1, 2, 5, 9)
			mode(v)


			#La longueur d’un objet est obtenue avec la fonction length :
			length(v)

</code>
</div>
</body>
</html>

<h1>Longeur</h1>

<p><strong>La longueur d’un objet est égale au nombre d’éléments qu’il contient.</strong>La longueur, au sens R du terme, d’une chaîne de caractères est toujours 1. Un objet de mode <strong><em>character</em></strong> doit contenir plusieurs chaînes de caractères pour que sa longueur soit supérieure à 1 :</p>

<pre><code>> v1 <- "actuariat"
> length(v1)
[1] 1
> v2 <- c("a", "c", "t", "u", "a", "r", "i", "a", "t")
> length(v2)
[1] 9
</code></pre>

<p>Il faut utiliser la fonction <em><strong>nchar </strong></em>pour obtenir le nombre de caractères dans une chaîne :</p>

<pre><code>> nchar(v1)
[1] 9
> nchar(v2)
[1] 1 1 1 1 1 1 1 1 1
</code></pre>

<p>Un objet peut être de longueur 0 et doit alors être interprété comme un contenant qui existe, mais qui est vide :</p>
<pre><code>
> v <- numeric(0)
> length(v)
[1] 0
</code></code>


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
            v1 <- "actuariat"
			length(v1)
          
			v2 <- c("a", "c", "t", "u", "a", "r", "i", "a", "t")
			length(v2)

</code>
</div>
</body>
</html>
