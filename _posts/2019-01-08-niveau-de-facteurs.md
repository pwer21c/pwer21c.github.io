---
layout: post
title: "3. Niveau de facteurs"
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

<h2>Niveau de facteurs</h2>

Lorsque vous importez un jeu de données, vous remarquerez généralement qu'il contient des facteurs avec des niveaux spécifiques. Parfois vous allez vouloir changer les noms de ces niveaux, pour des raisons de clarté ou autre. R vous permet de le faire avec la fonction <code>levels()</code> :

<pre><code>levels(factor_vector) <- c("nom1","nom2",...)
</code></pre>

Un bon exemple est le fichier brut qui vous est fourni après une enquête terrain (un sondage par exemple). Une des questions standard pour chaque questionnaire est le sexe de la personne interrogée. Vous vous souvenez de la question précédente ? Il s'agit d'un facteur et ses niveaux sont souvent notés <code>"M"</code> et "F".

<pre><code>enquete_vector <- c("M","F","F","M","M")
</code></pre>

Ensuite, lorsque vous voulez commencer votre analyse de données, votre principale préoccupation est de garder un bon aperçu de toutes les variables et de leur sens. À ce moment-là, vous voudrez sûrement changer les niveaux de facteur en indiquant <code>"Masculin"</code> et <code>"Feminin"</code> au lieu de <code>"M"</code> et <code>"F"</code> pour vous rendre la vie plus facile.

<h3>exercice</h3>

- Convertissez le vecteur de caractères <code>enquete_vector</code> dans un vecteur de facteurs. Assignez-le à « factorenquetevector ».
- Changez les niveaux de facteurs de <code>factor_enquete_vector</code> à <code>"Masculin"</code> et <code>"Feminin"</code>.

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
enquete_vector <- c("M", "F", "F", "M", "M")

# Convertissez enquete_vector en facteurs
factor_enquete_vector <- factor(enquete_vector)

# Spécifiez les niveaux de  factor_enquete_vector
levels(factor_enquete_vector) <- c("Feminin", "Masculin")

factor_enquete_vector

</code>
</div>
</body>
</html>
