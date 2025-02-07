---
layout: document
date:  2025-02-06
title: "Recommandations pour l'affichage des informations d'accessibilité"
previous: ../pages/diffuser.html
titlePrev: Informer
draft: false
---

<div markdown = "1" id="principes">
Le signalement des fonctions d'accessibilité des livres numériques signifie l’information donnée au lecteur avant achat pour lui permettre d’identifier les livres numériques qui lui permettront une lecture dans les meilleures conditions possibles.

*Cette recommandation est établie au niveau international par le W3C et transcrite en français à partir d’un travail interprofessionnel piloté par EDRLab dans le cadre d’une mission confiée par le comité de pilotage interministeriel. Elle a désormais atteint une maturité suffisante mais peut être mise à jour en fonction des avancées du projet et des recommandations internationales.*

<p>L'approche retenue vise à proposer un accès rapide aux informations clés en les affichant à priori, c'est à dire non masquées et clairement identifiées. 
Des informations plus détaillées sont contenues dans un élément masqué et peuvent être consultées sur action de l'utilisateur.</p>
<p>Une attention particulière est portée sur l'évitement de possibles redondances. </p>
<p>Une grille de correspondance, en fin de document, permet d'identifier les métadonnées ONIX qui assurent cette information. Une table de correspondance (crosswalk) est disponible pour assurer l'interopérabilité des principales autres normes de métadonnées (Schema.org, MARC, MARC21 et UNIMARC).</p>

<h2 id="fiche-livre-informations-générales">Fiche livre&#8239;: informations générales</h2>
<h3 id="détails-du-produit">Détails du produit</h3>
<p>
Doivent être affiché à minima les informations suivantes&#8239;: 
</p>

-   Format de fichier (EPUB, PDF, MP3, Audiobook, Etc.)
-   La mesure de protection ou son absence
-   Date de publication
-   Nom de la maison d’édition
-   La langue principale du contenu

<details>
<summary>Pourquoi ces informations sont importantes pour l’accessibilité</summary>

<ul>
<li>
Le format du fichier donne une indication forte sur les possibilités d’accessibilité, un livre audio au format MP3 sera moins structuré qu’un Audiobook par exemple.
</li>
<li>
La mesure de protection peut bloquer les technologies d’assistance comme les lecteurs d’écrans. Par ailleurs de nombreux matériels de lecture spécifiques comme les lecteurs DAISY ou les bloc note braille ne sont pas équipés pour lire des fichiers chiffrés.
</li>
<li>
La date de publication donne une indication sur la date de réalisation des fichiers. Un livre publié avant 2011 sera sans doute un fichier EPUB2, et un livre publié en 2022 aura plus de chance d’être correctement structuré.
</li>
<li>
Le nom de la maison d’édition peut valoriser les efforts faits par celle-ci en termes d’accessibilité.
</li>
<li>
La langue principale du contenu permet au lecteur de s’assurer qu’il pourra lire dans de bonnes conditions en vérifiant qu’il dispose d’une voix de synthèse ou de la table braille correspondante.
</li>
</ul>

</details>
<h3 id="accessibilité">Accessibilité</h3>

* Si aucune des informations n’est fournie, afficher&#8239;: <strong>Aucune information sur l’accessibilité n’est disponible</strong>. Il est conseillé de préciser les informations suivantes : 
  * <em>peut ne pas être entièrement lisible en voix de synthèse et braille</em> ; 
  * <em>les possibilités d'adaptation de l'affichage ne sont pas connue</em> ; 
  * <em>aucune conformité déclarée</em>.
* Si une ou plusieurs des informations ci-dessous sont présentes, elles devraient être regroupées sous un niveau de titre logique. L’intitulé de ce titre devrait être <strong>Accessibilité</strong> ou <strong>Informations d’accessibilité</strong>. Le pictogramme de l’homme de Vitruve pourra être utilisé en complément.

<p>Chaque tableau indique une catégorie d'information qui peuvent être affichées sur une seule ligne ou regroupées sous l'intitulé correspondant. Les intitulés des catégories peuvent être repris ou omis.</p>
<p>Les éléments d'importance forte devraient toujours être affichés et visibles sans action spécifique de l'utilisateur. Les autres éléments peuvent être masqués et disponibles seulement après action de l'utilisateur (élément détail, tooltip, popup ou lien vers une portion plus lointaine de la page web). Certains éléments peuvent ne pas être affichés si une conformité est déclarée.</p>

