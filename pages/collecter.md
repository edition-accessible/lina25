---
layout: page
title: Renseigner
date: 16 mai 2023
subtitle: et référencer des informations précises
orientation: assurer la présence d’informations de qualité sur l’accessibilité des livres numériques
audience: personnes en charge de produire, renseigner ou améliorer les métadonnées auprès des distributeurs, organismes de référencement et agences bibliographiques
previous: ./traiter.html
next: ./diffuser.html
titleNext: Informer
titlePrev: Traiter
---

<div markdown="1" id="principes">

{%- include principes.html -%}

Afin de rendre possible l’information de l’utilisateur, les métadonnées renseignées et collectées sur les ouvrages numériques référencés doivent inclure les informations d’accessibilité. Cela permet aussi de mettre en valeur le travail fourni et d’avoir un chiffrage précis de l’évolution du nombre de titres rendus accessibles.

Comme ces informations et leur affichage s’inscrit dans un cadre légal, leur exactitude revêt une importance particulière car elle engage les différents acteurs, éditeurs, intermédiaires et revendeurs. Une démarche d’information et de validation devrait être mise en œuvre pour assurer cette exactitude.

Nous proposons un [dictionnaire des métadonnées](../ressources/metadonnes) pour vous aider dans cette tâche. Vous y trouverez des tableaux de correspondance définissant les conditions et l'information nécessaire en lien avec le code ONIX correspondant.  

Les recommandations françaises sur l'[affichage des informations d'accessibilité](../ressources/Informer.md) (projet en cours) peuvent-être aussi utiles pour comprendre comment chaque code devrait se matérialiser sur les sites de diffusion et de distribution.

## Les informations nécessaires

Les exigences de la directive Européenne impliquent que des informations sont disponibles sur les quatre catégories suivantes : 
* les **modes de lecture** (tout le contenu disponible en voix de synthèse et braille, affichage modifiable, synchronisation texte et audio, etc.)&#8239;; 
* les possibilitées de **navigation** dans le fichier (table des matières dans le contenu, pagination de référence d’un imprimé, etc.), 
* les **fonctionnalités du livre** (illustrations, tableaux, schémas, math, etc.) et leur accessibilité. 
* les **risques** physiologiques éventuels liés à l'épilepsie ou à l'hypersensibilité.
* le **blocage** éventuel des fonctionnalités d’accessibilité par des mesures de protection inadéquates (DRM) devrait aussi être renseigné.

Chacune de ces catégorie est détaillée dans le dictionnaire des métadonnées d'accessibilité. 
### Les informations supplémentaires utiles

#### La conformité

La meilleure façon d’assurer que les informations sont juste consiste à pratiquer des tests de contrôle pour s’assurer que le document est conforme à EPUB accessibility AA (<a href="https://ns.editeur.org/onix/en/196/03">liste 196 code 03</a>) ou A (<a href="https://ns.editeur.org/onix/en/196/02">liste 196 code 02</a>). Dans ce dernier cas il faudra aussi assurer que la mise en forme est modifiable (<a href="https://ns.editeur.org/onix/en/175/E200">Liste 175 Code E200&#8239;: Redimensionnable</a>) pour rester dans les conditions acceptables de la directive européenne.

#### Le résumé d'accessibilité 

L'ajout d'un résumé d'accessibilité (<a href="https://ns.editeur.org/onix/en/196/00">Liste 196 Code 00&#8239;: Résumé sur l’accessibilité</a>) est fortement recommandé. Le nom de ce dernier est trompeur. Il ne s'agit pas d'un résumé complet, mais d'un complément d'information, d'une clarification et d'une amélioration des autres métadonnées d'accessibilité. Cette métadonnée est particulière car c'est un champ libre dans lequel ce que vous écrirez sera transporté et affiché tel quel.

Lors de la création du résumé d'accessibilité, il faut partir du principe que les autres métadonnées d'accessibilité ont déjà été présentées et que le résumé d'accessibilité sert à améliorer ces métadonnées. Si la publication présente des caractéristiques ou des lacunes qui ne sont pas exprimées dans les autres métadonnées d'accessibilité, le résumé d'accessibilité est l'endroit approprié pour inclure ces informations. 

Ce résumé devrait être le même que celui contenu dans le fichier EPUB (<span lang="en"><i>schema.org accessibility summary</i></span>) et préciser notamment les déficiences potentielles. Un guide de rédaction de ce résumé est en cours d'élaboration au sein du groupe des éditeurs du W3C. 

#### Certificats et démarches d'accessibilité

Les informations relatives à la certification d'accessibilité contenues dans les codes 196 01 et 93 sont délivrés par des tiers qui engagent leur responsabilité.

Les codes 196 94 à 99 permettent de renseigner les utilisateurs sur la démarche d'accessibilité de l'éditeur et de leur indiquer qui contacter en cas de difficulté.

</div>

<section  class="ressources" markdown="1">
<h2> Ressources</h2>
<ul>

<li>
<a href="../ressources/metadonnes" class="link color_orange" target="_self">Dictionnaire des métadonnées d'accessibilité</a>
</li>

<li>
<span lang="en"><a href="https://w3c.github.io/publ-a11y/drafts/schema-a11y-summary/" class="link color_orange">
Accessibility Summary Authoring Guidelines for EPUB Publications Draft Community Group Report 07 December 2022</a></span>
</li>

<li>
<a href="https://ns.editeur.org/onix/fr/196" class="link color_orange">ONIX liste 196</a>
</li>

<li>
<a href="https://edition-accessible.github.io/signalement/references/references.html" class="link color_orange">Tableau de correspondances schema.org et ONIX en Français</a>
</li>

<li>
<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>
</li>

</ul>
</section>

