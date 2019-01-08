---
layout: post
title: "4. Décrire un factor"
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

<h2>Décrire un factor</h2>

Après avoir terminé ce cours, une de vos fonctions préférées dans R sera <code>summary()</code>. Cela vous donnera un aperçu rapide de une_variable :

<pre><code>summary(une_variable)
</code></pre>

Pour en revenir à notre enquête, vous souhaitez savoir combien de réponses <code>"Masculin"</code> et combien de réponses <code>"Feminin"</code> vous avez dans votre étude. La fonction <code>summary()</code> vous donne la réponse à cette question.

<h3>Exercice</h3>

Utilisez <code>summary()</code> sur les vecteurs <code>enquete_vector</code> et <code>factor_enquete_vector</code>. Interpréter les résultats de ces deux vecteurs. Sont-ils équivalents dans ce cas ?

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
factor_enquete_vector <- factor(enquete_vector)
levels(factor_enquete_vector) <- c("Feminin", "Masculin")
factor_enquete_vector

# Placez votre code ici pour enquete_vector
summary(enquete_vector)

# Placez votre code ici pour factor_enquete_vector
summary(factor_enquete_vector)

</code>
</div>
</body>
</html>