<details>
<summary>Note sur l'usage des pictogrammes</summary>
<p>Les pictogrammes peuvent être des indicateurs visuels efficaces et peuvent faciliter l'accès à certains publics. Néanmoins plusieurs points d'attention sont à considérer lors de leur usage. La liste suivante relève les principaux, plus d'information sur l'usage des icônes à des fins d'accessibilité peut être trouvé sur les pages de règles supplémentaires aux WCAG du W3C : <a href="https://www.w3.org/WAI/WCAG2/supplemental/patterns/o1p07-icons-used/" lang ="en">Supplemental Guidance to WCAG 2 Cognitive Accessibility Design Pattern: Use Icons that Help the User</a>.</p>

<ul>
<li> Chaque icône ou symbole doit avoir une signification unique et se trouver à côté du contenu auquel il se rapporte.</li>
<li>  Utilisez des icônes ou des symboles clairs et sans ambiguïté, faciles à voir et à agrandir.</li>
<li> Tenez compte des différences culturelles.</li>
<li> Dans le cas où les pictogrammes ne seraient pas utilisés en combinaison avec le texte, une page guide devra indiquer à quelle information correspond chaque pictogramme et le texte alternatif correspondant devra être apposé à chaque occurrence.  </li>
<li> À l'inverse, si le texte est toujours présent avec le pictogramme, celui-ci devra être considérer comme décoratif et comporter un argument alt vide ainsi qu'un argument role decoration.</li>
</ul>

</details>

<h4>Modes de lecture</h4>
<table  class="zebra">
<thead>
<tr class="header">
<th>Texte à afficher</th>
<th>Définition</th>
<th>code ONIX</th>
<th>En cas d’absence</th>
<!--<th>Importance</th>-->
</tr>
</thead>
<tbody>
<tr class="even">
<td>Texte et images disponibles en voix de synthèse et braille</td>
<td>Le contenu nécessaire à la compréhension est entièrement restitué aux technologies d’assistance</td>
<td> <a href="https://ns.editeur.org/onix/fr/196/52">Liste 196 code 52 : Tout contenu non décoratif accessible aux utilisateurs privés de la vue</a>.</td>
<td>Indiquer : <em>Peut ne pas être entièrement lisible en voix de synthèse et braille.</em></td>
<!--<td>forte</td>-->
</tr>
<tr class="odd">
<td>Affichage adaptable</td>
<td>L’aspect du texte et la mise en page peuvent-être modifiés selon les possibilitées offertes par le système de lecture</td>
<td><a href="https://ns.editeur.org/onix/fr/196/36"> Liste 196 code 36 : Tout le contenu textuel peut être modifié</a></td>
<td>Indiquer : <em>Les possibilités d'adaptation de l'affichage ne sont pas connues.</em> Ne rien indiquer en cas de présence de <a href="https://ns.editeur.org/onix/fr/175/E201">Liste 175 Code E201&#8239;: Format fixe.</a></td>
<!--<td>forte</td>-->
</tr>
<tr class="even">
<td>Mise en page fixe</td>
<td>L’aspect du texte et la mise en page ne peuvent pas être modifiées ou de façon limitée.</td>
<td><a href="https://ns.editeur.org/onix/fr/175/E201">Liste 175 Code E201&#8239;: Format fixe.</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="odd">
<td>Texte et audio synchronisés</td>
<td>Le livre contient de l'audio préenregistré pour lequel une version textuelle visible est synchronisée.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/20">Liste 196 Code 20&#8239;: Audio préenregistré synchronisé</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="even">
<td>Texte et audio complémentaires</td>
  <td>La publication comporte des fichiers audio (y compris des vidéos) en plus du texte. Les deux sont nécessaires à la compréhension de l'ouvrage.</td>
  <td><a href="https://ns.editeur.org/onix/fr/81/06">code 06 </a> Video ; <a href="https://ns.editeur.org/onix/fr/81/25">Liste 81 code 25 </a> Animation narrative ; <a href="https://ns.editeur.org/onix/fr/81/26">Liste 81 code 26 </a> Enregistrement vidéo d'une lecture ; <a href="https://ns.editeur.org/onix/fr/81/27">Liste 81 code 27 </a> Performance -visuel ; <a href="https://ns.editeur.org/onix/fr/81/28">Liste 81 code 28 </a> Autre vidéo ; <a href="https://ns.editeur.org/onix/fr/81/29">Liste 81 code 29 </a> Performance partielle -vidéo ; <a href="https://ns.editeur.org/onix/fr/81/30">Liste 81 Code 30 </a> (Contenu vidéo supplémentaire ne fait pas partie du travail principal)
  </td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="odd">
