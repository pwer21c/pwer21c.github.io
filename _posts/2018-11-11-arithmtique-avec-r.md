---
layout: post
title: "Arithmétique avec R"
category: posts
suboderis: 1
group: initr
---

<div></div>
<div><span id="result_box" lang="fr">R peut être utilisé comme une simple calculatrice. Considérons les opérateurs arithmétiques suivants:</span></div>
<div></div>
<div>
<ul>
<li>Une addition +</li>
<li>Soustraction -</li>
<li>Multiplication *</li>
<li>Division /</li>
<li>Puissance  ^</li>
<li>Modulo %%</li>
</ul>
</div>
<div>
<div><span class="short_text" lang="fr"> </span><span class="short_text" lang="fr">Les deux derniers pourraient avoir besoin d’explications:</span></div>
<div>
<ul>
<li>l'opérateur de puissance (^) est évalué de droite à gauche ; tous les autres de gauche à droite. Ainsi, 2^2^3 est 2^8, et non 4^3</li>
<li>L'opérateur modulo retourne le reste d'une division :
<ul>
<li>5 %%2   ( 5/2 =1 reste 1)</li>
</ul>
</li>
</ul>
</div>
</div>
<p><span id="result_box" lang="fr">Avec cette connaissance, suivez les instructions ci-dessous pour compléter l'exercice.</span></p>
<p></p>

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
            # Une addition
            5 + 5
            
            # Une soustraction
            5 - 5
            
            # Une multiplication
            3 * 5
            
            # Une division
            (5 + 5)/2
            
            # Une puissance
            2^2^3
            
            # L'opérateur modulo
            28 %% 6

</code>
</div>
</body>
</html>
