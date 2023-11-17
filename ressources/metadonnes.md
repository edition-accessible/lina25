---
layout: document
title: "Dictionnaire des métadonnées d'accessibilité"
date: 16 novembre 2023
previous: ../pages/collecter.html
titlePrev: Renseigner
---

Les métadonnées d'accessibilité sont des informations que les éditeurs doivent renseigner lorsqu'ils établissent la fiche d'information de leur ouvrage. 

Elles viennent compléter les informations bibliographiques et commerciales qui peuvent être établies dans un fichier excel ou le back office d'un système de gestion des publications et peuvent être complétées et enrichies par des prestataires de services de diffusion ou de distribution.

Cette page a pour objectif de fournir un référentiel compréhensible permettant aux différents acteurs confrontés à cette activité de renseigner des informations fiables et complètes. 

Les informations indiquées ici sont relatives à ONIX. Des tableaux de correspondance permettent de les transposer en UNIMARC et MARC21.

### Modes de lecture

*Les codes ONIX concernant les modes de lecture sont apparus depuis la révision 63.*

### Lecture non visuelle

Cas d'usage : lorsque vous activez la fonction lecture audio de votre liseuse, la voix lira une description lorsqu’elle rencontre une image. Vous pourrez ainsi profiter de l’intégralité du livre sans perdre d’information.
<details><summary>En savoir plus sur la lecture non visuelle</summary>
<ul>
<li>Définition : le contenu du livre numérique est intégralement consultable en texte, les autres médias nécessaires à la compréhension sont décrits ou disposent d’une alternative textuelle.</li>
	<li>Exemple :
	<div class="ckeditor-html5-video" style="text-align: center;">
	<video controls="controls" controlslist="nodownload" src="https://raw.githubusercontent.com/edition-accessible/vocabulaire/main/docs/statics/thorium-descr-imgs.m4v" width="480px" aria-describedby="transcriptionThoriumVocal"></video>
	</div><span id="transcriptionThoriumVocal">Transcription : la voix de synthèse lit le titre puis la description de l'image. Un surlignage jaune permet d'identifier que c'est l'image qui est lue.</span></li>
	<li>Précisions : la plupart des publications numériques disponibles incluent leur contenu en texte numérique et peuvent indiquer qu’elles sont adaptées aux lecteurs d’écran. Les exceptions sont les publications dont une partie du contenu essentiel à la compréhension n’est inclus que dans des images, comme des graphiques, des tableaux ou des équations présentés sous forme d’images, et les publications dont l’apparence fixe est créée par une image de chaque page au lieu d’un texte véritable.</li>
</ul>
</details>

<a href="https://ns.editeur.org/onix/fr/196/52">ONIX 196-52 : Tout contenu non décoratif accessible aux utilisateurs privés de la vue</a>

### Modifier l’aspect du texte et la mise en page 

<p>Cas d'usage : lorsque vous lisez, vous souhaitez pouvoir modifier la taille des caractères ainsi que les espacements pour rendre la lecture confortable en fonction de votre matériel ou des conditions.</p>
<details><summary>En savoir plus sur les possibilités de modification de la mise en page</summary>
<ul>
<li>Exemple : <img alt="Dans l'interface de Thorium, l'aspect du livre est modifié : le fond passe en en sépia puis en noir ; la police est grossie puis modifiée, les espacements des lignes sont agrandis." src="https://raw.githubusercontent.com/edition-accessible/vocabulaire/main/docs/statics/thorium_adjust_txt.gif"></li>
<li>Définition : Lors de sa lecture, la mise en forme du fichier est adaptée aux besoins de l’utilisateur (taille adaptée à l’écran, police, taille de la police, espacements, etc.) en fonction des possibilités du logiciel de lecture.</li>	<li>Précisions : cela concerne les livres numériques au format EPUB (quand la mise en page n’est pas fixe), Kindle, Books ou HTML.</li>
</ul>
</details>

<a href="https://ns.editeur.org/onix/fr/196/36"> ONIX 196-36 : Tout le contenu textuel peut être modifié</a>

### Conserver l'aspect du texte et la mise en page 