<td>Contenu audio intégral (présentation, index, notes)</td>
<td>La totalité du contenu est disponible en audio (cela inclut toutes les informations comme le sommaire, le résumé, le temps de lecture et d’autres informations qui apparaissent généralement sur une image de couverture).</td>
<td><a href="https://ns.editeur.org/onix/fr/196/28">Liste 196 Code 28&#8239;: Audio-description alternative complète</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
</tbody>
</table>


<h4>Navigation</h4>
<table  class="zebra">
<thead>
<tr class="header">
<th>Texte à afficher</th>
<th>Définition</th>
<th>code ONIX</th>
<th>En cas d’absence</th>
<!--<th>Importance</th>-->
</tr>
</thead>
<tbody>
<tr class="even">
<td>Référence à la pagination du livre imprimé {contenu de 51-13 RelatedProduct}</td>
<td>Le livre peut être utilisé en complément de sa version imprimée, la pagination de référence étant préservée.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/19">Liste 196 Code 19 Numérotation de pages équivalente au document imprimé. <i>Il faudra indiquer ou pointer le livre de référence utilisé pour la pagination</i></a>.</td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="even">
<td>Table des matières adaptable</td>
<td>Un sommaire est présent dans le contenu du livre, ce qui permet de l'utiliser avec un affichage adapté.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/11">Liste 196 Code 11 Navigation dans la table des matières</a></td>
<td>ignorer</td>
<!--<td></td>--></tr>
<tr class="even">
<td>Index fonctionnels</td>
<td>Un ou des index sont présents dans le contenu du livre. Ils sont composés avec des liens hypertextes et permettent d'accéder aux points de référence indexés.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 12 Navigation dans l’index</a></td>
<td>ignorer</td>
<!--<td></td>--></tr>
<tr class="even">
<td>Navigation logique </td>
<td>La voix de synthèse lira les éléments dans un ordre logique déterminé par l'éditeur ou l'auteur.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 13 Ordre de lecture</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td>-->
</tr> 
<tr class="even">
<td>Navigation logique entre les chapitres</td>
<td>La structure du livre sera correctement interprétée par les dispositifs de lecture.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 29 Navigation suivant/précédent</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td>-->
</tr> 
</tbody>
</table>

<h4>Fonctionnalités</h4>

<table class="zebra">
<thead>
<tr class="header">
<th>Texte à afficher</th>
<th>Définition</th>
<th>code ONIX</th>
<th>En cas d’absence</th>
<!--<th>Importance</th>-->
</tr>
</thead>
<tbody>
<tr class="even">
<td>Images décrites par la voix de synthèse (descriptions courtes)</td>
<td><em>Le livre contient des images nécessaires à la compréhension pour lesquelles une alternative courte sera vocalisée (Alt text).</em></td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 14 Brèves descriptions alternatives</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td> -->
</tr>
<tr class="even">
<td>Images décrites (descriptions longues)</td>
<td>Le livre contient des images nécessaires à la compréhension pour lesquelles une alternative longue est proposée. Cette alternative peut être seulement vocalisée ou également disponible visuellement.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 15 Descriptions alternatives complètes</a></td>
<td>ignorer</td>
<!--<td></td>--></tr>
<tr class="odd">
<td>Données accessibles</td>
<td>Le livre contient des tableaux en images, des schémas ou des diagrammes qui sont complétés par un accès complet aux données qu’ils représentent</td>
<td><a href="https://ns.editeur.org/onix/fr/196/16">Liste 196 Code 16 Représentations graphiques de données également accessibles comme données non graphiques</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="even">
<td>Notations mathématiques structurées (MathML)</td>
<td>Le livre contient des formules mathématiques utilisant un langage fonctionnel (MathML)</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 17 Contenu mathématique accessible</a></td>
<td>ignorer</td>
<!--<td>forte</td>--></tr>
<tr class="even">
<td>Notations chimiques structurées (ChemML)</td>
<td>Le livre contient des formules chimiques utilisant un langage fonctionnel (ChemML)</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 18 Contenu chimique accessible</a></td>
<td>ignorer</td>
<!--<td>forte</td>--></tr>
<tr class="even">
<td>Compréhensible en noir et blanc</td>
<td>Le livre utilise des codes couleurs, mais celles-ci ne sont pas le seul moyen de compréhension.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/25">Liste 196 Code 25 Usage de la couleur</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td> -->
</tr>
<tr class="even">
<td>Lisible en noir et blanc</td>
<td>Le livre utilise des contrastes entre du texte et un fond, il restera lisible lors d'un affichage en noir et blanc.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/26">Liste 196 Code 26 Usage du contraste</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td> -->
</tr>
<tr class="even">
<td>Prononciation améliorée pour la voix de synthèse</td>
<td>Le livre contient des abréviations, des sigles, une numérotation romaine, ou des onomatopées qui seront correctement vocalisées.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/21">Liste 196 Code 21 Synthèse vocale optimisée</a></td>
<td>ignorer</td>
<!--<td></td>--></tr>
<tr class="even">
<td>Textes en langue étrangère correctement vocalisés</td>
<td>Le livre contient des portions de texte dans une autre langue que le contenu principal. Ces portions sont identifiées dans le code et seront correctement prononcées si la langue est disponible sur le dispositif de lecture.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/">Liste 196 Code 22 Balisage de la langue fournit</a></td>
<td>ignorer</td>
<!-- <td>Peut ne pas être affiché si la <a href="https://ns.editeur.org/onix/fr/196/02">Spécifications d’accessibilité EPUB 1.0 A (Liste 196 Code 02)</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Spécifications d’accessibilité EPUB 1.0 AA (Liste 196 Code 03)</a> est présente.</td> -->
</tr>

