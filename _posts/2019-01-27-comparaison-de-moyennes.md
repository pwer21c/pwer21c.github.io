---
layout: post
title: "1. Comparaison de moyennes"
category: posts
group: inference
---



<script async src="https://www.googletagmanager.com/gtag/js?id=UA-15159522-6"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-15159522-6');
</script>


<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"></script>

<h2>Test de Student pour un échantillon</h2>

1) Comparaison d'une moyenne observée à une valeur théorique

2) Conditions d'application: X bar doit être distribuée selon une loi normale (théorème central limite).
  - X suit une loi normale ou
  - n est grand

3) Hypothèses:
  - $$H_0$$: $$\mu = \mu_{0}$$
  - $$H_1$$: $$\mu \ne \mu_0$$ ("two.sided"), $$\mu < \mu_0$$("less") ou $$\mu > \mu_0$$ ("greater")

4) Statistique: Sous $$H_0$$  
  -  $$ t_{(n-1)ddl}=\frac{\bar{x}-\mu_0}{\sqrt{\frac{s^2}{n}}}$$ suit une loi de Student à n-1 ddl


<h2>Test de Student pour deux échantillons appariés</h2>

1) Comparaison des moyennes de deux échantillons appariés.

2) Préambule: Calcul des différences de toutes les paires (Y = $$X_1 - X_2$$), calcul de la moyenne des différences ($$\bar{Y}$$), calcue de la variance des différences ($$s_Y^2$$)

3) Condition d'application: $$\bar{Y}$$ doit être distribuée selon une loi normale (théorème central limite).
    - n est grand (n > 30) ou ...
    - ... la normalité des données (Y) est vérifiée

4) Hypothèses:
- $$H_0$$: $$\mu_1 = \mu_2$$
- $$H_1$$: $$\mu_1 \ne \mu_2$$ ("two.sided"), $$\mu_1 < \mu_2$$("less") ou $$\mu_1 > \mu_2$$ ("greater")

5) Statistique: Sous $$H_0$$  
-  $$ t_{(n-1)ddl}=\frac{\bar{y}-0}{\sqrt{\frac{s_y^2}{n}}}$$ suit une loi de Student à n-1 ddl

<h2>Test de Student pour deux échantillons indépendants</h2>

1) Conditions d'utilisation: $$\bar{X_1}$$ et $$\bar{X_2}$$ doivent être distribuées selon une loi normale (théorème central limite).
- $$n_1$$ et $$n_2$$ sont grands (n > 30) ou ...
- ... la normalité des données ($$X_1$$ et $$X_2$$) est vérifiée

2) Hypothèses:
- $$H_0$$: $$\mu_1 = \mu_2$$
- $$H_1$$: $$\mu_1 \ne \mu_2$$ ("two.sided"), $$\mu_1 < \mu_2$$("less") ou $$\mu_1 > \mu_2$$ ("greater")

3) Statistique: Sous $$H_0$$
- Si les variances sont égales   
  -  $$ t=\frac{\bar{x_1}-\bar{x_2}}{s\sqrt{\frac{1}{n_1} + \frac{1}{n_2}  }}$$ avec $$s=\sqrt{ \frac{ (n_1-1)s_1^2 + (n_2-1)s_2^2    }{  (n_1+n_2-2) } } $$ suit une loi de Student à $$n_1+n_2-2$$ ddl
- Si les variances sont différentes (test de Welch)   
  -  $$t=\frac{\bar{x_1}-\bar{x_2}}{s}$$ avec $$s=\sqrt{ \frac{ s_1^2}{n_1} + \frac{ s_2^2}{n_2} } $$ suit une loi de Student à $$ \frac{ ( s_1^2/n_1 + s_2^2/n_2  )^2  }{ (s_1^2/n_1)^2/(n_1-1) + (s_2^2/n_2)^2/(n_2-1)   } $$ ddl
