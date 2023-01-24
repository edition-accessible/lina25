---
layout: document
title: "Dictionnaire des métadonnées d'accessibilité"
date: 2023-01-01
draft: 'true'
previous: ../pages/collecter.html
titlePrev: Collecter
---

Les métadonnées d'accessibilité sont des informations supplémentaires que les éditeurs doivent renseigner lorsqu'ils établissent la fiche d'information de leur ouvrage. 

Elles viennent compléter les informations bibliographiques et commerciales qui peuvent êtres établies dans un fichier excel ou le back office d'un système de gestion des publications et peuvent être complétées et enrichies par des prestataires de services de diffusion ou de distribution.

Cette page a pour objectif de fournir un référentiel compréhensible permettant aux différents acteurs confrontés à cette activité de renseigner des informations fiables et complétes. 

Les informations indiquées ici sont relatives à ONIX. Des tableaux de correspondance permettent de les transposer en UNIMARC et MARC21.
### Modes de lecture

*Les codes ONIX reflétent actuellement mal les modes de lecture. Des demandes d'évolutions ont étées formulées et devraient apparaitre dans les prochaines révisions.*

### Lecture non visuelle

Le contenu nécessaire à la compréhension est-il entièrement restitué aux technologies d’assistance&#8239;?

Moyen de tester&#8239;: la fonction TTS de Thorium Reader permet d'écouter le livre y compris les textes alternatifs et textes masqués. Il est nécessaire de vérifier que ces derniers sont pertinents, notamment dans le cas de consignes liées à l'image.

Moyen de vérifier&#8239;: les balise img ont un argument Alt ou un texte rendant le même service que l'image est disponible dans la légende, le texte environnant, un lien ou un élément HTML `detail`.

ONIX&#8239;: demande d'évolution en cours de discussion.

### L’aspect du texte et la mise en page peuvent-être modifiés selon les possibilitées offertes par le système de lecture

ONIX&#8239;: demande d'évolution en cours de discussion.

<!-- <table class="zebra">
<thead>
<tr class="header">
<th>Condition</th>
<th>Accessibilité</th>
<th>code ONIX</th>
</tr>
</thead>
<tr><td></td>Le livre peut être lu par une voix de synthèse<td></td><td></td></tr>
<tr><td></td><td></td><td></td></tr>
<tr><td></td><td></td><td></td></tr>
<tr><td></td><td></td><td></td></tr>
</table> -->

### Navigation

*Pour être considéré accessible, chaque livre numérique doit comporter au moins deux méthodes de navigation.*

<table class="zebra">
<thead>
<tr class="header">
<th>Condition</th>
<th>Accessibilité</th>
<th>code ONIX</th>
</tr>
</thead>
<tr><td> L'ouvrage existe en imprimé</td>
<td>Dans le livre numérique il est possible d'identifier et de se rendre au début d'une page précise de l'ouvrage imprimé et ce dernier est connu</td>
<td><a href="https://ns.editeur.org/onix/en/196/19) et  <a href="">Liste 51 Code 13 Publication numérique basée sur (édition papier)</a>(https://ns.editeur.org/onix/en/51/13) ">Liste 196 Code 19 Numérotation de pages équivalente au document imprimé</a></td></tr>
<tr><td> Le livre est composé de chapitres, parties ou sections</td>
<td>Le code du livre comporte des niveaux de titre (h1, h2, h3) et leur hierarchie est cohérente</td>
<td><a href="https://ns.editeur.org/onix/en/196/29">Liste 196 Code 29 Navigation suivant/précédent</a></td></tr>
<tr><td> Le livre est composé de chapitres, parties ou sections, il a un sommaire ou une table des matières</td>
<td>Ce sommaire est reproduit dans le contenu affiché, il est possible d'adapter son affichage en modifiant police, taille de scaractères et espacements </td>
<td><a href="https://ns.editeur.org/onix/en/196/11">196 11 Navigation dans la table des matières</a></td></tr>
<tr><td> Le livre contient des index</td>
<td>les entrées des index sont des liens qui permettent d'accéder directement au point de référence indexé.</td>
<td><a href="https://ns.editeur.org/onix/en/196/12">196 12 Navigation dans l’index</a></td></tr>
<tr><td> Le livre contient des encadrés ou des textes en marge </td>
<td>L'ordre de lecture des contenus principaux et secondaires par la voix de synthèse ne crée pas de confusion</td>
<td><a href="https://ns.editeur.org/onix/en/196/13">196 13 Ordre de lecture</a></td>
</tr>
</table>


### Fonctionnalités

*Les fonctionnalités d'accessibilité sont conditionées au fonctionnalitées du contenu de l'oeuvre.*

