---
layout: document
title: "Guide d'affichage des métadonnées d'accessibilité 2.0 (projet)"
date: 2024-11-09
previous: ../pages/diffuser.html
titlePrev: Renseigner
---

<p>
  <a href="https://www.w3.org/standards/types%23reports"
    >Projet de rapport du groupe communautaire</a
  > 09 novembre 2024
</p>
<p>Traduction française, EDRLab.</p>
<p>Cette version : 
  <a
    href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/"
    >https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/</a
  >
</p>
<p>Dernière version en cours d’écriture : 
   <a href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/"
    >https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/guidelines/</a
  >
</p>
<p>Éditeurs:</p>
* Charles LaPierre (<a href="http://www.benetech.org/">Benetech</a>)
* Gregorio Pellegrino (<a href="https://fondazionelia.org/">Fondazione LIA</a>)
* Gautier Chomel (<a href="https://www.edrlab.org/">EDRLab</a> )
* George Kerscher (<a href="https://daisy.org/">DAISY Consortium</a>)

<p>Retour d'information :  <a href="https://github.com/w3c/publ-a11y/issues/new/choose">new issue</a>.
</p>
<p>
  <a href="https://www.w3.org/policies/%23copyright">Copyright</a> © 2024 les
  contributeurs au Guide de l'expérience utilisateur pour l'affichage des
  métadonnées d'accessibilité 2.0, publié par le
  <a href="https://www.w3.org/groups/cg/publishingcg"
    >Publishing Community Group</a
  > dans le cadre de l'<a
    href="https://www.w3.org/community/about/agreements/cla/"
    >accord de licence des contributeurs communautaires du W3C (CLA)</a
  >. Un
  <a href="https://www.w3.org/community/about/agreements/cla-deed/">résumé</a
  > lisible par une personne est disponible.
</p>
<hr />
<h2 id="h.30j0zll">Résumé</h2>
<p>
  Il est utile de connaître l'accessibilité d'une publication, quelles que
  soient les capacités d'une personne, car des caractéristiques telles que la
  possibilité de procéder à des ajustements visuels améliorent l'expérience de
  lecture pour tout le monde. Ces lignes directrices proposent un cadre commun pour présenter 
  les déclarations de métadonnées sur l'accessibilité des publications de manière
  conviviale, afin d'offrir aux utilisateurs finaux des informations faciles à
  comprendre, quelles que soient leurs connaissances techniques, et cohérentes
  d'une publication à l'autre et d'un catalogue numérique à l'autre.
</p>
<h2 id="h.1fob9te">Statut de ce document</h2>
<p>
  Cette spécification a été publiée par le
  <a href="https://www.w3.org/groups/cg/publishingcg"
    >Publishing Community Group</a
  >. Il ne s'agit pas d'une norme du W3C et elle n'est pas non plus sur la voie
  des normes du W3C. Veuillez noter qu'en vertu de l'<a
    href="https://www.w3.org/community/about/agreements/cla/"
    >accord de licence du contributeur communautaire du W3C (CLA)</a
  >, il existe un droit de retrait limité et que d'autres conditions
  s'appliquent. En savoir plus sur les
  <a href="https://www.w3.org/community/"
    >groupes communautaires et commerciaux du W3C</a
  >.
</p>
<p>
  Les <a href="https://github.com/w3c/publ-a11y/issues/">issues GitHub</a> sont
  privilégiées pour les discussions.
</p>
<h2 id="h.2et92p0">1. Introduction</h2>
<p>
  Lire une publication est une expérience personnelle. Pour la
  plupart des gens, il s'agit d'une routine, et l'on ne se préoccupe
  guère de la manière dont le titre a été obtenu avant d'être lu. Les
  utilisateurs peuvent se rendre dans une librairie ou rechercher le titre à
  acheter en ligne. Il peut aussi avoir été sélectionné par un enseignant dans
  le cadre d'un cours.
</p>
<p>
  Considérons maintenant que cette personne est aveugle et qu'elle a besoin
  d'une technologie d'assistance. L'utilisateur a besoin de cette technologie
  pour l'aider dans le processus d'achat et pour lire la publication. La
  personne peut se poser les questions suivantes : le lecteur d'écran
  fonctionnera-t-il avec ce titre ; y a-t-il des descriptions d'images qui
  seront prononcées pour décrire ces images ; y a-t-il des numéros de page
  accessibles ; l'ordre de lecture est-il correct ? Toutes ces questions
  d'accessibilité, et bien d'autres encore, sont des problèmes potentiels que
  rencontrent les consommateurs lorsqu'ils essaient d'acheter et, en fin de
  compte, de lire une publication numérique.
</p>
<p>
  La bonne nouvelle est que de plus en plus d'éditeurs créent des publications
  qui sont nativement Accessibles (c'est-à-dire accessibles dès la conception,
  et non pas corrigées à postériori) et font valider ou auditer l'accessibilité
  par des organisations tierces.
</p>
<h3>1.1 Terminologie </h3>
Plusieurs termes utilisés dans les présentes lignes directrices doivent être définis pour plus de clarté :
<dl>
<dt>publication numérique</dt>
<dd>Le terme « publication numérique » est utilisé dans le présent document pour désigner les publications produites dans n'importe quel format numérique. Les publications numériques ne se limitent pas aux livres, mais englobent toute œuvre écrite, visuelle ou audio distribuée et lue sous forme numérique.

Parmi les exemples de publications numériques figurent les livres électroniques, les livres audio, les mangas, les bandes dessinées, les revues, les manuels scolaires numériques, les livres d'images et les livres d'images pour enfants accompagnés d'un fichier audio. Les formats utilisés sont notamment EPUB, PDF et Digital Talking Books (DTB).</dd>
<dt>braille dynamique </dt>
<dd> Le terme braille dynamique est utilisé pour désigner le contenu généré en braille à la volée, par opposition aux formats de braille numérique préformatés. Ce rendu dynamique du contenu est parfois appelé braille électronique ou braille rafraîchissable. 

 Le braille dynamique est généralement restitué sur un appareil distinct du système de lecture, doté de picots permettant de présenter le braille sur un écran tactile. Ces appareils, communément appelés afficheurs braille actualisables, peuvent être reliés à un ordinateur personnel, ou il peut s'agir d'un appareil autonome de prise de notes polyvalent doté d'un afficheur braille actualisable. </dd>
<dt> lecture à voix haute </dt>
<dd> Le terme « lecture à voix haute » est utilisé pour désigner un contenu généré à la volée sous forme de discours synthétique, par opposition à une narration préenregistrée. La fonctionnalité de lecture à haute voix est souvent une caractéristique des systèmes de lecture, mais elle peut être fournie par une technologie d'assistance distincte. </dd>
<dt>système de lecture</dt>
<dd>Toutes les publications numériques nécessitent un système de lecture pour présenter la publication à l'utilisateur final. Les systèmes de lecture peuvent être des applications fonctionnant sur un téléphone intelligent ou une tablette. Il existe des systèmes de lecture qui sont des applications fonctionnant sur des ordinateurs personnels. Il existe également des systèmes de lecture intégrés dans des appareils dédiés à une seule fin, la présentation d'une publication. Il existe même des compétences qui fonctionnent sur des haut-parleurs intelligents et qui peuvent être considérées comme des systèmes de lecture.</dd>

