---
layout: page
title: Informer
date: 2024-09-09
subtitle: et conseiller au plus près des besoins
orientation: informer le lecteur avant achat ou emprunt.
audience: libraires et bibliothèques
previous: ./collecter.html
next: ./afficher.html
titleNext: Afficher
titlePrev: Renseigner
---

<div markdown="1" id="principes">
{%- include principes.html -%}

Trouver, acheter et finalement lire une publication est une expérience personnelle. Pour les personnes empêchées de lire le texte imprimé du fait d'un handicap, cette démarche implique de se poser des questions du type _pourrais-je modifier la police d'affichage et sa taille&#8239;; mon lecteur d’écran fonctionnera-t-il avec ce titre&#8239;; y a-t-il des descriptions d’images qui seront énoncées&#8239;; y a-t-il des référence aux pages du livre imprimé&#8239;; l’ordre de lecture est-il logique_.

Les lecteurs peuvent utiliser différents services en ligne que ce soient les sites des librairies indépendantes, des portails reliés à un dispositif de lecture ou encore des bibliothèques publiques ou spécialisées. La recherche d’un ouvrage particulier peut aussi amener le lecteur à consulter des sites internationaux ou localisés dans d’autres pays. Les mêmes informations devraient être retrouvées dans ces différents cas de figure afin de garantir une expérience utilisateur équivalente sans avoir à comprendre un nouveau mode de fonctionnement pour trouver l’information pertinente.

Le groupement des éditeurs du W3C propose un guide pour homogénéiser cette expérience utilisateur. Initialement publié en septembre 2021, il a servi de base à plusieurs projets d’implémentation et a été revue courant 2024 en fonction des retours obtenus de ces expériences.

En France EDRLab a été missionné pour étudier, en collaboration avec les différents acteurs de la chaîne du livre en France, comment devraient être affichées sur les sites de distribution les métadonnées relatives à l’accessibilité des livres numériques. Ce travail est en lien étroit avec les recommandations du W3C.

Une première implémentation de ces recommandation est visibles sur 140 sites de librairies opérés par Titelive, comme par exemple la fiche concernant le [Cours de Poétique de Paul Valéry sur epagine](https://www.epagine.fr/ebook/9782072907098-cours-de-poetique-tome-1-le-corps-et-l-esprit-1937-1940-paul-valery/#targetAccess).  

### Les informations nécessaires

Les livres qui répondent aux exigences de la directive Européenne doivent indiquer qu'ils&#8239;:

-   permettent la lecture non visuelle (vocalisée ou transmise à un dispositif braille)&#8239;;
-   permettent la modification de l'affichage&#8239;;
-   permettent la navigation via une table des matières et la structure.

Les fonctionnalités spécifiques à certains types de contenus doivent aussi être indiquées. Cela comprend&#8239;:

-   la présence d'audio pré enregistrés synchronisés avec le texte&#8239;;
-   la présence d'une pagination de référence à un livre imprimé&#8239;;
-   la présence de formules mathématiques, chimiques ou physiques dans un format accessibles&#8239;;
-   la présence de descriptions détaillées pour les graphiques de données&#8239;;
-   la présence de flashs, sons ou simulations de mouvement qui peuvent déclencher des crises chez les personnes à risque.

<span class="exergue">Pour les personnes en charge de définir Le tableau de correspondances de la recommandation française indique comment obtenir, prioriser et labelliser ces informations. Ces travaux sont encore en cours.</span>

### Les autres informations utiles

Certains éditeurs font le choix de déclarer la conformité de leurs livres numériques que cette conformité soit attestée par leurs services ou par des tiers de confiance. Dans ces cas, il est important d'informer les lecteurs de cette démarche et de donner accès aux documents mis à disposition comme les rapports d'accessibilité, les liens vers les déclarations des éditeurs ou les contacts définis par ces derniers.

Certains livres particuliers ont des fonctionnalités d'accessibilité peu communes ou bien seront presque accessibles à un détail prêt. Pour cela le résumé d'accessibilité permet à l'éditeur de donner une information que les autres métadonnées ne peuvent pas transporter.

<span class="exergue">Le [dictionnaire des métadonnées](https://www.lina25.fr/ressources/metadonnees) de la recommandation française indique comment obtenir, prioriser et labelliser ces informations. </span>

### Le choix du vocabulaire

Afin que les lecteurs n'aient pas à interpréter un nouveau vocabulaire sur chaque site de vente ou de prêt en ligne, un vocabulaire type est proposé. Il est issu de plusieurs sondages et panels organisés en partenariat avec les acteurs concernés. Si vous voulez plus de renseignements sur la démarche et les résultats vous pouvez vous référer aux résultats de l'étude.

### Mesures techniques de protection (DRM)

Lorsqu’ils choisissent de recourir à des mesures techniques de protection des livres numériques qu’ils commercialisent, les éditeurs doivent veiller à ce que celles-ci ne puissent faire obstacle aux fonctions d’accessibilité.

Les techniques de marquage par filigrane ne posent aucun problème d'accessibilité. En revanche des techniques plus robustes faisant appel au chiffrement des données peuvent avoir un impact non négligeable si elles empêchent l'extraction du texte dont les technologies d'assistance ont besoin pour restituer le contenu en audio ou en braille.

Les deux solutions actuellement disponibles pour le chiffrement des fichiers sont Adobe Adopt et Readium LCP. Leur usage implique une restriction des dispositifs utilisables par le lecteur.

-   Adobe Adopt permet la lecture sur le logiciel Adobe Digital Edition. Cette DRM nécessite aussi la création d'un compte et son usage est soumis au Règlement Général pour la Protection des Données (RGPD).
-   Readium LCP permet la lecture sur un grand nombre d'applications comme Aldiko Next, Thorium Reader et d'autres applications basées sur Readium SDK&#8239;; mais permet aussi la lecture sur des dispositifs matériels comme les Pocketbook e-ink readers (dont les liseuses Vivlio). Readium LCP ne collecte aucune information sur les lecteurs qui l'utilisent.

</div>

<section  class="ressources" markdown="1">

<h2>Ressources</h2>

<h3> Informer sur l’accessibilité des livres numériques</h3>

<ul>
<li>
<a href="../ressources/Informer" class="link color_orange" target="_self">recommandations françaises sur l'affichage des informations d'accessibilité</a>
</li>
<li>
<a href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/" class="link color_orange" target="_self" lang="en">Accessibility Metadata Display Guide for Digital Publications 2.0 </a>(en anglais)
</li>
<li>
<a href="../ressources/signalement" class="link color_orange">Méthodologie et prototype de l'étude Française (2021-2024)</a>
</li>
<li>
<a href="../ressources/signalement-en" class="link color_orange" lang="en">Methodology and prototype of the French study (2021-2024)</a> (en anglais)
</li>
<li>
<a href="../ressources/signpostingprototypefr" class="link color_orange">Prototype d'affichage des informations d'accessibilité</a>
</li>
<li>
<a href="https://edition-accessible.github.io/signalement/vocabulaire.html" class="link color_orange">Les résultats de l'étude sur le vocabulaire (2022)</a>
</li>
</ul>

<h3> Mesures techniques de protection (DRM)</h3>

<a href="https://www.edrlab.org/readium-lcp/" class="link color_orange">Readium LCP (en anglais)</a>

</section>

