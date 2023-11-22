---
layout: page
title: Concevoir
date: 2023-03-13
subtitle: des contenus complets
orientation: fournir des contenus permettant la production de livres numériques accessibles.
audience: auteurs et éditeurs.
previous: ../index.html
next: ./produire.html
titleNext: Produire
titlePrev: Accueil
---

<div markdown="1" id="principes">
{%- include principes.html -%}

La grande majorité des livres ont ou auront une version numérique, et cette version numérique doit sauf exception être nativement accessible. Dès l’écriture d’un ouvrage, il est donc nécessaire que ses auteurs et éditeurs préparent le matériel qui permettra de produire facilement un livre numérique accessible.

Les objets éditoriaux sont divers, chaque collection peut nécessiter une liste d’attention différente. Nous présentons ici les cas les plus communs pour lesquels les services de fabrication auront besoin d’éléments pour assurer un résultat satisfaisant.

### Alternatives aux images

Les personnes aveugles ne peuvent pas voir les images. Elles lisent des livres numériques à l’aide de technologies d'assistance qui reproduisent le contenu textuel en audio ou en braille. Cela concerne aussi les personnes qui vont utiliser les fonctionnalités de lecture audio (<abbr title="text to speech">TTS</abbr>) de leur lecteur pour lire en pratiquant une autre activité comme du sport, de la cuisine ou de la conduite.

Pour ces cas d’usages il est nécessaire de proposer des alternatives textuelles aux images porteuses d’information. L’auteur d’un livre est la personne la mieux placée pour écrire ces alternatives et s’assurer qu’elles font sens et s’intègrent parfaitement dans l'œuvre.

Pour vous aider dans les choix éditoriaux relatifs aux alternatives aux images, les membres du <abbr title="Syndicat national de l'édition">SNE</abbr> ont rédigé à l’intention des auteurs et éditeurs des documents d’aide à la décision qui proposent aussi des pistes d’organisation pour assurer que toutes les ressources ont bien étées traitées.

Le guide <i>Comment décrire les images</i> produit par le Diagram Center et traduit par l’association Braillenet propose des exemples expliqués de descriptions, d’autres ressources d’auto formation sont disponibles en anglais sur le site du Diagram Center.

### Données ayant servi à la construction des diagrammes et graphiques

Les diagrammes, graphiques et autre images d’illustration issues de données ne sont pas accessibles. Pour que des alternatives textuelles puissent être rédigées facilement pendant la phase de production numérique, il est nécessaire que les données - éventuellement simplifiées pour mieux s’intégrer à l’expérience de lecture - soient remises aux services de production de l’éditeur en même temps que le manuscrit.

<span class="exergue">Ces données peuvent être délivrées dans un format CSV, Excel ou XML en fonction des capacitées des services de production.</span>

### Formes longues des abréviations et des sigles

Les technologies d’assistance, et en particulier les lecteurs d’écran (logiciels capables de transformer du texte en voix synthétique), butent souvent sur les abréviations et les sigles, qui deviennent inintelligibles. Les auteurs sont les mieux placés pour fournir avec leur manuscrit une liste de formes longues des abréviations et sigles contenus dans leur texte, afin que les équipes de production de livres numériques puissent intégrer ces formes longues dans les fichiers générés, sous une forme facile à gérer par les technologies d’assistance.

<span class="exergue">Ces informations peuvent être fournies sous la forme d’un document annexe de format textuel, ou sous la forme d’un fichier de données (CSV, Excel ou XML). </span>

### Autres points d’attention

Selon les contenus de votre livre numérique, vous pourrez avoir à vous assurer de l’accessibilité d’autres aspects de votre œuvre. Pour y répondre au mieux une série de ressources sélectionnée vous permettra de vous imprégner des cas pratiques.

Voici une liste non exhaustive des situations que vous pouvez rencontrer et auxquelles vous devrez être attentif.