<h2 id="h.tyjcwt">2. Vue d'ensemble</h2>
<p>
  Ce document aide ceux qui souhaitent restituer les informations
  d'accessibilité aux utilisateurs à comprendre comment représenter les
  allégations exprimées par les métadonnées d'accessibilité lisibles par machine
  dans une interface utilisateur proposant une expérience utilisateur (UI/UX)
  cohérente. Ce document s'adresse aux responsables de la mise en œuvre, tels
  que les librairies, les détaillants, les distributeurs, etc. Les créateurs de
  contenu tireront profit de la lecture de ces principes et sont encouragés à
  suivre la
  <a href="https://www.w3.org/TR/epub-a11y-11/"
    >section EPUB Accessibility 1.1 Conformance and Discoverability Requirements
    et ses techniques.</a
  >
</p>
<p>NOTE</p>
<p>
  Ce document présente des principes de haut niveau sans entrer dans les
  questions techniques liées aux différentes normes de métadonnées dans
  l'industrie de l'édition.
</p>
<p>
  C'est pourquoi il existe des techniques qui montrent aux développeurs comment
  récupérer les données pour afficher les informations décrites dans le présent
  document.
</p>
<p>Fin de note</p>
<p>
  Les métadonnées trouvées dans une publication numérique ou dans un
  enregistrement externe correspondant peuvent contenir d'importantes
  allégations d'accessibilité qui aident les utilisateurs finaux à trouver et à
  déterminer si la publication peut répondre à leurs besoins spécifiques en
  matière d'accessibilité.
</p>
<p>
  Toutes les métadonnées d'accessibilité sont censées être lisibles par machine
  - à l'exception du résumé sur l'accessibilité - de manière à ce que les
  métadonnées d'accessibilité puissent être extraites et affichées uniformément
  dans différentes publications et localisées dans différentes langues
  d'interface utilisateur.
</p>
<p>
  Un aspect important est que le rôle des métadonnées du résumé d'accessibilité
  a changé dans la dernière version de la spécification d'accessibilité de
  l'EPUB, de sorte qu'une analyse plus approfondie de la section du
  <a href="#accessibility-summary">résumé d'accessibilité</a> est recommandée.
</p>
<p>
  Ce document fournit des conseils sur la manière d'agréger et d'afficher les
  revendications inhérentes aux métadonnées pour les utilisateurs finaux ; il ne
  s'agit pas de lignes directrices strictes, mais de suggestions visant à
  fournir une expérience cohérente aux utilisateurs par le biais de différents
  portails. Il ne s'agit pas de lignes directrices strictes, mais de suggestions
  visant à offrir une expérience cohérente aux utilisateurs de différents
  portails. Les différents responsables de la mise en
  <a href="#implementations">œuvre</a> peuvent choisir d'appliquer ces lignes
  directrices d'une manière légèrement différente.
</p>
<h3 id="h.3dy6vkm">2.1 Allégations et déclarations d'accessibilité</h3>
<p>
  Lors de la présentation des métadonnées d'accessibilité fournies par
  l'éditeur, il est suggéré d'introduire la section en utilisant des termes tels
  que "revendications" ou "déclarations". Ce titre devrait clairement indiquer à
  l'utilisateur final que les informations proviennent directement de l'éditeur
  et représentent les informations sur l'accessibilité que l'éditeur a souhaité
  communiquer.
</p>
<h3 id="h.4d34og8">2.3 Techniques de métadonnées</h3>
<p>
  Pour aider les développeurs à mettre en œuvre ces lignes directrices, des
  notes détaillées sont disponibles pour expliquer comment extraire des
  informations des normes de métadonnées de l'industrie de l'édition.
</p>
<p>
  Au moment de la publication de ce document, les techniques disponibles pour
  les normes de métadonnées sont les suivantes :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html"
      >Métadonnées d'accessibilité de l'EPUB (OPF)</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html"
      >Métadonnées d'accessibilité ONIX</a
    >
  </li>
</ul>
<p>NOTE</p>
<p>
  Les éditeurs mettent à jour leurs enregistrements ONIX lorsque nécessaire.
  Nous nous attendons à ce que des métadonnées d'accessibilité "inconnues"
  soient initialement fournies, mais qu'elles changent au fur et à mesure que de
  nouvelles informations sont disponibles. Pour cette raison, les implémenteurs
  doivent être prêts à mettre à jour les métadonnées d'accessibilité au fur et à
  mesure que de nouveaux flux ONIX sont mis à disposition.
