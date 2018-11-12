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

<h1>Longeur</h1>

<p><strong>La longueur d’un objet est égale au nombre d’éléments qu’il contient.</strong>La longueur, au sens R du terme, d’une chaîne de caractères est toujours 1. Un objet de mode <strong><em>character</em></strong> doit contenir plusieurs chaînes de caractères pour que sa longueur soit supérieure à 1 :</p>
<table style="background-color: #c8c7c3; width: 484px; height: 147px;" border="0">
<tbody>
<tr>
<td>
<p><span style="font-size: medium;">f<span style="font-size: small;">&gt; v1 &lt;- "actuariat"</span></span></p>
<p><span style="font-size: small;">&gt; length(v1)</span></p>
<p><span style="font-size: small;">[1] 1</span></p>
<p><span style="font-size: small;">&gt; v2 &lt;- c("a", "c", "t", "u", "a", "r", "i", "a", "t")</span></p>
<p><span style="font-size: small;">&gt; length(v2)</span></p>
<p><span style="font-size: small;">[1] 9</span></p>
</td>
</tr>
</tbody>
</table>
<p></p>
<p>Il faut utiliser la fonction <em><strong>nchar </strong></em>pour obtenir le nombre de caractères dans une chaîne :</p>
<table style="background-color: #c8c7c3; width: 484px; height: 147px;" border="0">
<tbody>
<tr>
<td>
<p><span style="font-size: small;">&gt; nchar(v1)</span></p>
<p><span style="font-size: small;">[1] 9</span></p>
<p><span style="font-size: small;">&gt; nchar(v2)</span></p>
<p><span style="font-size: small;">[1] 1 1 1 1 1 1 1 1 1</span></p>
</td>
</tr>
</tbody>
</table>
<p>Un objet peut être de longueur 0 et doit alors être interprété comme un contenant qui existe, mais qui est vide :</p>
<table style="background-color: #c8c7c3; width: 484px; height: 147px;" border="0">
<tbody>
<tr>
<td>
<p><span style="font-size: small;">&gt; v &lt;- numeric(0)</span></p>
<p><span style="font-size: small;">&gt; length(v)</span></p>
<p><span style="font-size: small;">[1] 0</span></p>
</td>
</tr>
</tbody>
</table>
<p><br /><br /></p>
<p><iframe scrolling="yes" src="https://catalogue-ent2.univ-paris8.fr/datacamp/sbang/ch3_2.html" width="100%" height="330px" frameborder="0"></iframe></p>