</tbody>
</table>

<h4>Points d'attention</h4>
<table  class="zebra">
<thead>
<tr class="header">
<th>Texte à afficher</th>
<th>Définition</th>
<th>code ONIX</th>
<th>En cas d’absence</th>
<!--<th>Importance</th>-->
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Attention ce livre inclut des Flashs lumineux</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/13/">Liste 143 Code 13&#8239;: Avertissement&#8239;: risque de clignotement</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="odd">
<td>Ce livre ne comporte pas de risques liés à des Flashs lumineux</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/14/">Liste 143 Code 14&#8239;: Aucun avertissement nécessaire pour les risques liés à un clignotement</a></td>
<td>ignorer</td>
<td>Ne devrait pas être affiché</td>
</tr>
<tr class="even">
<td>Attention ce livre inclut des bruitages sonores</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/15/">Liste 143 Code 15&#8239;: risque sonore</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="even">
<td>Ce livre ne comporte pas de risques liés à des bruitages sonores</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/16/">Liste 143 Code 16&#8239;: Aucun avertissement nécessaire pour les risques liés à un niveau sonore</a></td>
<td>ignorer</td>
<td>Ne devrait pas être affiché</td>
</tr>
<tr class="odd">
<td>Attention ce livre inclut des sensations de mouvement</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/17/">Liste 143 Code 17&#8239;: Avertissement&#8239;: risque de simulation de mouvement</a></td>
<td>ignorer</td>
<!--<td>forte</td>-->
</tr>
<tr class="odd">
<td>Ce livre ne comporte pas de risques liés à des sensations de mouvement</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/143/18/">Liste 143 Code 18&#8239;: Aucun avertissement nécessaire pour les risques liés à des simulations de mouvement</a></td>
<td>ignorer</td>
<td>Ne devrait pas être affiché</td>
</tr>
</tbody>
</table>
<!-- <details>
<summary>Notes sur les modes de lecture et fonctions d’accessibilité</summary>
<p>
Ces informations de premier niveau constituent les fonctionnalités cruciales pour l'accès à la lecture. Elles s'adressent aux personnes en situation de handicap mais peuvent aussi rendre service à une grande majorité de lecteurs.
</p>
</details> -->
<section>
<h4 id="conformite">Conformité</h4>

<table class="zebra">

