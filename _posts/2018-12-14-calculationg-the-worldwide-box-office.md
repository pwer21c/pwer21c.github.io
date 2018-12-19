---
layout: post
title: "3. Calcul du box-office mondial"
category: posts
oderis: 3
group: matrix

---
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>

<h2>Calcul du box-office mondial</h2>


Pour calculer le total des recettes pour les trois films « Star Wars »,  vous devez utiliser la somme de la colonne des recettes des Etat-Unis et de la colonne des recettes non-américaines.

Dans R, la fonction <code>rowSums()</code> calcule facilement les totaux pour chaque ligne d’une matrice. Cette fonction crée un nouveau vecteur:

<pre><code>
rowSums(my-matrix)
</code></pre>
