---
layout: page
title: Renseigner
date: 2025-09-04
subtitle: et référencer des informations précises
orientation: assurer la présence d’informations de qualité sur l’accessibilité des livres numériques
audience: personnes en charge de produire, renseigner ou améliorer les métadonnées auprès des distributeurs, organismes de référencement et agences bibliographiques
previous: ./produire.html
next: ./diffuser.html
titleNext: Informer
titlePrev: Produire
---

<div markdown="1" id="principes">

{%- include principes.html -%}

Afin de rendre possible l’information de l’utilisateur, les métadonnées renseignées et collectées sur les ouvrages numériques référencés doivent inclure les informations d’accessibilité. Cela permet aussi de mettre en valeur le travail fourni et d’avoir un chiffrage précis de l’évolution du nombre de titres rendus accessibles.

Comme ces informations et leur affichage s’inscrit dans un cadre légal, leur exactitude revêt une importance particulière car elle engage les différents acteurs, éditeurs, intermédiaires et revendeurs. Une démarche d’information et de validation devrait être mise en œuvre pour assurer cette exactitude.

Nous proposons un *dictionnaire des métadonnées* pour vous aider dans cette tâche. Vous y trouverez des tableaux de correspondance définissant les conditions et l'information nécessaire en lien avec le code ONIX correspondant.  

*L'étude française sur l'affichage des informations d'accessibilité* ajoute des ressources utiles pour comprendre comment chaque code devrait se matérialiser sur les sites de diffusion et de distribution.

## Les informations nécessaires

Les exigences de la directive Européenne impliquent que des informations sont disponibles sur les quatre catégories suivantes&nbsp;: 
* les **modes de lecture** (tout le contenu disponible en voix de synthèse et braille, affichage modifiable, synchronisation texte et audio, etc.)&#8239;; 
* les possibilités de **navigation** dans le fichier (table des matières dans le contenu, pagination de référence d’un imprimé, etc.), 
* les **fonctionnalités du livre** (illustrations, tableaux, schémas, math, etc.) et leur accessibilité. 
* les **risques** physiologiques éventuels liés à l'épilepsie ou à l'hypersensibilité.
* le **blocage** éventuel des fonctionnalités d’accessibilité par des mesures de protection inadéquates (DRM) devrait aussi être renseigné.

Chacune de ces catégorie est détaillée dans le <a href="https://www.lina25.fr/ressources/metadonnees">dictionnaire des métadonnées d'accessibilité</a>. 

## Les informations supplémentaires utiles

### Les exemptions

Les exemptions prévues par l'EAA peuvent être renseignées sous la forme de métadonnées. Ces dernières n'ont pas vocation à être affichées mais permettront aux autorités de cibler les contrôles et à l'interprofession d'établir des statistiques sur l'impact de la directive Européenne sur le secteur du livre numérique.

* Si l’éditeur est une micro-entreprise, il doit renseigner le code [196-75&nbsp;: Exception 1 EAA - micro-entreprises](https://ns.editeur.org/onix/fr/196/75).
* Si la mise en conformité du livre numérique génére un surcout disproportionné, l'éditeur doit renseigner le code [196 - 76 &nbsp;: Exception 2 EAA – charge disproportionnée](https://ns.editeur.org/onix/fr/196/76).
* Si la mise en conformité du livre numérique implique une modification fondamentale de l'oeuvre, l'éditeur doit renseigner le code [196 - 77&nbsp;: Exception 3 EAA – modification fondamentale](https://ns.editeur.org/onix/fr/196/77)

### La conformité

La meilleure façon d’assurer que les informations sont juste consiste à pratiquer des tests de contrôle pour s’assurer que le document est conforme à EPUB accessibility AA (<a href="https://ns.editeur.org/onix/en/196/03">liste 196 code 03</a>) ou A (<a href="https://ns.editeur.org/onix/en/196/02">liste 196 code 02</a>). Dans ce dernier cas il faudra aussi assurer que la mise en forme est modifiable (<a href="https://ns.editeur.org/onix/en/175/E200">Liste 175 Code E200&#8239;: Redimensionnable</a>) pour rester dans les conditions acceptables de la directive européenne.

### Addenda et résumé d'accessibilité 

Dans les cas où il vous parait nécessaire d'ajouter une information concernant l'accessibilité du livre, il est possible de rédiger un texte à placer dans l'Addenda sur l’accessibilité (<a href="https://ns.editeur.org/onix/en/196/92">Liste 196 Code 92&#8239;: </a>). Ce peut aussi être une URL vers une page plus détaillée. Cette métadonnée est particulière car c'est un champ libre dans lequel ce que vous écrirez sera transporté et affiché tel quel. Il faut partir du principe que les autres métadonnées d'accessibilité ont déjà été présentées et que cet addenda sert à indiquer des caractéristiques ou des lacunes qui ne sont pas exprimées par les autres métadonnées. 

Cet addenda devrait être le même que celui contenu dans le fichier EPUB sous le code (<span lang="en"><i>schema.org accessibility summary</i></span>) et préciser notamment les déficiences potentielles. Le guide d'usage des métadonnées d’accessibilité du W3C (*Expressing Accessibility Metadata in the EPUB Package Document*) comporte une section explicative sur le sujet. 

Dans le passé, les métadonnées d'accessibilité n'étaient pas affichées par les catalogues en ligne, le résumé d'accessibilité (<a href="https://ns.editeur.org/onix/en/196/00">Liste 196 Code 00&#8239;: </a>) permettait alors de palier à ce manque. Il ne devrait plus être utilisé aujourd'hui.

### Certificats et démarches d'accessibilité

Les informations relatives à la certification d'accessibilité contenues dans les codes 196 01 et 93 sont délivrés par des tiers qui engagent leur responsabilité.

Les codes 196 94 à 99 permettent de renseigner les utilisateurs sur la démarche d'accessibilité de l'éditeur et de leur indiquer qui contacter en cas de difficulté.

</div>

<section  class="ressources" markdown="1">
<h2> Ressources</h2>
<ul>
<li> <a href="https://www.lina25.fr/ressources/metadonnees" class="link color_orange" target="_self">Dictionnaire des métadonnées d'accessibilité</a>
</li>
<li>
<a href="../ressources/Informer" class="link color_orange" target="_self">Étude française sur l'affichage des informations d'accessibilité</a>
</li>
<li>
<a href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/" class="link color_orange" target="_self" lang="en">Accessibility Metadata Display Guide for Digital Publications 2.0 </a>(en anglais)
</li>

<li>
<span lang="en"><a href="https://w3c.github.io/publ-a11y/epub-a11y-meta-guide/1.0/draft/index.html" class="link color_orange">
Expressing Accessibility Metadata in the EPUB Package Document</a></span>
</li>

<li>
<a href="https://ns.editeur.org/onix/fr/196" class="link color_orange">ONIX liste 196</a>
</li>

<!-- <li>
<a href="https://edition-accessible.github.io/signalement/references/references.html" class="link color_orange">Tableau de correspondances schema.org et ONIX en Français</a>
</li> -->

<li>
<a href="https://w3c.github.io/publ-a11y/drafts/a11y-crosswalk-MARC/" class="link color_orange">Tableau de correspondances schema.org, ONIX, MARC21 et UNIMARC en Anglais</a>
</li>

</ul>
</section>