-   Les médias temporels (audio, vidéo) doivent disposer d’une alternative textuelle comme une transcription ou des sous-titres non incrustés.
-   Les médias temporels (audio, vidéo) ne doivent pas se déclencher sans action de l’utilisateur, et l’utilisateur doit toujours avoir la possibilité de les stopper.
-   Le langage utilisé doit correspondre aux personnes qui utilisent le support. Adapter au mieux le vocabulaire et les formulations de phrases permet d’éviter la double tâche ou des tâches complexes qui entraîneraient une surcharge cognitive.
-   Les contenus complexes comme les mathématiques ou les formules chimiques devraient être fournis dans un langage informatique adapté (LaTeX, MathJax ou MathML par exemple) pour permettre leur conversion.
-   Si votre ouvrage propose des indications qui reposent sur une discrimination visuelle, une seconde méthode d’identification doit être proposée.
-   Les conséquences des actions de l’utilisateur doivent être clairement identifiées (par exemple si cliquer sur un lien déclenche le téléchargement d’un document ou redirige vers un site en ligne).

<span class="exergue">Vos contenus doivent être perceptibles, utilisables et compréhensibles même lorsqu'ils sont consultés sur un écran petit, n'affichant pas les couleurs ou encore sans écran, via une vocalisation ou un rendu en braille. </span>

</div>

<section  class="ressources" markdown="1">

## Ressources

### Alternatives aux images

<ul>

<li><a href="https://www.sne.fr/app/uploads/2022/10/SNE-Normes-et-stanrdards-Textes-alternatifs-image-Document-de-synthese-.._vdef2.pdf" class ="link color_orange"><cite>Mise en accessibilité des images dans les EPUBs - synthése des travaux du groupe normes et standard du SNE.</cite> octobre 2022 (PDF non balisé, 2 Mo)</a></li>

<li><a href="https://www.sne.fr/app/uploads/2022/10/SNE_Atelier_Normes-et-Standards_Accessibilite_Textes-alternatifs_2022.pptx.pdf" class ="link color_orange">Présentation de l’atelier sur la production de textes alternatifs aux images du groupe normes et standard du SNE, octobre 2022 (PDF non balisé, 5.6 Mo)</a></li>

<li><a href="https://github.com/benetech/AccessibleImageSampleBook/blob/master/AccessibleImageSampleBookFrench/DIAGRAM_Image-Description-Guidelines_FR.epub?raw=true" class ="link color_orange"><cite>Comment décrire les images&#8239;?</cite> DIAGRAM Center&#8239;; NCAM&#8239;; Association BrailleNet (EPUB, 7.7 Mo) </a></li>

<li class="color_orange"><a href="http://diagramcenter.org/" class ="link color_orange" lang="en">Diagram Center <span lang="fr">(en anglais)</span></a></li>

<li class="color_orange"><a href="https://poet.diagramcenter.org/" class ="link color_orange" lang="en">Poet training tool <span lang="fr">(en anglais)</span></a></li>

</ul>

### Compréhension générale

<ul>

<li class="color_orange"><a href="https://www.accessiblebooksconsortium.org/publishing/fr/" class ="link color_orange">
Site web du Consortium pour des livres accessibles (ABC)</a></li>

<li><a href="https://www.accessiblebooksconsortium.org/documents/102554/102064/abc_charter.pdf" class ="link color_orange">Charte de l’édition accessible</a></li>

<li><a href="https://www.accessiblebooksconsortium.org/documents/102554/254117/best_practice_guidelines.doc" class ="link color_orange"><cite>Édition accessible, Pratiques recommandées à l’intention des éditeurs</cite> (fichier .doc).</a></li>

<li><a href="https://www.inclusivepublishinginpractice.org/" class ="link color_orange">L'édition inclusive en pratique</a></li>

<li><a href="https://inclusivepublishing.org/" class ="link color_orange" lang="en">inclusive publishing <span lang="fr">(en anglais)</span></a></li>

<li><a href="https://daisy.org/webinar-series/" class ="link color_orange">Les webinaires du consortium Daisy <span lang="fr">(en anglais)</span></a></li>
</ul>
</section>