<table class="zebra">
<thead>
<tr class="header">
<th>Condition</th>
<th>Accessibilité</th>
<th>code ONIX</th>
</tr>
</thead>
<tr><td> Le livre contient des images nécessaires à la compréhension</td>
<td>Des alternatives textuelles courtes sont proposées (argument Alt ou courte légende descriptive) </td>
<td><a href="https://ns.editeur.org/onix/en/196/14">196 14 Brèves descriptions alternatives</a></td></tr>
<tr><td>Le livre contient des images complexes nécessaires à la compréhension</td>
<td>Une alternative longue est proposée. Cette alternative peut être seulement vocalisée ou également disponible visuellement.</td>
<td> <a href="https://ns.editeur.org/onix/en/196/15">196 15 Descriptions alternatives complètes</a></td></tr>
<tr><td>Le livre contient des tableaux en images, des schémas ou des diagrammess</td>
<td>Le livre contient des tableaux en images, des schémas ou des diagrammes qui sont complétés par un accès complet aux données qu’ils représentent</td>
<td><a href="https://ns.editeur.org/onix/en/196/16">196 16 Représentations graphiques de données également accessibles comme données non graphiques</a></td></tr>
<tr><td> Le livre contient des portions dans une langue différente du contenu général</td>
<td> Ces portions sont vocalisées avec la voix et les intonations correspondantes</td>
<td><a href="https://ns.editeur.org/onix/en/196/22">196 22 Balisage de la langue fourni</a></td></tr>
<tr><td>Le livre contient des abréviations, des sigles, une numérotation romaine, ou des onomatopées </td>
<td>Elles sont correctement vocalisées</td>
<td><a href="https://ns.editeur.org/onix/en/196/21">Liste 196 Code 21 Synthèse vocale optimisée</a></td></tr>
<tr><td></td>
<td></td>
<td> <a href="https://ns.editeur.org/onix/en/196/25">196 25 Usage de la couleur</a></td></tr>
<tr><td></td>
<td></td>
<td><a href="https://ns.editeur.org/onix/en/196/26">196 26 Usage du contraste</a></td></tr>
<tr><td></td>
<td></td>
<td> <a href="https://ns.editeur.org/onix/en/196/17) ">196 17 Contenu mathématique accessible</a></td></tr>
<tr><td></td>
<td></td>
<td> <a href="https://ns.editeur.org/onix/en/196/18">196 18 Contenu chimique accessible</a></td>
</tr>
</table>

### Avertissements

Si des risques existent ils doivent être déclarés. Ces informations sont transportées par les codes suivants&#8239;:

-   <a href="https://ns.editeur.org/onix/en/143/13">Liste 143 Code 13&#8239;: Avertissement&#8239;: risque de clignotement</a>
-   <a href="https://ns.editeur.org/onix/en/143/15">Liste 143 Code 15&#8239;: Effets sonores</a>
-   <a href="https://ns.editeur.org/onix/en/143/17">Liste 143 Code 17&#8239;: Avertissement&#8239;: risque de simulation de mouvement</a>

Même si ils n'ont pas vocation à être affichés, les codes déclarant une absence de risque permettent de s'assurer que l'absence de ces trois codes n'est pas due à un manque de vigilance&#8239;:

-   <a href="">Liste 143 Code 14&#8239;: Aucun avertissement nécessaire pour les risques liés à un clignotement</a>(https://ns.editeur.org/onix/en/143/13)
-   <a href="">Liste 143 Code 16&#8239;: Aucun avertissement nécessaire pour les risques liés à un niveau sonore</a>(https://ns.editeur.org/onix/en/143/15)
-   <a href="">Liste 143 Code 18&#8239;: Aucun avertissement nécessaire pour les risques liés à des simulations de mouvement</a>(https://ns.editeur.org/onix/en/143/17)

### Les informations supplémentaires utiles

La meilleure 

Une façon simple d’assurer cette information consiste à s’assurer que le document est conforme à EPUB accessibility AA (<a href="">liste 196 code 03</a>(https://ns.editeur.org/onix/en/196/03)).

Si le document est conforme EPUB accessibility A (<a href="">liste 196 code 02</a>(https://ns.editeur.org/onix/en/196/02)) il devrait aussi assurer que la mise en forme est modifiable (Liste 175 Code E200&#8239;: Redimensionnable).

Si il est présent, le résumé d'accessibilité (<a href="">Liste 196 Code 00&#8239;: Résumé sur l’accessibilité</a>(https://ns.editeur.org/onix/en/196/00)) devrait être transporté. Ce résumé devrait être le même que celui contenu dans le fichier EPUB (schema.org accessibility summary) et préciser notament les déficiences potentielles.

Les informations relatives à la conformité et à la politique d'accessibilité de l'éditeur contenues dans les codes 196 93 à 99 devraient également être transportées si elles sont présentes.

-   <a href="">196 93 Certification de conformité par</a>(https://ns.editeur.org/onix/en/196/93)
-   <a href="">196 94 Page web pour les informations détaillées d’accessibilité</a>(https://ns.editeur.org/onix/en/196/94)
-   <a href="">196 95 Page web d’un intermédiaire approuvé pour les informations détaillées d’accessibilité</a>(https://ns.editeur.org/onix/en/196/95)
-   <a href="">196 96 Page web de l’éditeur pour les informations détaillées d’accessibilité</a>(https://ns.editeur.org/onix/en/196/96)
-   <a href="">196 97 Compatibilité testée</a>(https://ns.editeur.org/onix/en/196/97)
-   <a href="">196 98 Contact intermédiaire approuvé</a>(https://ns.editeur.org/onix/en/196/98)
-   <a href="">196 99 Contact éditeur pour informations complémentaires sur l’accessibilité</a>(https://ns.editeur.org/onix/en/196/99)


<!-- 
## Modes de lecture

### Lecture non visuelle

Intitulé&#8239;: Texte et images disponibles en voix de synthèse et braille

Le contenu nécessaire à la compréhension est-il entièrement restitué aux technologies d’assistance&#8239;?

Moyen de tester&#8239;: la fonction TTS de Thorium Reader permet d'écouter le livre y compris les textes alternatifs et textes masqués. Il est nécessaire de vérifier que ces derniers sont pertinents, notamment dans le cas de consignes liées à l'image.

Moyen de vérifier&#8239;: les balise img ont un argument Alt  

ONIX&#8239;: demande d'évolution en cours de discussion.

### L’aspect du texte et la mise en page peuvent-être modifiés selon les possibilitées offertes par le système de lecture

ONIX&#8239;: demande d'évolution en cours de discussion.
 -->
