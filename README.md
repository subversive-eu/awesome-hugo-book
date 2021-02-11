# Hey!

## My Awesome Hugo Book

- [Français](#objectif-et-besoin) (en construction)
- [Anglais](#english) (french before)

<p align="center">
  <kbd><img src="https://subversive-eu.github.io/awesome-hugo-book/media/merakist-min.jpg" alt="Web SEO" /></kbd>
</p>

### Objectif et Besoin

- Offrir une liste d'outils pour les administrateurs et développeurs de site internet statique ou non, utilisant hugo ou non.

- Rendre plus simple l'utilisation et le développement de site sous hugo.

- Version 1 : <https://subversive-eu.github.io/book-seo/>

- Juste une page avec des favoris disponibles partout facile à interpréter.

- [Hugo version v80](https://github.com/gohugoio/hugo/releases/tag/v0.80.0)


Table des matières | 
------------ | 
[Introduction](#introduction) | ι
[Performance](#performance) | ι
[Architecture](#architecture) | ι
[Sécurité](#sécurité) | ι
[Contenu](#contenu) | ι
[Meta Data](#meta-data) | ι
[Ressources](#ressources) | ι

***

###  Introduction

Un bon site Web répondra à la question : que viennent chercher les gens sur mon site Web ? -> Votre site internet a besoin d’être documenté sur un sujet précis.

Si vous devez aborder plus de deux sujets vraiment différents, préférez utiliser un sous-domaine pour chaque sujet comme automobile vs cuisine. automobile.example.com vs cuisine.example.com

Un type de recherche une page, reste l’idéal.

**Fonctionnement de la recherche Google**

Pour faire explorer vos pages par googlebot, utiliser un sitemap.xml : example.com/sitemap.xml

Ne pas hésiter à envoyer une demande d’exploration de pages individuelles via la GoogleSearchConsole.

Vos chemins d’URL doivent être simples, intelligibles et logiques pour vos pages.

Googlebot va explorer votre site en fonction du fichier robots.txt, dans la racine de votre site example.com/robots.txt.

Vous pourrez interdire l’accès du bot a certaines pages ou dossier délicat.

Identifiez votre page canonique et les autres pages.

Assurer vous que googlebot a accés aux ressources.

J’ai fait un article sur [le fonctionnement de la recherche](https://subversive-eu.github.io/awesome-hugo-book//blog/fonctionnement-recherche.md).

**La base du SEO**

Google regarde la perfomance de votre site, il observe vos metas données ainsi que votre contenu.

Votre Architecture se doit d’être simple est logique. Vous n’oublierez pas la sécurité de votre site.

**Garder le cap**

Google mais à jour régulièrement ses consignes aux developpers, vous vous devrez de ne rien louper en lisant ces blogs :
Google For Dev #

    Dev
    Webmaster [FR]
    Webmaster

De plus il vous faudra une base de ressources displonibles pour gagner du temps dans votre travail.

Le plus important est d’avoir un objectif quantifiable et mesurable, le reste est bido

### Performance

- Préférez les petites images en taille (donc conservez la qualité)
- Compressez vos images jpg ou jpeg vers les formats -> JPEG 2000, JPEG XR ou WEBP
- Conserver uniquement le script js que vous utilisez
- Minifiez votre JS
- Conserver uniquement le css que vous utilisez
- Minifiez votre CSS
- Minifiez votre html
- Ayez un site adapté a toutes les plateformes
- Evitez les redirections
- Détestez les icônes

 *Outils*

- [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
- [Vitesse de la page](https://tools.pingdom.com/)
- [Minifier votre css](http://minifycode.com/)
- [Test Page Speed](https://www.internetmarketingninjas.com/tools/free-tools/pagespeed)

*Design réactif*

- [affiche le site en responsive multi plateforme](https://www.responsinator.com/)
- [Google Mobile friendly ?](https://search.google.com/test/mobile-friendly?)
- [Responsive-Test](https://0xfederico.github.io/test-responsive-website/)

*Image*

- [Compress Img](https://compressjpeg.com/)
- [Webp convertor](https://webp-converter.com/)
- [Squoosh compressor](https://squoosh.app/)

### Architecture

L’architecture de votre site doit être simple. L’ensemble de votre site doit être interconnecté.

Pour un utilisateur cela peut-être compliqué mais un robot lui a une certaine aisance, c’est un paradoxe. Mais ce sont les robots qui permettent de vos retrouver en haut de la page.

- Une page une utilité.
- De chaque page, je peux aller ou je veux sur le site.
- De chaque page, j’ai un contenu facile a lire avec une page performante, des meta données complètes et un contenu unique.

Demandez vous ce qu’aime les gens, ce que viennent chercher les gens sur votre site. Vos pages doivent y répondre.

- Un rendu en recherche impeccable cf schema.org
- Le sitemap est très important, il est l’index du robot, il regroupe toutes les pages.

*Outils*

- [Analyse l’architecture pour une page](https://www.siteliner.com/)
- [Analyse Générale de l’architecture du site](https://neilpatel.com/)
- [Logiciel architecture des liens](https://www.screamingfrog.co.uk/seo-spider/)
- [SiteMap validator](https://www.xml-sitemaps.com/validate-xml-sitemap.html)
- [Sitemap pour image](https://support.google.com/webmasters/answer/178636)

### Sécurité

La sécurité reste un point à ne pas négligler.
Un site peu fiable, avec des rapports des utilisateurs ne sera pas recommandable et les robots en tiendront compte.

En général le protocole https suffit.

Evitez la redirection.

Appréciez le protocole www.votredomaine.com.

gethyas.com

*Outils*

- [Webpagetest](https://www.webpagetest.org/)
- [Mozilla Observatoire](https://observatory.mozilla.org/)

### Contenu

Le contenu de votre site est le plus important !

Il doit être unique et simple mais complexe.

Le robot aime les nouveaux sites, avec beaucoup de liens, mais n’apprécie pas les liens cassés.

Il aime également le contenu frais. Aujourd’hui le monde va plus vite, a vous de suivre.

- Titre : 60 caractères
- Description: 155-160 caractères
- Mots clés: titre + description + tags/categories/etiquettes + h2 + h3
- Citez vos sources
- Utiliser des liens externes
- Utiliser des liens internes -> croiser vos pages
- 3 articles minimum par catégories
- Ratio minimum 1:2 ratio entre catégorie
- Eviter les lire ici, cliquez ici
- Evitez les liens photos ou ensemble.
- Préférez du texte qui décrit le lien, simple mais efficace
- Votre contenu doit être **unique**

*SEO*

- [Plus d’info à propos de Schema](https://schema.org/)
- [Données structurées Listes](https://developers.google.com/search/docs/guides/search-gallery)
- [JSON-LD données](https://github.com/JayHoltslander/Structured-Data-JSON-LD)
- [OpenGraph Protocol](https://ogp.me/)
- [structured-data/testing-tool](https://search.google.com/structured-data/testing-tool)
- [Debug by Iframely](http://debug.iframely.com/)
- [mon seo](https://github.com/subversive-eu/site/tree/master/themes/PaperMod/layouts/partials/templates)
- [Valider le protocole Opengraph](https://www.opengraph.xyz/)

*RSS*

- [W3 validator](https://validator.w3.org/feed/)
- [Podba](https://podba.se/validate/)

*Shortcodes*

- [Hugo shortcodes par parsiya](https://github.com/parsiya/Hugo-Shortcodes)
- [les miens](https://github.com/subversive-eu/site/tree/master/layouts/shortcodes)

*Autres Outils*

- [Convertisseur](https://convertio.co/)
- [Image Magick](https://imagemagick.org/index.php)
- [Free Photos](https://unsplash.com/)

*Rédaction*

- [Markdown Syntax Guide](https://sourceforge.net/p/hugo-generator/wiki/markdown_syntax/)
- [Evernote-powered statically-generated blogs and websites](https://github.com/zzamboni/enwrite)
- [Mon guide /outils Markdown](https://subversive.eu/articles/markdown-syntax-how-to-use-figure-with-html-css-and-tabs.html)
- [Syntaxe basique MArkdown](https://www.markdownguide.org/basic-syntax/)

*Emoji* dans le fichier config.yml

```enableEmoji: true``` 💙

- [Emoji list](https://www.webfx.com/tools/emoji-cheat-sheet/)
- [Explain Emoji](https://hugoloveit.com/emoji-support/)

*Commentaires*

- [Isso | Disqus alternative](https://posativ.org/isso/)
- [Visual Captcha](https://visualcaptcha.net/)
- [Invisible-recaptcha-validator | self-hosted](https://github.com/andrewrmn/invisible-recaptcha-validator)
- [Staticman!](https://staticman.net/)
- [Staticman tuto fr 2021](https://subversive.eu/articles/ecrire-des-commentaires-sur-un-site-statique-hugo-avec-staticman-et-heroku.html)

### Meta Data

Le balisage meta reste important tant qu’il est pratique et qu’il réponds à la demande des bots.

La demande des bots, dépends de la demande des gens. Si vous comprenez ce que les gens cherchent et aiment faire sur internet alors vous comprendrez cette liste.

La personne ou le robot qui lit votre url doit comprendre ce dont la page parle.

*Balise Head de votre page*

- Gérer le Opengraph protocol complet
- Gérer le Twitter Cards protocol complet
- Gérer le Structured Data protocol complet
- Gérer le sitemap + sitemap image
- Acceptez robots.txt noindex
- Titre
- Une hreflang
- keywords /peu utile/
- RSS
- Canonical
- Description
- Autheur
- Vos ressources
- Votre URL

*Attributs*

Très important pour le handicap, considérez que le robot est un handicapé qui ne voit pas mais se faire le contenu de la page. Pour une personne handicapée c’est pareil, elle a un robot qui lui lit les attributs, ce qui lui permet d’évoluer n’importe où, à condition que votre site en ait.

- title pour un lien ex:
```
<a Title="{{ .Name }}" href="{{ .URL | absLangURL }}"> {{ .Name }} </a>
```
- name pour un bouton ex:
```
<button name="Description du bouton" ></button>
```
- alt pour une image ex:
```
alt="description de l'image
```
- alt pour une vidéo

*Outils*

- [HTML / XHTML / XML Validator](https://validator.w3.org/)
- [Google test robots.txt](https://support.google.com/webmasters/answer/6062598)
- [HTML Ressources](https://htmlhead.dev/)
- [Tuto hugo tags](https://www.skcript.com/svr/perfect-seo-meta-tags-with-hugo/)

### Ressources

Tout ce qui ne rentre pas dans les autres catégories.

- [Danstools](https://www.danstools.com/)
- [HUGO BEST PRACTICES](https://github.com/spech66/hugo-best-practices)
- [AWESOME INCLUSIVE](https://github.com/sindresorhus/awesome)
- [Lipi static blog generator](https://sohanchy.com/Lipi/)
- [A free web scraper](https://www.parsehub.com/)
- [awesome-static-generators](https://github.com/phamap/awesome-static-generators)
- [awesome-hugo](https://www.awesome-hugo.dev/)

*Thème pour documentation*
- [Docsy](https://docsy.dev)
- [Docuapi](https://docuapi.netlify.app)
- [Learn](https://learn.netlify.app)
- [Hyas](https://gethyas.com)
- [Zdoc](https://zzo-docs.vercel.app/)
- [Compose](https://docs.neuralvibes.com/)

*Design kit*

- [Material Design](https://material.io/)
- [Material Design Lite](https://getmdl.io/)
- [Syna](https://about.okkur.org/syna/)
- [Normalize.css CSS reset](https://necolas.github.io/normalize.css/)
- [Animate.css](https://animate.style/)
- [Primer](https://primer.style/)
- [Clarity Design System](https://clarity.design/)
- [jPopup](https://www.rvdizajn.com/jpopup/)
- [Google-Fonts-Awesome](https://google-webfonts-helper.herokuapp.com/fonts)
- [EditorJs ](https://editorjs.io/)
- [dark-mode-toggle](https://github.com/GoogleChromeLabs/dark-mode-toggle)

*Icones*

- [Feathericons](https://feathericons.com/)
- [Fontawesome](https://fontawesome.com/)
- [IcoMoon](https://icomoon.io/)
- [Simpleicons](https://simpleicons.org/)
- [Octicons](https://primer.style/octicons/)

[*Cette merveilleuse photo*](https://subversive-eu.github.io/awesome-hugo-book/media/winter-photo.webp)

*Vrac*

- [Editeur de contenu github a distance](https://prose.io/)
- [Page de status microservices](https://github.com/valeriansaliou/vigil)
- [Supabase | Firebase Alternative](https://supabase.io/)
- [Editorial revue](https://www.getrevue.co/)
- [Mail List](https://substack.com/)

*Data Service*

- [DataStudio by google](https://datastudio.google.com/overview)

*Outils offrant une vue d'ensemble:*

- [technicalseo.com](https://technicalseo.com/tools/)
- [nibbler](https://nibbler.silktide.com/)
- [seotesteronline](https://www.seotesteronline.com/)
- [outiref](https://www.outiref.fr/)
- [https://alyze.com/](https://alyze.com/)
- [webpagetest](https://www.webpagetest.org/)  
- [Google text-enrichis tools tester](https://search.google.com/test/rich-results)




---
# draft :
## English

### Goal

- Deploy a full documentation about fundamentals and tricks.

-> Make life easier and faster for hugo webmaster ! (because i'm one of them and sometimes we need to stock list, like hard list !).

### Project

- Come from <https://subversive-eu.github.io/book-seo/>, it's in french, but using jekyll (hate it!) and a lot of errors and not full !
- Just want a website bookmarks ! nothing more.
- Do not think, join me, just to send a link, this can help.

going to deploy using netlify. (did)



PS: [hugo release v80](https://github.com/gohugoio/hugo/releases/tag/v0.80.0).

PS2: need a better readme.md to share project. <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>

PS3: start in french going to english ?