<p>Cas d'usage : vous souhaitez disposer d’une représentation exacte de la version papier pour l’imprimer ou parce que vous utilisez le livre numérique en complément d’une édition imprimée.</p>
<details><summary>En savoir plus sur la mise en page fixe</summary>
<ul>
<li>Exemple : <a href="https://ressources.sesamath.net/coll_docs/cah/valide/manuel_chapitre_2014_2SP1.pdf">Une page d'un manuel scolaire dont la mise en page structure fortement la lecture.</a><br/><img alt="" src="https://raw.githubusercontent.com/edition-accessible/vocabulaire/main/docs/statics/image6.png" style="width: 319.71px; height: 502.60px; margin-left: 0.00px; margin-top: 0.00px; transform: rotate(0.00rad) translateZ(0px); -webkit-transform: rotate(0.00rad) translateZ(0px);" title=""></li>
<li>Définition : Lors de sa lecture, la mise en forme du fichier n’est pas modifiée quelle que soit la taille de l’écran. L’utilisateur ne peut pas modifier la police ou les espacements.</li>
<li>Précisions : les mises en page fixes sont par nature difficilement accessibles car elles ne permettent pas d'ajuster le texte à sa vision ou à son écran. Il est aussi particulièrement complexe d'assurer leur restitution correcte par une technologie d'assistance comme un lecteur d'écran qui assure la restitution vocale ou braille. Par ailleurs la pagination de référence de l'original peut-être ajoutée dans un format EPUB ou HTML et rendue disponible via un menu spécifique.</li>
</ul>
</details>

<a href="https://ns.editeur.org/onix/fr/175/E201">
ONIX 175 - E201 : Format fixe</a>


### Livres audio accessibles

<p>Cas d'usage : lorsque vous achetez un livre audio vous voulez être sûr que toute l’information est présente sous forme audio, y compris le sommaire, le temps de lecture et d’autres informations qui peuvent être communiquées sur une image de couverture jointe aux fichiers audios.</p>
<details><summary>En savoir plus sur l'accessibilité du livre audio</summary>
<ul>
<li>Exemple : <img alt="Capture d'écran d'un dossier contenant des fichiers MP3 et un fichier couverture.mp3" src="https://raw.githubusercontent.com/edition-accessible/vocabulaire/main/docs/statics/image3.png"></li>
<li>Définition : indication que cette publication peut être lue intégralement en mode audio. Cette désignation s’applique même si le texte est également disponible avec l’audio.</li>
<li>Précisions : les livres audio présentés sans texte sont considérés comme des publications optimisées. Ils ne répondent pas à toutes les exigences en matière d’accessibilité et ne seront donc pas identifiés lors du filtrage des publications “accessibles”, mais ils donnent accès à la publication à des utilisateurs spécifiques qui ont besoin de l’audio. Le fait de permettre aux utilisateurs d’être autonomes pour chercher dans une collection toutes les publications avec le son intégral aidera ces utilisateurs et le fait d’inclure cette information dans les métadonnées affichées alertera également les utilisateurs pour lesquels le son est inaccessible.</li>
</ul>
</details>

<a href="https://ns.editeur.org/onix/fr/196/39">196 - 39 : Accessibilité d’un matériel complémentaire à un livre audio</a>

### Autres modes de lecture

Il existe des livres imprimés qui ne peuvent prétendre à une accessibilité universelle, à moins d'être livrés en différentes versions dans une même édition. Cependant certaines éditions spécialisées peuvent répondre à des besoins spécifiques. 

ONIX permet d'informer sur ces éditions. Si la liste 196 est dédiée à l'accessibilité numérique, la <a href="https://ns.editeur.org/onix/fr/21">liste 21</a> permet d'indiquer un type d'édition particulier. On retiendra en particulier :

<ul>
   <li><a href="https://ns.editeur.org/onix/fr/21/HRE">21:HRE Édition haute lisibilité</a></li>
   <li><a href="https://ns.editeur.org/onix/fr/21/BRL">21:BRL Édition en Braille</a></li>
   <li><a href="https://ns.editeur.org/onix/fr/21/ETR">21:ETR Édition facile à lire</a></li>
   <li><a href="https://ns.editeur.org/onix/fr/21/LTE">21:LTE Édition en grands caractères</a></li>
   <li><a href="https://ns.editeur.org/onix/fr/21/ULP">21:ULP Édition en très gros caractères</a></li>
</ul>

<p>Les libellés peuvent être utilisés tels que proposés par ONIX.</p> 

### Navigation

