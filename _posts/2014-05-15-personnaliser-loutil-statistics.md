---
layout: post
title: "Personnaliser l'outil Statistics"
category: posts
---

Question : Lors de la génération de statistiques avec le canal Statistics, il ne m'est proposé que le groupe Everyone.
Comment peut-on ajouter d'autres groupes à la liste déroulante ?

Pour cela adaptez le fichier
<pre><code>
 /uportal-war/src/main/data/default_entities/event-aggregation/default.event-aggregation.xml
</code></pre>
, les statistics sont générées à partir des events agrégés. Attention quand même à bien faire attention à ce que vous faites car il y a eu de nombreux messages sur les listes au sujet de l'agrégation des event qui causaient une augmentation significative de la base et qui pouvait provoquer des arrêtes de services, donc monitorez bien votre base.
