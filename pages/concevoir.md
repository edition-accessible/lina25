---
layout: page
title: Concevoir
subtitle: des contenus complets
orientation: fournir des contenus permettant la production de livres numériques accessibles.
audience: auteurs et éditeurs.
previous: ../index.html
next: ./produire.html
---

<div markdown="1" id="principes">
{%- include principes.html -%}

La grande majorité des livres ont ou auront une version numérique, et cette version numérique doit sauf exception être nativement accessible. Dès l’écriture d’un ouvrage, il est donc nécessaire que ses auteurs et éditeurs préparent le matériel qui permettra de produire facilement un livre numérique accessible.

Les objets éditoriaux sont divers, chaque collection peut nécessiter une liste d’attention différente. Nous présentons ici les cas les plus communs pour lesquels les services de fabrication auront besoin d’éléments pour assurer un résultat satisfaisant.

### Alternatives aux images

Les personnes aveugles ne peuvent pas voir les images. Elles lisent des livres numériques à l’aide de technologies d'assistance qui reproduisent le contenu textuel en audio ou en braille. Cela concerne aussi les personnes qui vont utiliser les fonctionnalités de lecture audio (<abbr title="text to speech">TTS</abbr>) de leur lecteur pour lire en pratiquant une autre activité comme du sport, de la cuisine ou de la conduite.

Pour ces cas d’usages il est nécessaire de proposer des alternatives textuelles pour les images porteuses d’information. L’auteur d’un livre est la personne la mieux placée pour écrire ces alternatives et s’assurer qu’elles font sens et s’intègrent parfaitement dans l'œuvre.

Pour vous aider dans les choix éditoriaux relatifs aux alternatives aux images, les membres du <abbr title="Syndicat national de l'édition">SNE</abbr> ont rédigé à l’intention des auteurs et éditeurs des documents d’aide à la décision qui proposent aussi des pistes d’organisation pour assurer que toutes les ressources ont bien étées traitées.

### Données ayant servi à la construction des diagrammes et graphiques

Les diagrammes, graphiques et autre images d’illustration issues de données ne sont pas accessibles. Pour que des alternatives textuelles puissent être rédigées facilement pendant la phase de production numérique, il est nécessaire que les données - éventuellement simplifiées pour mieux s’intégrer à l’expérience de lecture - soient remises aux services de production de l’éditeur en même temps que le manuscrit.

<blockquote><i>Ces données peuvent être délivrées dans un format CSV, Excel ou XML en fonction des capacitées des services de production.</i></blockquote>

### Formes longues des abréviations et des sigles

Les technologies d’assistance, et en particulier les lecteurs d’écran (logiciels capables de transformer du texte en voix synthétique), butent souvent sur les abréviations et les sigles, qui deviennent inintelligibles. Les auteurs sont les mieux placés pour fournir avec leur manuscrit une liste de formes longues des abréviations et sigles contenus dans leur texte, afin que les équipes de production de livres numériques puissent intégrer ces formes longues dans les fichiers générés, sous une forme facile à gérer par les technologies d’assistance.

<blockquote> <i>Ces informations peuvent être fournies sous la forme d’un document annexe de format textuel, ou sous la forme d’un fichier de données (CSV, Excel ou XML). </i></blockquote>

### Autres points d’attention
Selon les contenus de votre livre numérique, vous pourrez avoir à vous assurer de l’accessibilité d’autres aspects de votre œuvre. Pour y répondre au mieux une série de ressources sélectionnée vous permettra de vous imprégner des cas pratiques. 

Voici une liste non exhaustive des situations que vous pouvez rencontrer et auxquelles vous devrez être attentif : 

* Les médias temporels (audio, vidéo) doivent disposer d’une alternative textuelle comme une transcription ou des sous-titres non incrustés. 
* Les médias temporels (audio, vidéo) ne doivent pas se déclencher sans action de l’utilisateur, et l’utilisateur doit toujours avoir la possibilité de les stopper.
* Le langage utilisé doit correspondre aux personnes qui utilisent le support. Adapter au mieux le vocabulaire et les formulations de phrases permet d’éviter la double tâche ou des tâches complexes qui entraineraient une surcharge cognitive.
* Les contenus complexes comme les mathématiques ou les formules chimiques devraient être fournies dans un langage informatique adapté (LaTeX, MathJax ou MathML par exemple) pour permettre leur conversion.
* Si votre ouvrage propose des indications qui reposent sur une discrimination visuelle, une seconde méthode d’identification doit être proposée.
* Les conséquences des actions de l’utilisateur doivent être clairement identifiées (par exemple si cliquer sur un lien déclenche le téléchargement d’un document ou redirige vers un site en ligne).

<blockquote> <i>Vos contenus doivent être perceptibles, utilisables et compréhensibles même lorsqu'ils sont consultés sur un écran petit, n'affichant pas les couleurs ou encore sans écran, via une vocalisation ou un rendu en braille. </i></blockquote>


</div>

<aside markdown="1">

## Ressources

### Guides pratique

<a href="https://www.sne.fr/app/uploads/2022/10/SNE-Normes-et-stanrdards-Textes-alternatifs-image-Document-de-synthese-.._vdef2.pdf" class ="link color_orange">Mise en accessibilité des images dans les EPUBs - synthése des travaux du groupe normes et standard du SNE, octobre 2022 (PDF non balisé, 2 Mo)</a>

<a href="https://www.sne.fr/app/uploads/2022/10/SNE_Atelier_Normes-et-Standards_Accessibilite_Textes-alternatifs_2022.pptx.pdf" class ="link color_orange">Présentation de l’atelier sur la production de textes alternatifs aux images du groupe normes et standard du SNE, octobre 2022 (PDF non balisé, 5.6 Mo)</a>

<a href="https://github.com/benetech/AccessibleImageSampleBook/blob/master/AccessibleImageSampleBookFrench/DIAGRAM_Image-Description-Guidelines_FR.epub?raw=true" class ="link color_orange"><i>Comment décrire les images ?</i> DIAGRAM Center ; NCAM ; Association BrailleNet (EPUB, 7.7 Mo) </a>

<a href="https://diagramcenter.org" class ="link color_orange">Le Diagram Center (en anglais)</a> propose un outil d’exercices en ligne ([Poet training tool, en anglais](https://poet.diagramcenter.org/)), des ressources video et un [guide de bonnes pratiques (en anglais)](http://diagramcenter.org/table-of-contents-2.html).

### Autres ressources


<a href="https://www.accessiblebooksconsortium.org/publishing/fr/" class ="link color_orange">
Le Consortium pour des livres accessibles (ABC)</a> propose une [charte de l’édition accessible](https://www.accessiblebooksconsortium.org/docs/fr/charter.docx)
ainsi qu'un guide [Édition accessible, Pratiques recommandées à l’intention des éditeurs](https://www.accessiblebooksconsortium.org/export/abc/fr/best_practice_guidelines.doc).

<a href="https://inclusivepublishing.org/" class ="link color_orange">inclusive publishing (en anglais)</a> regroupe des ressources utiles.

<a href="https://daisy.org" class ="link color_orange">Le consortium Daisy (en anglais)</a> propose des webinaires   visibles sur la page dédiée [Webinaires Daisy (en anglais)](https://daisy.org/webinar-series/)

</aside>
