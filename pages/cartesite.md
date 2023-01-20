---
layout: document
title: "Carte du site"
subtitle: 
date: 2021-01-20
---

<!DOCTYPE html>
<html lang="fr"><head>
    <meta charset="utf-8" />
    <title>À propos | LINA25</title>
    <script
        src="https://kit.fontawesome.com/a9faad54a1.js"
        crossorigin="anonymous"
    ></script>
    <link
        href="feed.xml"
        type="application/atom+xml"
        rel="alternate"
        title="Lina 25 Feed"
    />
    <!--TODO : j'ai pas l'impression que le fil rss est généré.-->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
        href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&family=Poppins:wght@200;400;700&display=swap"
        rel="stylesheet"
    />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
        rel="stylesheet"
        href='/lina25/assets/sass/main.css'
    />
    <link
    rel="stylesheet"
    href='/lina25/assets/sass/print.css'
/>
<link
rel="stylesheet"
href='/lina25/assets/sass/tableaux.css'
/>
    <base target="_blank" />
</head>
<body><nav aria-label="Accès rapide" id="skip_link">
    <a href="#main" target="_self">contenu</a>
</nav>

<nav class="nav">
    <a class="logo" href='/lina25/index.html' target="_self">
        <img
            src='/lina25/assets/images/Icons/Logo.svg'
            alt="Livre Numérique Accessible 2025"
        />
    </a>
    <ul class="menu">
        <li>
            <a href='/lina25/index.html#pourquoi' target="_self"
                >Pourquoi ce site</a
            >
        </li>
        <li>
            <a href='/lina25/index.html#savoirs' target="_self"
                >Ce que vous devez savoir</a
            >
        </li>
    </ul>
    <div id="dropdown_button">
        <button
            type="button"
            class="dropdown_btn"
            aria-label="dropdown menu"
            tabindex="0"
            hidden
        >
            <span class="nav_button">
                <i class="fa-solid fa-bars"></i>
                <span><i class="fa-solid fa-xmark"></i></span>
            </span>
        </button>
        <nav id="nav_dpdn">
            <ul id="dpdn" class="dropdown-content_wrapper" role="menu">
                <li>
                    <a
                        href='/lina25/index.html#pourquoi'
                        target="_self"
                        >Pourquoi ce site</a
                    >
                </li>
                <ul class="dropdown_savoir">
                    <li>
                        <a
                            href='/lina25/index.html#savoirs'
                            target="_self"
                            id="savoir"
                            >Ce que vous devez savoir</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/concevoir.html'
                            target="_self"
                            >Concevoir des contenus complets</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/produire.html'
                            target="_self"
                            >Produire des structures sémantiques riches</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/traiter.html'
                            target="_self"
                            >Traiter le fonds</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/collecter.html'
                            target="_self"
                            >Collecter & référencer des informations précises</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/diffuser.html'
                            target="_self"
                            >Diffuser & distribuer au plus près des besoins</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/afficher.html'
                            target="_self"
                            >Afficher une expérience de lecture riche</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/lire.html'
                            target="_self"
                            >Lire dans les meilleures conditions</a
                        >
                    </li>
                    <li>
                        <a
                            href='/lina25/pages/loi.html'
                            target="_self"
                            >Ce que dit la loi</a
                        >
                    </li>
                </ul>
            </ul>
        </nav>
    </div>
</nav>

<script>
    const btn = document.getElementById("dropdown_button");
    btn.addEventListener("click", function () {
        this.classList.toggle("button-open");
    });

    const nav = document.querySelector(".nav");
    const logo = document.querySelector(".logo");

    window.onscroll = function (e) {
        let navdpdn = document.getElementById("nav_dpdn");
        if (window.pageYOffset > 1) {
            nav.style.height = "75px";
            logo.style.width = "300px";
            navdpdn.style.top = "75px";
        } else if (window.pageYOffset < 1) {
            nav.style.height = "200px";
            logo.style.width = "400px";
            navdpdn.style.top = "200px";
        } else {
            logo.style.width = "400px";
            if (window.screen.width < 1300) {
                let navdpdn = document.getElementById("nav_dpdn");
                navdpdn.style.top = "200px";
                nav.style.height = "150px";
            } else {
                nav.style.height = "200px";
            }
        }
    };
</script>
<img src="/lina25/assets/images/Banners/SVG/Home.svg" alt="">

  <header id="contenu" class="header_documents">
    <a href="" target="_self" title="page précédente : " id="arrow_left"><i class="fa-solid fa-angle-left arrow"></i></a>
    <div class="title_pages">
      <h1>À propos</h1>
      <h2></h2>
    </div>
  </header>

  <main class="document" aria-label="Content" id="main">
    <section>
      <p>Ce site est réalisé par EDRLab.</p>

<p>Maquette et graphismes réalisés par Marion Raveau.</p>

<p>Intégration et développement par Arthur Le Meur.</p>

    </section>
  </main><footer class="page__footer page__footer-follow">
    <ul class="social-icons">
        <li><a href="/pages/apropos">À propos</a></li>
        <!--TODO-->
        <span aria-hidden="true">|</span>
        <li><a href="pages/accessibilite">Accessibilité : ????????</a></li>
        <!--TODO Ce doit aussi être un lien vers une page accessibilité qui donne les infos de test-->
        <span aria-hidden="true">|</span>
        <li><a href="https://edrlab.org/">EDRLab 2022</a></li>
        <span aria-hidden="true">|</span>
        <li id="GH">
            <a
                href="https://github.com/edition-accessible/lina25"
                rel="nofollow noopener noreferrer"
            >
                <i class="fab fa-fw fa-github" aria-hidden="true"></i>
                <span>GitHub</span>
            </a>
        </li>
        <span aria-hidden="true">|</span>
        <li id="RSS">
            <a href="/feed.xml"
                ><i class="fas fa-fw fa-rss-square" aria-hidden="true"></i
                ><span>Carte du site</span></a
            ><!--TODO-->
        </li>
    </ul>
</footer>
</body>

</html>