</p>
<p>Fin de note</p>
<h2 id="h.2s8eyo1">3. Informations générales</h2>
<p>
  Pour résoudre le problème de l'affichage des métadonnées d'accessibilité sous
  une forme lisible par une personne, les fournisseurs détermineront la
  déclaration correcte à afficher (à partir du guide de l'utilisateur) en
  analysant les métadonnées et en utilisant le document approprié sur les
  techniques d'affichage.
</p>
<p>
  Les détails du produit fournissent des informations précieuses sur la facilité
  d'utilisation du livre par rapport aux besoins spécifiques de l'utilisateur.
  Les informations suivantes devraient toujours être affichées :
</p>
<ul>
  <li>Format de fichier (EPUB 2 ou 3, PDF, MP3, Audiobook, etc.)</li>
  <li>Mesure de protection ou absence de mesure de protection</li>
  <li>Nom de la maison d'édition</li>
  <li>Langue principale du contenu</li>
</ul>
<h3 id="h.17dp8vu">
  3.1 Pourquoi ces informations sont-elles importantes pour l'accessibilité ?
</h3>
<ul>
  <li>
    Le format de fichier donne une forte indication de l'accessibilité : un
    livre audio au format MP3 sera moins structuré qu'un livre au format W3C
    audiobook  ; un PDF ne permet pas de modifier la typographie, l'EPUB 2 est
    déprécié, un EPUB 3 prend en charge la navigation dans les pages et une
    meilleure sémantique structurelle, etc.
  </li>
  <li>
    La mesure de protection peut bloquer les technologies d'assistance telles
    que les lecteurs d'écran. En outre, de nombreux dispositifs de lecture
    spécifiques tels que les lecteurs DAISY ou les blocs-notes en braille ne
    sont pas équipés pour lire les fichiers cryptés.
  </li>
  <li>
    Le nom de la maison d'édition peut mettre en évidence les efforts qu'elle a
    faits en matière d'accessibilité.
  </li>
  <li>
    La langue principale du contenu permet aux lecteurs d'être sûrs qu'ils
    pourront lire avec leur technologie d'assistance qui utilise la voix
    synthétisée ou la table braille correspondant à la langue.
  </li>
</ul>
<h2 id="h.3rdcrjn">4. Informations clés sur l'accessibilité</h2>
<p>NOTE</p>
<p>
  Lorsque le créateur de contenu ne fournit pas de métadonnées d'accessibilité
  pour une publication, trois éléments d'information clés devraient toujours
  être présents et peuvent être affichés avec une indication que l'information
  est manquante : <a href="#visual-adjustments">Ajustements visuels</a>,
  <a href="#supports-nonvisual-reading"
    >Prise en charge de la lecture non visuelle</a
  > et <a href="#conformance-group">Conformité</a>.
</p>
<p>Fin de note</p>
<p>NOTE</p>
<p>
  Le présent document ne définit pas l'ordre dans lequel les principales
  informations relatives à l'accessibilité doivent être présentées ; chaque
  responsable de la mise en œuvre peut décider de l'ordre dans lequel les
  informations relatives à l'accessibilité sont présentées.
</p>
<p>Fin de note</p>
<h3 id="h.26in1rg">4.1 Ajustements visuels</h3>
<p>
  Cette information clé doit toujours être affichée, même en l'absence de
  métadonnées (voir les exemples où les métadonnées ne sont pas connues).
</p>
<p>
  Indique si les utilisateurs peuvent modifier l'apparence du texte et la mise
  en page en fonction des possibilités offertes par le système de lecture.
</p>
<p>
  Ce champ indique si les ajustements visuels sont possibles, impossibles ou
  inconnus.
</p>
<p>
  Les lecteurs souffrant de déficiences visuelles ou de handicaps cognitifs
  doivent pouvoir modifier la couleur du texte et de son arrière-plan
  (contraste), la famille et la taille des polices utilisées, ainsi que
  l'espacement entre les lettres, les mots, les phrases ou les paragraphes.
</p>
<p>
  Il ne suffit pas de savoir qu'une publication peut s'adapter à la zone
  d'affichage du système de lecture pour savoir qu'il est possible de modifier
  la police, l'espacement et les couleurs, ou que ces modifications
  n'entraîneront pas d'autres problèmes de lisibilité (par exemple, un texte
  coupé par son contenant).
</p>
<h4 id="h.lnxbz9">4.1.1 Exemples</h4>
<p>
  Pour une flexibilité d’utilisation les exemples sont fournis sous forme de
   listes descriptives et compactes.
</p>
<p>
  <a href="#example-descriptive-explanations">EXEMPLE 1</a> : Formulations
  descriptives
</p>
<ul>
  <li>
    L'apparence du texte et la mise en page peuvent être modifiées en fonction
    des options du système de lecture (famille et taille des polices, espaces
    entre les paragraphes, les phrases, les mots et les lettres, ainsi que la
    couleur de l'arrière-plan et du texte).
  </li>
  <li>
    Le texte et la mise en page ne peuvent pas être modifiés. L'expérience de
    lecture est proche d'une version imprimée. Les systèmes de lecture peuvent
    offrir des options de zoom.
  </li>
  <li>La possibilité de modifier l'apparence n'est pas connue.</li>
</ul>
<p>
  <a href="#example-compact-explanations">EXEMPLE 2</a> : Formulations compactes
</p>
<ul>
  <li>L'apparence peut être modifiée.</li>
  <li>L'apparence ne peut pas être modifiée.</li>
  <li>La possibilité de modifier l'apparence n'est pas connue.</li>
</ul>
<h4 id="h.35nkun2">
  4.1.2 Techniques d'affichage pour l'aide aux ajustements visuels
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#visual-adjustments"
      >(document en cours de finalisation, en anglais) EPUB OPF : Adaptations visuelles</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#visual-adjustments"
      >(document en cours de finalisation, en anglais) ONIX : Ajustements visuels</a
    >
  </li>
</ul>
<h3 id="h.1ksv4uv">4.2 Prise en charge de la lecture non visuelle</h3>
<p>
  Cette information clé doit toujours être affichée, même en l'absence de
  métadonnées (voir les exemples où les métadonnées ne sont pas connues).
</p>
<p>
  Indique si tout le contenu nécessaire à la compréhension peut être consultée
  sous forme de texte et est donc entièrement disponible pour les technologies
  d'assistance et les systèmes de lecture utilisant la synthèse vocale ou le
  braille électronique.
</p>
<p>NOTE</p>
<p>
  Les termes "braille électronique" et "braille rafraîchissable" sont utilisés
  de manière interchangeable. Il s'agit d'un appareil à picots qui présente le
  braille sur un écran tactile.
</p>
<p>Fin de note</p>
<p>
  Ce champ indique si la lecture non visuelle est possible, non possible ou
  inconnue.
</p>
<p>
  Les publications numériques dont une partie du contenu essentiel est présenté
  sous une forme non textuelle (comme des graphiques, des tableaux ou des
  équations présentés sous forme d'images, de vidéos, etc.) doivent inclure des
  alternatives textuelles afin de garantir que les utilisateurs qui lisent avec
  d'autres sens que la vue (principalement auditifs et tactiles) ont accès aux
  mêmes informations que les lecteurs visuels. Ces alternatives textuelles
  peuvent inclure des descriptions détaillées, des transcriptions, des
  sous-titres, etc. en fonction de la nature du contenu non visuel.
</p>
<h4 id="h.44sinio">4.2.1 Exemples</h4>
<p>
  Pour une flexibilité d’utilisation les exemples sont fournis sous forme de
   listes descriptives et compactes.
</p>
<p>
  <a href="#example-descriptive-explanations-0">EXEMPLE 3</a> : Formulations
  descriptives
</p>
<ul>
  <li>
    Tous les contenus peuvent être lus en voix de synthèse et en
    braille électronique.
  </li>
  <li>
    Certaines parties du contenu peuvent ne pas être lus en  lecture en
    voix de synthèse et en braille électronique.
  </li>
  <li>
    Tous les contenus ne sont pas lisibles en  lecture en voix de synthèse
    et en braille électronique.
  </li>
</ul>
<p>
  <a href="#example-compact-explanations-0">EXEMPLE 4</a> : Formulations
  compactes
</p>
<ul>
  <li>Lisible en voix de synthèse et en braille.</li>
  <li>
    Peut ne pas être entièrement lisible en voix de synthèse et en braille.
  </li>
  <li>Pas entièrement lisible en lecture en voix de synthèse et en braille.</li>
  <li>On ne sait pas si elle est lisible en voix de synthèse et en braille.</li>
</ul>
<h4 id="h.2jxsxqh">
  4.2.2 Techniques d'affichage pour l'aide à la lecture non visuelle
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#supports-nonvisual-reading"
      >(document en cours de finalisation, en anglais) EPUB OPF : lecture non visuelle</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#supports-nonvisual-reading"
      >(document en cours de finalisation, en anglais) ONIX : lecture non visuelle</a
    >
  </li>
</ul>
<h3 id="h.z337ya">4.3 Conformité</h3>
<p>
  Cette information clé doit toujours être affichée, même en l'absence de
  métadonnées (voir les exemples où les métadonnées ne sont pas connues).
</p>
<p>
  Indique si la publication numérique prétend respecter les normes de conformité
  internationalement reconnues en matière d'accessibilité.
</p>
<p>
  Les métadonnées de conformité utilisent souvent une terminologie que la
  plupart des gens ne comprendront pas, et il convient donc de fournir des
  <a href="#conf-statements">déclarations simples</a> lorsque les niveaux
  d'accessibilité EPUB et WCAG sont identifiés.
</p>
<p>
  Si la publication ne contient pas de déclaration de conformité, le site doit
  indiquer que la publication ne contient pas de déclaration de conformité.
</p>
<p>
  Dans la plupart des cas, les gens voudront en savoir plus sur la conformité et
  la certification de la publication. L'organisme de certification doit être
  identifié avec ses références et placé immédiatement après la déclaration de
  conformité.
</p>
<h4 id="h.3j2qqm3">4.3.1 Déclarations de conformité</h4>
<p>
  La liste suivante explique la signification de chaque déclaration de
  conformité recommandée.
</p>
<dl>
<dt>Cette publication dépasse les normes d'accessibilité reconnues.</dt>
<dd>
  La publication contient une déclaration de conformité à la norme EPUB
  Accessibility et WCAG 2 Level AAA.
</dd>
<dt>Cette publication répond aux normes d'accessibilité reconnues.</dt>
<dd>
  La publication contient une déclaration de conformité aux normes
  d'accessibilité EPUB et WCAG 2 niveau AA.
</dd>
<dt>Cette publication répond aux normes minimales d'accessibilité.</dt>
<dd>
  La publication contient une déclaration de conformité aux normes
  d'accessibilité EPUB et WCAG 2 niveau A.
</dd>
<dt>La publication ne comprend pas de déclaration de conformité.</dt>
<dd>
  Les métadonnées de conformité sont manquantes et la conformité à une norme de
  cette publication est inconnue.
</dd>
<dt>Nom du certificateur</dt>
<dd>
  Identifie l'organisation qui fournit l'examen de certification ou le processus
  de certification.
</dd>
<dt>Références du certificateur</dt>
<dd>
  Si le certificateur a un badge ou un titre, le texte est fourni. S'il existe
  un lien vers son certificat, celui-ci peut être fourni sous forme de lien. Si
  le certificateur possède un logo ou un badge, celui-ci peut être affiché.
  L'affichage du logo ou du badge peut être convenu entre le certificateur et le
  distributeur qui affiche les métadonnées d'accessibilité.
</dd>
</dl>
<h4 id="h.1y810tw">4.3.2 Informations détaillées sur la conformité</h4>
<p>
  Les informations suivantes peuvent être placées dans une section qui présente
  les détails des informations de conformité.
</p>
<dl>
<dt>Déclaration de conformité</dt>
<dd>
  Identifie la spécification d'accessibilité et le niveau de conformité auxquels
  les affirmations de la publication sont faites. Lorsque la publication prétend
  être conforme à plus d'une spécification, des déclarations de conformité
  supplémentaires peuvent être fournies.
</dd>
<dt>Date de certification</dt>
<dd>
  Si la date de l'évaluation par le certificateur est fournie, cela peut être
  intéressant. Elle est normalement associée au certificateur.
</dd>
<dt>Rapport du certificateur</dt>
<dd>Si un lien vers un rapport est fourni, il peut être intéressant.</dd>
</dl>
<h4 id="h.4i7ojhp">4.3.3 Exemples</h4>
<p>
  Trois exemples sont fournis pour la déclaration de conformité, l'un montre une
  déclaration qui affirme respecter les normes d'accessibilité recommandées et
  un deuxième qui affirme respecter le niveau minimum. Le troisième exemple
  montre une publication dont l'accessibilité est inconnue et la dernière montre que l'information sur la conformité est manquante.
</p>
<p>
  Les exemples présentent la déclaration de conformité, le certificateur, les
  références du certificateur et sont suivis par la section des informations
  détaillées sur la conformité.
</p>
<p>
  <a
    href="#example-conformance-statement-that-claims-to-meet-accepted-accessibility-standards-followed-by-detailed-conformance-information"
    >EXEMPLE 5</a
  > : Déclaration de conformité affirmant respecter les normes d'accessibilité
  reconnues, suivie d'informations détaillées sur la conformité.
</p>
<ul>
  <li>Cette publication répond aux normes d'accessibilité reconnues.</li>
  <li>Cette publication est certifiée par le test d'accessibilité de Foo.</li>
  <li>
    Le certificateur porte le titre de "Enterprise Accessibility Rating"
    (évaluation de l'accessibilité des entreprises).
  </li>
  <li>
    Informations détaillées sur la conformité : Cette publication fait état de
    (EPUB Accessibility 1.1 et Web Accessibility Content Guidelines (WCAG) 2.1
    Level AA.) Cette publication a été certifiée le 2021-09-07 par Foo's
    Accessibility Testing avec un certificat de "Enterprise Accessibility
    Rating". Pour plus d'informations, consultez le
    <a href="http://www.example.com/a11y/report/9780000000001"
      >rapport du certificateur.</a
    >
  </li>
</ul>
<p>
  EXEMPLE 6 : Déclaration de conformité affirmant respecter les normes minimales
  d'accessibilité, suivie d'informations détaillées sur la conformité.
</p>
<ul>
  <li>Cette publication répond aux normes minimales d'accessibilité.</li>
  <li>Cette publication est certifiée par le test d'accessibilité de Foo.</li>
  <li>
    Le certificateur porte le titre de "Enterprise Accessibility Rating"
    (évaluation de l'accessibilité des entreprises).
  </li>
  <li>
    Informations détaillées sur la conformité : Cette publication fait état de
    l'accessibilité EPUB 1.1 et des directives d'accessibilité au contenu Web
    (WCAG) 2.1 niveau A. La publication a été certifiée le 2021-09-07 par Foo's
    Accessibility Testing avec la mention "Enterprise Accessibility Rating".
    Pour plus d'informations, voir le
    <a href="http://www.example.com/a11y/report/9780000000001"
      >rapport du certificateur.</a
    >
  </li>
</ul>
<p>
  EXEMPLE 7 : Déclaration
  de conformité inconnue
</p>
<ul>
  <li>La publication ne comprend pas de déclaration de conformité.</li>
  <li>
    Informations détaillées sur la conformité : Les métadonnées de conformité
    n'ont pas été trouvées.
  </li>
</ul>
<h4 id="h.2xcytpi">4.3.4 Techniques d'affichage pour l'aide à la conformité</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#conformance-group"
      >(document en cours de finalisation, en anglais) EPUB OPF : Conformité</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#conformance-group"
      >(document en cours de finalisation, en anglais) ONIX : Conformité</a
    >
  </li>
</ul>
<h3 id="h.1ci93xb">4.4 Audio préenregistré</h3>
<p>Ces informations doivent être cachées si les métadonnées sont absentes.</p>
<p>
  Indique la présence d'un audio préenregistré et précise si cet audio est
  autonome (livre audio), s'il accompagne le texte (clips audio et vidéo
  intégrés) ou s'il représente une alternative au texte (lecture synchronisée
  texte-audio).
</p>
<p>
  Les livres audio créés pour un usage courant offrent un accès important à de
  nombreux utilisateurs handicapés, même s'ils ne sont pas accessibles à tous.
  Au fur et à mesure qu'ils gagnent en popularité, les livres audio pourraient
  offrir davantage d'options d'accessibilité à l'avenir.
</p>
<p>
  Certaines publications fournissent des fichiers audio (y compris des fichiers
  audio dans des vidéos) en plus du texte. Dans ce cas, il est important que
  l'utilisateur soit informé qu'il ne pourra peut-être pas accéder à tout le
  contenu du livre sous forme textuelle.
</p>
<p>
  Certaines publications proposent des fichiers audio préenregistrés avec
  synchronisation du texte. Les utilisateurs malentendants peuvent ainsi accéder
  à l'intégralité du contenu de ces livres.
</p>
<h4 id="h.3whwml4">4.4.1 Exemples</h4>
<p>
  Pour une flexibilité d’utilisation les exemples sont fournis sous forme de
   listes descriptives et compactes.
</p>
<p>
  <a href="#example-descriptive-explanations-1">EXEMPLE 8</a> : Formulations
  descriptives
</p>
<ul>
  <li>Livre audio sans alternative textuelle.</li>
  <li>Les contenus sont disponibles en version audio et en version texte.</li>
  <li>
    Tous les contenus sont disponibles sous forme de fichiers audio
    préenregistrés synchronisés avec le texte.
  </li>
</ul>
<p>
  <a href="#example-compact-explanations-1">EXEMPLE 9</a> : Formulations
  compactes
</p>
<ul>
  <li>Audio uniquement.</li>
  <li>Audio et texte complémentaire.</li>
  <li>Synchronisation de l'audio et du texte.</li>
</ul>
<h4 id="h.2bn6wsx">
  4.4.2 Techniques d'affichage pour le support audio préenregistré
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#pre-recorded-audio"
      >(document en cours de finalisation, en anglais) EPUB OPF  : Audio complet</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#pre-recorded-audio"
      >(document en cours de finalisation, en anglais) ONIX : audio complet</a
    >
  </li>
</ul>
<h3 id="h.qsh70q">4.5 Navigation</h3>
<p>
  Ces informations essentielles peuvent être masquées si les métadonnées sont
  absentes. Il est également possible d'indiquer qu'aucune information sur la navigation n'est disponible. 

</p>
<p>Identifie les fonctions de navigation incluses dans la publication.</p>
<p>
  Il est important de proposer différentes façons de naviguer dans les
  publications numériques (table des matières, index, etc.) pour permettre à
  l'utilisateur d'accéder facilement à chaque partie du contenu. Ces fonctions
  sont à la fois essentielles pour l'accessibilité et très importantes pour tous
  les utilisateurs qui lisent les publications. Par conséquent, il est important
  de communiquer clairement à l'utilisateur les fonctions de navigation
  disponibles dans la publication afin qu'il puisse les sélectionner
  correctement.
</p>
<p>
  Notez que la norme WCAG (Web Content Accessibility Guidelines) 2.1 exige qu'il
  y ait plus d'une façon de localiser une page dans un ensemble de pages (<a
    href="https://www.w3.org/TR/WCAG21/%23multiple-ways"
    >critère de réussite 2.4.5 Multiple Ways</a
  >).
</p>
<h4 id="h.3as4poj">4.5.1 Exemples</h4>
<p>
  Les exemples sont fournis à titre Formulations compactes descriptives et
  compactes pour une plus grande souplesse d'adoption.
</p>
<p>
  <a href="#example-descriptive-explanations-2">EXEMPLE 10</a> : Formulations
  descriptives
</p>
<ul>
  <li>
    La présence d'une table des matières facilite l'accès direct à chaque
    chapitre via des liens.
  </li>
  <li>
  Inclut des éléments de structure pour les titres et des tableaux pour aider les utilisateurs de technologies d'assistance à naviguer facilement.
  </li>
  <li>L'index fournit des liens vers les références des articles.</li>
  <li>
    Des repères permettent d'accéder rapidement aux principales parties du
    livre.
  </li>
  <li>
    Une liste de pages permet aux utilisateurs de naviguer directement vers les
    pages de la version imprimée identifiée.
  </li>
</ul>
<p>
  <a href="#example-compact-explanation">EXEMPLE 11</a> : Explication compacte
</p>
<p>Navigation par table des matières, index, repères et liste de pages.</p>
<h4 id="h.1pxezwc">4.5.2 Techniques d'affichage pour l'aide à la navigation</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#navigation"
      >(document en cours de finalisation, en anglais) EPUB OPF : Navigation</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#navigation"
      >(document en cours de finalisation, en anglais) ONIX : Navigation</a
    >
  </li>
</ul>
<h3 id="h.49x2ik5">4.6 Graphiques, diagrammes et formules</h3>
<p>
  Ces informations essentielles peuvent être masquées si les métadonnées sont
  absentes. 
  Il est également possible d'affirmer que l'accessibilité des formules, des graphiques, des mathématiques et des diagrammes qui n'ont pas été identifiés comme étant accessibles. 
</p>
<p>
  Indique la présence de formules (y compris mathématiques, chimiques, etc.), de
  graphiques, de tableaux ou de diagrammes,et si ceux-ci sont disponibles dans
  un format accessible ou sous une forme alternative (par exemple, si les
  formules sont navigables avec des technologies d'assistance, ou si des
  descriptions étendues sont disponibles pour les images complexes).
</p>
<p>
  Ce groupe ne doit être affiché que si les métadonnées indiquent la présence de
  formules ou de tableaux et graphiques, sinon il peut être masqué.
</p>
<h4 id="h.2p2csry">4.6.1 Exemples</h4>
<p>
  Pour une flexibilité d’utilisation les exemples sont fournis sous forme de
   listes descriptives et compactes.
</p>
<p>
  <a href="#example-descriptive-explanations-3">EXEMPLE 12</a> : Formulations
  descriptives
</p>
<ul>
  <li>
    Contient des formules mathématiques, physiques ou chimiques sous une forme
    accessible. Des graphiques et des diagrammes sont présents et décrits par
    des descriptions détaillées.
  </li>
  <li>
    Contient des formules mathématiques, physiques ou chimiques, des graphiques
    et des diagrammes sans aucune information sur l'accessibilité de ce contenu.
  </li>
</ul>
<p>
  <a href="#example-compact-explanations-2">EXEMPLE 13</a> : Formulations
  compactes
</p>
<ul>
  <li>
    Formules accessibles. Graphiques et diagrammes accompagnés de descriptions
    détaillées.
  </li>
  <li>
    L'accessibilité des formules, des graphiques et des diagrammes est inconnue.
  </li>
</ul>
<h4 id="h.147n2zr">
  4.6.2 Techniques d'affichage des graphiques, diagrammes et formules
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#charts-diagrams-and-formulas"
      >(document en cours de finalisation, en anglais) EPUB OPF : Graphiques et formules</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#charts-diagrams-and-formulas"
      >(document en cours de finalisation, en anglais) ONIX : Graphiques et formules</a
    >
  </li>
</ul>
<h3 id="h.3o7alnk">4.7 Risques</h3>
<p>
  Ces informations essentielles peuvent être masquées si les métadonnées sont
  absentes. Il est également possible d'indiquer qu'aucune information sur les risques possibles n'est disponible. 

</p>
<p>
  Identifie tout risque (par exemple, éléments clignotants, sons de fond ou
  simulation de mouvement) susceptible d'affecter les utilisateurs sensibles sur
  le plan physiologique.
</p>
<p>
  Contrairement à d'autres propriétés d'accessibilité, la présence de dangers
  peut être exprimée de manière positive ou négative. En effet, les utilisateurs
  recherchent des contenus qui ne présentent pas de risques pour eux et veulent
  savoir si un contenu est potentiellement dangereux pour eux.
</p>
<p>
  Le vocabulaire des propriétés de risques comprend une valeur inconnue, ce qui
  signifie que le créateur du contenu des métadonnées reconnaît explicitement
  que la ressource n'a pas fait l'objet d'une vérification des risques. Cela
  diffère de l'absence de métadonnées pour cette propriété, qui n'a aucune
  signification.
</p>
<h4 id="h.23ckvvd">4.7.1 Exemples</h4>
<p>
  Pour une flexibilité d’utilisation les exemples sont fournis sous forme de
   listes descriptives et compactes.
</p>
<p>
  <a href="#example-descriptive-explanations-4">EXEMPLE 14</a> : Formulations
  descriptives
</p>
<ul>
  <li>La publication ne présente aucun risque.</li>
  <li>
    La publication contient des flashs lumineux, des sons ou des stimuli visuels
    qui changent rapidement, ainsi que des simulations de mouvements, qui
    peuvent causer de l'inconfort, de la distraction, des crises de
    photosensibilité ou le mal des transports.
  </li>
  <li>Aucune information sur les risques éventuels.</li>
</ul>
<p>
  <a href="#example-compact-explanations-3">EXEMPLE 15</a> : Formulations
  compactes
</p>
<ul>
  <li>Aucun risque.</li>
  <li>
    Risques liés aux clignotements, aux sons et à la simulation de mouvements.
  </li>
  <li>Aucune information sur les risques.</li>
</ul>
<h4 id="h.ihv636">
  4.7.2 Techniques d'affichage pour la notification des dangers
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#hazards"
      >(document en cours de finalisation, en anglais) EPUB OPF : Risques</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#hazards"
      >(document en cours de finalisation, en anglais) ONIX : Risques</a
    >
  </li>
</ul>
<h3 id="h.32hioqz">4.8 Résumé de l'accessibilité</h3>
<p>
  Ces informations essentielles peuvent être masquées si les métadonnées sont
  absentes. 
   Il est également possible d'indiquer qu'aucun résumé sur l'accessibilité n'est disponible. 
</p>
<p>
  Le résumé de l'accessibilité était destiné (dans EPUB Accessibility 1.0) à
  décrire en prose lisible par une personne les caractéristiques d'accessibilité
  présentes dans la publication ainsi que les lacunes éventuelles. À partir de
  la version 1.1 d'EPUB Accessibility, le résumé d'accessibilité est devenu un
  résumé lisible par une personne de l'accessibilité qui complète, sans les
  dupliquer, les autres métadonnées de découvrabilité.
</p>
<p>
  Il s'agit d'un champ libre qui permet aux auteurs d'ajouter des informations
  supplémentaires aux propriétés accessibles de la ressource.
</p>
<p>
  En raison de sa nature, aucun traitement spécifique du contenu n'est
  nécessaire ; il suffit d'extraire le texte des métadonnées et de l'afficher
  pour les utilisateurs finaux.
</p>
<h4 id="h.1hmsyys">4.8.1 Exemples</h4>
<p>
  <a href="#example-an-example-accessibility-summary">EXEMPLE 16</a> : Un
  exemple de résumé d'accessibilité
</p>
<p>
  Des experts en la matière ont été chargés de créer le texte alternatif. Les
  tableaux sont représentés sous forme d'images et le texte intégral du tableau
  est fourni sous l'image dans l'élément de détail, qui peut être développé.
  Plusieurs courtes vidéos en langue des signes expliquent les concepts clés.
</p>
<h4 id="h.41mghml">4.8.2 Techniques d'affichage du résumé d'accessibilité</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#accessibility-summary"
      >(document en cours de finalisation, en anglais)  EPUB OPF  : Résumé de l'accessibilité</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#accessibility-summary"
      >(document en cours de finalisation, en anglais) ONIX : Résumé de l'accessibilité</a
    >
  </li>
</ul>
<h3 id="h.2grqrue">4.9 Considérations juridiques</h3>
<p>
  <a href="https://github.com/w3c/publ-a11y/issues/350">QUESTION 350</a> :
  Retour d'information sur les exceptions et exemptions des éditeurs
</p>
<p>
  Nous recherchons activement des commentaires sur cette section "considérations
  juridiques". Si vous êtes éditeur, nous avons besoin de vos commentaires !
</p>
<p>
  Cette information clé doit être cachée si les métadonnées ne sont pas
  présentes.
</p>
<p>NOTE</p>
<p>
  Clause de non-responsabilité : rien ici ne peut être interprété comme un
  conseil juridique fourni par le W3C ou tout autre groupe ou individu ayant
  contribué à ce document. Demandez toujours un avis juridique à votre service
  interne ou à votre conseiller juridique afin d'évaluer la conformité juridique
  et les risques.
</p>
<p>Fin de note.</p>
<p>
  Dans certaines juridictions, les éditeurs peuvent se prévaloir d'une
  dérogation à l'obligation de fournir des publications accessibles, y compris
  des métadonnées d'accessibilité. Cette question doit toujours faire l'objet
  d'une clarification par le conseiller juridique de chaque juridiction. Au
  moment de la rédaction de ce document, la loi européenne sur l'accessibilité
  (European Accessibility Act, EAA) mentionne le cas des micro-entreprises, soit
  celles employant moins de 10 personnes et ayant un chiffre d'affaires annuel
  ou un total de bilan inférieur à 2 millions d'euros.
</p>
<p>
  D'autres aspects juridiques dans l'EAA peuvent concerner les exceptions pour
  les versions individuelles d'un titre, où le fait de rendre le titre
  accessible pourrait entraîner une altération fondamentale du contenu ou
  imposer une charge disproportionnée à l'éditeur, et dans ce cas la juridiction
  n'exigera pas son accessibilité (ce qui peut varier d'une juridiction à
  l'autre).
</p>
<p>
  Les éditeurs peuvent avoir besoin d'inclure des informations sur une exemption
  ou une exception dans les métadonnées pour des raisons juridiques ou de
  clarté, soit pour les organismes qui appliquent la législation, soit pour
  d'autres communications entre entreprises. Toutefois, il ne s'agit pas
  d'informations qui doivent être affichées sur des sites publics, car elles ne
  signifient rien pour la plupart des consommateurs et pourraient entraîner des
  malentendus. Néanmoins, l'objectif est de fournir autant d'informations que
  possible sur l'accessibilité.
</p>

<h4 id="h.3fwokq0">
  4.9.1 Exemple
</h4>
<p>
 *Dans de nombreux cas, aucune information relative à une exception ou à une exemption légale ne sera présentée. L'exemple suivant est fourni à titre d'explication descriptive possible lorsque des informations relatives à une exception légale ou à une exemption doivent être présentées.* 

 Cette publication fait l'objet d'une dérogation en matière d'accessibilité dans certaines juridictions. 
</p>

<h4 id="h.3fwokq0">
  4.9.2 Techniques d'affichage pour les considérations juridiques
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#legal-considerations"
      >(document en cours de finalisation, en anglais) EPUB OPF : considérations juridiques</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#legal-considerations"
      >(document en cours de finalisation, en anglais) ONIX : considérations juridiques</a
    >
  </li>
</ul>
<h3 id="h.1v1yuxt">4.10 Informations supplémentaires sur l'accessibilité</h3>
<p>
  Ces informations essentielles peuvent être masquées si les métadonnées sont
  absentes.
</p>
<p>
  Cette section énumère des catégories de métadonnées supplémentaires qui
  peuvent aider les utilisateurs à mieux comprendre les caractéristiques
  d'accessibilité des publications numériques. Il s'agit de métadonnées qui
  n'entrent pas dans les autres catégories ou qui sont rarement utilisées dans
  l'édition commerciale.
</p>
<p>
  Les informations complémentaires sur l'accessibilité comprennent un large
  éventail d'informations liées au contenu de la publication. Par conséquent,
  les caractéristiques sont regroupées afin que la présentation soit plus
  compréhensible pour les utilisateurs finaux.
</p>
<p>Structure</p>
<p>
  Pour des informations sur les éléments structurels qui facilitent
  l'utilisation d'une ressource (par exemple, ARIA).
</p>
<p>Sauts de page</p>
<p>
  L'inclusion de marqueurs de saut de page provenant d'une source imprimée
  permet aux utilisateurs d'identifier où ils se trouvent dans une publication
  numérique par rapport à son équivalent imprimé.
</p>
<p>Adaptation</p>
<p>
  Pour des informations sur les dispositions du contenu qui permettent la
  lecture dans des modes d'accès alternatifs (par exemple, sous-titres codés,
  annotations en rubis, langue des signes, transcription).
</p>
<p>Clarté</p>
<p>
  Pour des informations sur la façon dont le contenu a été amélioré pour une
  meilleure clarté auditive ou visuelle (par exemple, utilisation de contraste
  élevé).
</p>
<p>Tactile</p>
<p>
  Pour des informations sur le contenu disponible sous forme tactile (par
  exemple, graphique tactile, objets tactiles).
</p>
<p>Contenu</p>
<p>
  Pour des informations sur des types spécifiques de contenu présents dans la
  publication numérique (par exemple, texte sur visuel, musique sur visuel).
</p>
<p>Autres</p>
<p>
  Pour les informations qui n'entrent pas dans l'une des catégories précédentes
  (par exemple, le contrôle de la synchronisation ou la dépendance à l'égard de
  la couleur).
</p>
<h4 id="h.4f1mdlm">4.10.1 Exemples</h4>
<p>
  De nombreuses caractéristiques peuvent être présentes. Certaines d'entre elles
  sont énumérées dans les exemples. Une liste complète peut être trouvée dans
  les techniques.
</p>
<p>
  <a href="#example-descriptive-explanations-5">EXEMPLE 17</a> : Formulations
  descriptives
</p>
<ul>
  <li>
    Le contenu est enrichi de rôles ARIA afin d'optimiser l'organisation et de
    faciliter la navigation.
  </li>
  <li>Les sauts de page sont repris de la source imprimée originale.</li>
  <li>Les vidéos incluses dans les publications sont sous-titrées.</li>
  <li>
    Des graphiques tactiles ont été intégrés pour faciliter l'accès des aveugles
    aux éléments visuels.
  </li>
  <li>Les partitions musicales fournies sont accessibles visuellement.</li>
  <li>
    Le contenu contient des informations codées par des couleurs, qui peuvent
    être imperceptibles pour les personnes qui ne distinguent pas les couleurs.
  </li>
</ul>
<p>
  <a href="#example-compact-explanations-4">EXEMPLE 18</a> : Formulations
  compactes
</p>
<ul>
  <li>Rôles ARIA.</li>
  <li>Pagination de l’imprimé</li>
  <li>Sous-titres codés pour les vidéos.</li>
  <li>Graphiques tactiles joints.</li>
  <li>Les partitions musicales sont présentées de manière visuelle.</li>
  <li>Information codée par les couleurs.</li>
</ul>
<h4 id="h.2u6wntf">
  4.10.2 Techniques d'affichage d'informations supplémentaires sur
  l'accessibilité
</h4>
<p>
  Les techniques spécifiques permettant de respecter ce principe sont définies
  dans les documents suivants :
</p>
<ul>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/epub-metadata/index.html#additional-accessibility-information"
      >(document en cours de finalisation, en anglais) EPUB OPF : Caractéristiques du livre</a
    >
  </li>
  <li>
    <a
      href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/techniques/onix-metadata/index.html#additional-accessibility-information"
      >(document en cours de finalisation, en anglais) ONIX : Caractéristiques du livre</a
    >
  </li>
</ul>
<h2 id="h.19c6y18">5. Découvrir des contenus accessibles</h2>
<p>
  Les lignes directrices relatives à la présentation des métadonnées
  d'accessibilité détaillées dans le présent document visent à améliorer
  l'expérience de l'utilisateur lorsque les lecteurs parcourent l'entrée du
  catalogue d'une publication. Toutefois, les métadonnées d'accessibilité ont
  également un rôle essentiel à jouer pour aider les lecteurs à découvrir les
  publications qui leur sont accessibles.
</p>
<p>
  Les fournisseurs de publications, tels que les librairies et les
  bibliothèques, créent des outils de recherche et de filtrage qui interprètent
  les métadonnées d'accessibilité pour faciliter la découverte. L'ensemble et la
  variété des filtres dépendent du public auquel ils s'adressent et du type de
  livre qu'ils proposent.
</p>
<p>
  Les commentaires des utilisateurs indiquent qu'en l'absence de filtres
  d'accessibilité spécifiques, ils considèrent que les détails du produit tels
  que le format du fichier et les mesures de protection (par exemple, la gestion
  des droits numériques) sont des informations cruciales pour déterminer la
  facilité d'utilisation.
</p>
<p>
  Compte tenu de ces réalités, les sections suivantes proposent un ensemble
  minimal et un ensemble étendu d'options de filtrage. La plupart des
  informations spécifiques peuvent être ajoutées si elles sont jugées utiles
  pour le public de la plateforme.
</p>
<h3 id="h.3tbugp1">5.1 Ensemble minimal de filtrage</h3>
<p>
  Les systèmes de lecture, le commerce et les plateformes de distribution
  disposent généralement d'options de filtrage spécifiques ; l'uniformisation
  des aspects clés et la fourniture de conseils pour une approche standardisée
  peuvent faciliter le processus de découverte pour les utilisateurs à la
  recherche de titres pertinents. Toutefois, cela ne doit pas empêcher les
  utilisateurs ayant des besoins de lecture spécifiques de trouver les livres
  qu'ils recherchent. Pour atteindre cet objectif, il est recommandé que toutes
  les plateformes présentent deux capacités minimales, centrées sur les modes de
  consommation du contenu. Il s'agit de :
</p>
<ol>
  <li>Titres favorisant la lecture non visuelle</li>
  <li>Titres qui prennent en charge les ajustements visuels</li>
</ol>
<p>
  Il convient de noter que seules les valeurs positives doivent être utilisées.
</p>
<p>
  <a href="#example-minimum-filtering-options">EXEMPLE 19</a> : Options de
  filtrage minimum
</p>
<ul>
  <li>Lisible en voix de synthèse et braille</li>
  <li>L'affichage peut être modifié</li>
</ul>
<h3 id="h.28h4qwu">5.2 Ensemble de filtrage étendu</h3>
<p>
  Dans certains domaines, l'ajout d'autres options deviendra important pour
  aider les utilisateurs à trouver un contenu qui réponde à un besoin ou à des
  scénarios particuliers. Chaque domaine déterminera de manière unique la
  sélection des éléments appropriés. Voici quelques exemples de ces domaines
  (non exclusifs) :
</p>
<ul>
  <li>
    Dans un contexte académique, la présence de numéros de page imprimés peut
    être cruciale pour s'assurer que le lecteur sera en mesure de trouver ou de
    faire une référence.
  </li>
  <li>
    Dans un contexte technique ou scientifique, les informations sur les moyens
    d'accès à des contenus complexes tels que les graphiques, les diagrammes et
    les formules seraient d'une grande importance pour savoir si les balises
    d'accessibilité sont présentes.
  </li>
  <li>
    Sur les marchés où la conformité à la législation est exigée, l'information
    sur la conformité devient obligatoire.
  </li>
  <li>
    Les plateformes dédiées à la vente de livres pour enfants et de contenus
    interactifs pourraient vouloir permettre aux utilisateurs de sélectionner
    des livres ne présentant aucuns risques ou les informer de la présence de
    sons préenregistrés.
  </li>
</ul>
<p>
  <a href="#example-extended-filtering-options">EXEMPLE 20</a> : Options de
  filtrage étendues
</p>
<ul>
  <li>Pagination identique à l’imprimé</li>
  <li>Graphiques, diagrammes et formules</li>
  <li>Normes minimales d'accessibilité (A)</li>
  <li>Normes d'accessibilité acceptées (AA)</li>
  <li>Aucun risque</li>
  <li>Audio préenregistré</li>
</ul>
<h2 id="h.nmf14n">6. La localisation</h2>

Un livre électronique peut être acheté dans n'importe quel pays, sans disponibilité limitée ni frais de livraison supplémentaires. Les lecteurs souhaitent un affichage cohérent des informations relatives à l'accessibilité, et c'est là le rôle principal du guide d'affichage. La formulation proposée dans ce guide a été largement discutée par un groupe important représentant différents acteurs des pays anglophones. Elle a été améliorée après des tests de validation et a été examinée par des groupes de testeurs.

Nous comprenons que différents pays ou différents services destinés à un public cible peuvent vouloir utiliser un langage spécifique, et nous avons prévu une certaine souplesse dans le guide pour tenir compte de cette situation tout en maintenant un niveau élevé de compréhension et une qualité similaire pour aider les utilisateurs d'un pays à trouver des informations similaires entre deux librairies ou bibliothèques dans la même zone linguistique. Il ne suffit pas de traduire les chaînes de caractères ; le sens subtil des mots et des phrases des concepts d'accessibilité doit être localisé pour une compréhension maximale. C'est pourquoi nous avons l'intention de fournir un mécanisme permettant à la communauté des éditeurs de fournir des traductions qui localisent les chaînes de caractères pour une communication tout aussi efficace dans de nombreuses langues.

La <a href="https://w3c.github.io/publ-a11y/a11y-meta-display-guide/2.0/draft/localizations">page de traduction des chaînes de localisation du guide</a> énumère les traductions en contextualisant le processus de localisation.

Les sous-sections suivantes proposent un cadre de localisation pour aider à établir des zones linguistiques dont les libellés sont convenus entre les acteurs de la zone géographique concernée.

<h3>6.1 Stratégie de localisation</h3>

Avec l'évolution rapide du paysage des livres électroniques accessibles, la plupart des personnes concernées découvrent un nouveau monde. Pour que l'information soit largement diffusée et comprise, l'implication des acteurs locaux tels que les ONG, les bibliothèques au service des personnes handicapées et d'autres acteurs locaux dans la lutte pour mettre fin à la famine de livres pour les lecteurs incapables de lire les imprimés est cruciale et doit être soulignée.

La localisation du guide d'affichage est une bonne occasion de faire connaître les nombreuses caractéristiques d'accessibilité offertes par les formats modernes tels que l'EPUB. Inversement, le fait d'avoir une échelle de projet locale pour écrire un vocabulaire compréhensible pour décrire ces caractéristiques est une approche qualitative précieuse qui profitera à tous les acteurs de la chaîne de valeur.

Pour construire un projet local et faciliter les comparaisons de retour d'expérience, vous pouvez utiliser la méthodologie, les ressources et les prototypes open source publiés par EDRLab pour le projet original <a href="https://edition-accessible.github.io/signalement/index.html">Signalement des livres numériques accessibles</a> qui a conduit à la <a href="https://edition-accessible.github.io/signalement/documents/EDRLab-Signalement_lettreW3C_FR.pdf">lettre de retour d'expérience (PDF)</a> adressée au début de 2022. Ce projet a déjà été utilisé et adapté en divers endroits.

Dans ces projets, l'accent a été mis sur les implications pour les utilisateurs finaux. Par exemple, la formulation française proposée par EDRLab résulte d'une enquête quantitative auprès de différents groupes de lecteurs, de panels d'observations individuelles soigneusement sélectionnés et d'un processus de retour d'information étendu grâce à une formule dédiée disponible sur les 140 premières plateformes de mise en œuvre.

En outre, des entreprises comme VitalSource qui ont besoin d'une localisation à grande échelle ont proposé de mettre en libre accès leur travail de traduction professionnel, ce qui a permis de produire la quantité nécessaire et qu'il vaut mieux utiliser que rien lorsqu'aucun projet national n'a publié un vocabulaire artisanal.

Pour concilier les deux sources de matériel de localisation, nous proposons un mécanisme de collecte basé sur une identification détaillée de la provenance. Parce que des personnes et des organisations ayant différents niveaux de technicité doivent pouvoir contribuer, nous acceptons à la fois les fichiers bruts par le biais de Pull requests et proposons également une interface utilisateur de localisation conviviale par le biais de GitLocalize.

<h3>6.2 Comment contribuer ?</h3>

Faites-nous d'abord savoir le plus tôt possible que vous travaillez sur une localisation et que vous souhaitez la soumettre. Cela nous permet de préparer un espace réservé pour votre travail. Ce n'est pas obligatoire, mais nous vous invitons à contacter le groupe et à participer à un appel régulier du groupe de travail, car ces appels sont ouverts à tous.

Lorsque vous êtes prêt à publier votre travail, deux options sont possibles :

Si vous ne savez pas ce qu'est un JSON ou une Pull Request, vous pouvez nous contacter afin que nous puissions attribuer un rôle de traducteur sur la <a href="https://gitlocalize.com/repo/9555">page Gitlocalize dédiée au projet</a>.
Si vous vous sentez techniquement prêt ou si vous avez un collaborateur qui peut faire une demande d'extraction, le processus consiste à dupliquer le fichier canonique original UX-Guide-Metadata/draft/localizations/fr-US/display_guide_vocabulary_w3c_en-US.json, à le modifier en changeant les valeurs devant chaque clé, et à ouvrir une demande d'extraction pour que nous puissions l'examiner. Veuillez noter que nous pourrions avoir des questions ou demander des précisions au cours du processus avant d'accepter et de fusionner votre contribution.

<h3>6.3 Comment choisir entre les fichiers de localisation ?</h3>

Comment choisir entre les fichiers de localisation ?
Les premières clés de chaque fichier JSON contiennent des informations descriptives à son sujet, notamment

* Auteur, nom de l'organisation responsable de l'établissement et de la maintenance de cette localisation
* Langue, est un code de 4 lettres où les deux premières lettres spécifient la langue selon ISO 639-1 et les deux autres le pays selon ISO 3166-1 alpha-2
* Variante, un nom libre d'un mot pour identifier votre travail.
* Audience décrit le public. Nous recommandons d'utiliser n'importe quel vocabulaire de la liste ONIX 28. Il est possible d'informer plus d'un public en séparant chacun d'eux par une virgule.
* Description, un champ libre comprenant une brève description de la manière dont cette localisation a été obtenue.


<h2 id="h.37m2jsg">7. Mise en œuvre</h2>
<p>
  <a href="https://github.com/w3c/publ-a11y/issues/268">QUESTION 268</a> :
  Coordonnées des responsables de la mise en œuvre
</p>
<p>
  Nous recueillons des informations sur les entreprises et les organisations qui
  souhaitent éventuellement fournir des exemples de mise en œuvre. Veuillez
  consulter cette
  <a href="https://github.com/w3c/publ-a11y/issues/268">question GitHub</a> pour
  prendre connaissance des entreprises et des organisations qui se sont portées
  candidates. Pour éventuellement proposer une implémentation, veuillez indiquer
  le nom de votre entreprise, votre nom et vos coordonnées.
</p>
<p>
  Ces lignes directrices fournissent un cadre général et font des suggestions
  sur l'affichage des métadonnées d'accessibilité. Il ne s'agit pas d'une
  description normative de ce qui doit être fait. Il est instructif de fournir
  des exemples de mise en œuvre de la part de la communauté.
</p>
<p>
  Les liens ci-dessous sont des pages statiques qui illustrent des mises en
  œuvre concrètes. Ces exemples proviennent de sites web d'organisations qui ont
  accepté de nous permettre de présenter le travail qu'elles ont accompli pour
  afficher les métadonnées d'accessibilité.
</p>
<p>Liens à déterminer</p>
<h2 id="h.1mrcu09">A. Remerciements</h2>
<p>Cette section n'est pas normative.</p>
<p>
  Les contributions éditoriales des personnes suivantes ont été
  essentiels à la réalisation de ce guide :
</p>

<ul>
  <li>Avneesh Singh</li>
  <li>Charles LaPierre</li>
  <li>Chris Saynor</li>
  <li>Gautier Chomel</li>
  <li>George Kerscher</li>
  <li>Gregorio Pellegrino</li>
  <li>Madeleine Rothberg</li>
  <li>Matt Garrish</li>
</ul>
<p>
  Les membres suivants du groupe de la communauté de l'édition ont contribué à
  l'élaboration de ce document :
</p>

<ul>
  <li>Chris Oliver</li>
  <li>Christopher Carr</li>
  <li>Hadrien Gardeur</li>
  <li>James Yanchak</li>
  <li>Jason White</li>
  <li>Jonas Lillqvist</li>
  <li>Miia Kirsi</li>
  <li>Naomi Kennedy</li>
  <li>Rick Johnson</li>
  <li>Simon Mellins</li>
</ul>