*La norme WCAG indique : [2.4.5 Accès multiples](https://www.w3.org/Translations/WCAG20-fr/#navigation-mechanisms-mult-loc) : une page Web peut être située par plus d'un moyen dans un ensemble de pages Web [...]. (Niveau AA)*

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
<td><a href="https://ns.editeur.org/onix/en/196/19">Liste 196 Code 19 Numérotation de pages équivalente au document imprimé</a>. <i>En complément <a href="https://ns.editeur.org/onix/en/51/13">Liste 51 Code 13 Publication numérique basée sur (édition papier) permet de renseigner le titre dont est issue la numérotation.</a></i></td></tr>
<tr><td> Le livre est composé de chapitres, parties ou sections</td>
<td>Le code du livre comporte des niveaux de titre (h1, h2, h3) et leur hierarchie est cohérente</td>
<td><a href="https://ns.editeur.org/onix/en/196/29">Liste 196 Code 29 Navigation suivant/précédent</a></td></tr>
<tr><td> Le livre est composé de chapitres, parties ou sections, il a un sommaire ou une table des matières</td>
<td>Ce sommaire est reproduit dans le contenu affiché, il est possible d'adapter son affichage en modifiant police, taille des caractères et espacements </td>
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

*Les fonctionnalités d'accessibilité sont conditionnées au fonctionnalités du contenu de l'œuvre.*

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
<tr><td>La publication  contient des tableaux en images, des schémas ou des diagrammes</td>
<td>Un accès complet aux données qu’ils représentent est possible</td>
<td><a href="https://ns.editeur.org/onix/en/196/16">196 16 Représentations graphiques de données également accessibles comme données non graphiques</a></td></tr>
<tr><td>La publication  contient des portions dans une langue différente du contenu général</td>
<td> Ces portions sont vocalisées avec la voix et les intonations correspondantes</td>
<td><a href="https://ns.editeur.org/onix/en/196/22">196 22 Balisage de la langue fournit</a></td></tr>
<tr><td>La publication  contient des abréviations, des sigles, une numérotation romaine, ou des onomatopées </td>
<td>Elles sont correctement vocalisées</td>
<td><a href="https://ns.editeur.org/onix/en/196/21">Liste 196 Code 21 Synthèse vocale optimisée</a></td></tr>
<tr><td>La publication fait appel à des codes couleurs pour identifier des portions ou des ressources</td>
<td>La couleur n'est pas la seule façon d'identifier ces portions et leur rôle</td>
<td> <a href="https://ns.editeur.org/onix/en/196/25">196 25 Usage de la couleur</a></td></tr>
<tr><td>La publication comporte des textes sur fonds colorés</td>
<td>La lecture reste possible en noir et blanc</td>
<td><a href="https://ns.editeur.org/onix/en/196/26">196 26 Usage du contraste</a></td></tr>
<tr><td>La publication contient des formules mathématiques</td>
<td>Les formules sont lisibles par la voix de synthèse et il est possible de les copier en conservant leur structure (elles sont balisées grâce au langage MathML) </td>
<td> <a href="https://ns.editeur.org/onix/en/196/17) ">196 17 Contenu mathématique accessible</a></td></tr>
<tr><td>La publication contient des formules chimiques</td>
<td>Les formules sont lisibles par la voix de synthèse et il est possible de les copier en conservant leur structure (elles sont balisées grâce au langage ChemML) </td>
<td> <a href="https://ns.editeur.org/onix/en/196/18">196 18 Contenu chimique accessible</a></td>
</tr>
</table>

### Avertissements

Si des risques existent ils doivent être déclarés. Ces informations sont transportées par les codes suivants&#8239;:

-   La publication contient des animations ont des vidéos avec plus de trois flashs successifs : <a href="https://ns.editeur.org/onix/en/143/13">Liste 143 Code 13&#8239;: Avertissement&#8239;: risque de clignotement</a>.
-   La publication contient des effets sonores déclenchés automatiquement qui peuvent surprendre le lecteur : <a href="https://ns.editeur.org/onix/en/143/15">Liste 143 Code 15&#8239;: Effets sonores</a>.
-   La publication contient des animations ou des vidéos qui simulent un mouvement et peuvent destabiliser le lecteur : <a href="https://ns.editeur.org/onix/en/143/17">Liste 143 Code 17&#8239;: Avertissement&#8239;: risque de simulation de mouvement</a>.

Même s'ils n'ont pas vocation à être affichés, les codes déclarant une absence de risque permettent de s'assurer que l'absence de ces trois codes n'est pas due à un manque de vigilance&#8239;:

-   <a href="https://ns.editeur.org/onix/en/143/13">Liste 143 Code 14&#8239;: Aucun avertissement nécessaire pour les risques liés à un clignotement</a>
-   <a href="https://ns.editeur.org/onix/en/143/15">Liste 143 Code 16&#8239;: Aucun avertissement nécessaire pour les risques liés à un niveau sonore</a>
-   <a href="https://ns.editeur.org/onix/en/143/17">Liste 143 Code 18&#8239;: Aucun avertissement nécessaire pour les risques liés à des simulations de mouvement</a>