<thead>
<tr class="header">
<th>Texte à afficher</th>
<th>Définition</th>
<th>code ONIX</th>
<th>En cas d’absence</th>
<!--<th>Importance</th>-->
</tr>
</thead>
<tbody>
<tr>
<td>Contenus accessibles conformes aux standards (A ou AA)</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/196/02">Liste 196 Code 02 Spécifications d’accessibilité EPUB 1.0 A</a> ou <a href="https://ns.editeur.org/onix/fr/196/03">Liste 196 Code 03&#8239;: Spécifications d’accessibilité EPUB 1.0 AA</a></td>
<td>Ignorer</td>
<!--<td></td>-->
</tr>
<tr>
<td>Responsable de la conformité</td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/196/90">196 90 Certification de conformité par</a></td>
<td>Ignorer</td>
<td>Ce champ est obligatoire si une conformité est déclarée. Si la conformité est garantie par l'éditeur, ce champ doit être identique à celui indiquant l'éditeur. On parle dans ce cas d'auto-certification.</td>
</tr>
<tr>
<td><a href="responsable-conformite.html">Lien vers la page du responsable de la conformité</a></td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/196/93">196 93 Certification de conformité par (URL).</a></td>
<td>Ignorer</td>
<td>Contient un lien vers une page de l'organisme responsable de la conformité</td>
</tr>
<tr>
<td><a href="infos-accessibilite-ed.html">Politique d’accessibilité de l’éditeur</a></td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/196/96">Liste 196 code 96 Page web de l’éditeur pour les informations détaillées d’accessibilité</a></td>
<td>ignorer</td>
<!--<td></td>-->
</tr>

<tr>
<td><a href="ace-smart-report-fr.html">Rapport de conformité</a></td>
<!--<td></td>-->
<td><a href="https://ns.editeur.org/onix/fr/196/94">196 94 Page web pour les informations détaillées d’accessibilité</a></td>
<td>Ignorer</td>
<td>Contient un lien vers une page détaillant les résultats des tests de conformité pour un titre.</td>
</tr>
<tr>
<td>texte</td>
<td>Le résumé d'accessibilité doit être considéré comme un addendum. C'est un texte écrit par l’éditeur indiquant les limites ou les particularités qui ne sont pas exprimables autrement en ONIX.</td>
<td><a href="https://ns.editeur.org/onix/fr/196/00">Liste 196 Code 00&#8239;: Résumé sur l’accessibilité content=“lorem ipsum …”</a></td>
<td>ignorer</td>
<!--<td></td>-->
</tr>
</tbody>
</table>
</section>

<section>
<h2 id="filtres-de-recherche">Filtres de recherche</h2>
<ul class="facet-multiselect-checkbox">
<li>
<input type="checkbox"><label class="option">Affichage adaptable</label>
</li>
<li>
<input type="checkbox"><label class="option">Texte et images accessibles en voix de synthèse et braille</label>
</li>
<li>
<input type="checkbox"><label class="option">Texte et audio synchronisés</label>
</li>
</ul>
<p>Un pictogramme Homme de Vitruve avec texte alt " accessible" peut-être affecté à tout fichier déclarant <strong>Liste 196 Code 03 Spécifications d’accessibilité EPUB 1.0 AA</strong>&#8239;: <img src="https://www.w3.org/2021/09/UX-Guide-metadata-1.0/principles/media/accessibility.svg" alt="Informations sur l'accessibilité" style="width: 15px">
</p>
</section>

<section>
<h2>Au sujet des livres imprimés</h2>
<p>Les livres imprimés ne peuvent prétendre à une accessibilité universelle, à moins d'être livrés en différentes versions dans une même édition. Cependant certaines éditions spécialisées peuvent répondre à des besoins spécifiques. </p>
<p>ONIX permet d'informer sur ces éditions. Si la liste 196 est dédiée à l'accessibilité numérique, la <a href="https://ns.editeur.org/onix/fr/21">liste 21</a> permet d'indiquer un type d'édition particulier. On retiendra en particulier&#8239;:</p>
<ul>
<li><a href="https://ns.editeur.org/onix/fr/21/HRE">21:HRE Édition haute lisibilité</a></li>
<li><a href="https://ns.editeur.org/onix/fr/21/BRL">21:BRL Édition en Braille</a></li>
<li><a href="https://ns.editeur.org/onix/fr/21/ETR">21:ETR Édition facile à lire</a></li>
<li><a href="https://ns.editeur.org/onix/fr/21/LTE">21:LTE Édition en grands caractères</a></li>
<li><a href="https://ns.editeur.org/onix/fr/21/ULP">21:ULP Édition en très gros caractères</a></li>
</ul>
<p>Les libellés peuvent être utilisés tels que proposés par ONIX.</p>
</section>
</div>