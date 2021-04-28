# Hey!

## My Awesome Hugo Book

- [Français](#objectif-et-besoin) (en perpétuelle construction)
- [Anglais](#english) (french before)

<p align="center">
  <kbd><img style=" 
  width: 100%;
  height: 100%;
  border-radius: 50%;
  object-fit: cover;
  object-position: center;"
  src="https://subversive-eu.github.io/awesome-hugo-book/media/merakist-min.jpg" alt="Web SEO" /></kbd>
</p>

### Objectif et Besoin

- Offrir une liste d'outils pour les administrateurs et développeurs de site internet statique ou non, utilisant hugo ou non.

- Rendre plus simple l'utilisation et le développement de site sous hugo.

- Juste une page avec des favoris disponibles partout facile à interpréter.


Table des matières | 
------------ | 
[Introduction](#introduction) |
[Performance](#performance) |
[Architecture](#architecture) |
[Sécurité](#sécurité) |
[Contenu](#contenu) |
[Meta Data](#meta-data) |
[Accessibilité](#accessibilité) |
[Ressources](#ressources) |
[Audit](#audit) |

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

**La base du SEO**

Google regarde la perfomance de votre site, il observe vos metas données ainsi que votre contenu.

Votre Architecture se doit d’être simple est logique. Vous n’oublierez pas la sécurité de votre site.

**Garder le cap**

Google met à jour régulièrement ses consignes aux developpers, vous vous devrez de ne rien louper en lisant ces blogs :

- [Dev](https://developers.googleblog.com/)
- [Webmaster [FR]](https://webmaster-fr.googleblog.com/)
- [Webmaster](https://webmasters.googleblog.com/)

De plus il vous faudra une base de ressources displonibles pour gagner du temps dans votre travail.

Le plus important est d’avoir un objectif quantifiable et mesurable, le reste est bidon.

### Performance

- Préférez les petites images en taille (donc conservez la qualité)
- Compressez vos images jpg ou jpeg vers les formats -> JPEG 2000, JPEG XR ou WEBP
- Conserver uniquement le script js que vous utilisez
- [Minifiez votre JS](https://github.com/subversive-eu/site/blob/master/themes/PaperMod/layouts/partials/footer.html)
- Conserver uniquement le css que vous utilisez
- [Minifiez votre CSS](https://github.com/subversive-eu/site/blob/master/themes/PaperMod/layouts/partials/head.html)
- Minifiez votre html
- Ayez un site adapté a toutes les plateformes
- Evitez les redirections
- Détestez les icônes

```
Minifier votre HTML -> Dans le fichier config.yml ajouter :
minify:
 minifyOutput: true
 
Pour observer le résultat -> clic droit sur une page de votre site (local ou non) afficher le code source.
```

 *Outils*

- [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
- [Vitesse de la page](https://tools.pingdom.com/)
- [Minifier votre css](http://minifycode.com/)
- [Test Page Speed](https://www.internetmarketingninjas.com/tools/free-tools/pagespeed)
- [Minifier et nettoyer CSS JS HTML ..](https://www.10bestdesign.com/dirtymarkup/)
- [Website Speed](https://tools.pingdom.com/)
- [GTMetrix, (la même chose que la lighthouse mais en plus sévère)](https://gtmetrix.com/)
- [Le Meilleur outil !](https://web.dev/measure/)
- [Clean-Css](https://github.com/jakubpawlowicz/clean-css)

*Design réactif*

- [affiche le site en responsive multi plateforme](https://www.responsinator.com/)
- [Google Mobile friendly ?](https://search.google.com/test/mobile-friendly?)
- [Responsive-Test](https://0xfederico.github.io/test-responsive-website/)
- [Google Chrome lighthouse](https://developers.google.com/web/tools/lighthouse/)

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

- Un rendu en recherche impeccable cf schema.org.
- Le sitemap est très important, il est l’index du robot, il regroupe toutes les pages.
- [sitemap.xml dans le dossier layouts](https://github.com/subversive-eu/site/blob/master/layouts/sitemap.xml).


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

Dans le dossier `static` de votre site hugo, ajoutez le fichier `_headers` :  
Insérez si **CE QUE VOUS COMPRENEZ SEULEMENT ET UNIQUEMENT CE QUE VOUS COMPRENEZ**.  
Si vous ne comprenez rien, ne mettez rien. (Uniquement disponible avec netlify)

```
/*
  X-Content-Type-Options: nosniff
  X-XSS-Protection: 1; mode=block
  X-Frame-Options: DENY
  Referrer-Policy: no-referrer
  Cache-Control: no-store
  X-DNS-Prefetch-Control: off
```

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

- [OpenGraph Protocol](https://ogp.me/)
  - [Valider le protocole Opengraph](https://www.opengraph.xyz/)
- [Schema](https://schema.org/)
  - [Données structurées Listes](https://developers.google.com/search/docs/guides/search-gallery)
  - [structured-data/testing-tool](https://search.google.com/structured-data/testing-tool)
  - [JSON-LD données](https://github.com/JayHoltslander/Structured-Data-JSON-LD)
- [Twitter_Cards](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards)
- **[Meilleur Outil !](http://debug.iframely.com/)**
- [Templates que j'utilise](https://github.com/subversive-eu/site/tree/master/themes/PaperMod/layouts/partials/templates)
- [Les déployer depuis le partial head (dernières lignes)](https://github.com/subversive-eu/site/blob/master/themes/PaperMod/layouts/partials/head.html)
PS: Ne pas oublier dans config.yml params:
```
env: production
```
- [Robots.txt](https://github.com/subversive-eu/site/blob/master/static/robots.txt)

Ne pas utiliser ```<noscript>```, cela nuît au référencement.

*RSS*

- [RSS 2.0 Documentation](https://validator.w3.org/feed/docs/rss2.html)
- [ATOM Documentation](https://tools.ietf.org/html/rfc4287)
- [W3 validator](https://validator.w3.org/feed/)
- [Podba](https://podba.se/validate/)

*Shortcodes*

- [Hugo shortcodes par parsiya](https://github.com/parsiya/Hugo-Shortcodes)
- [les miens](https://github.com/subversive-eu/site/tree/master/layouts/shortcodes)

*Autres Outils*

- [Convertisseur](https://convertio.co/)
- [Image Magick](https://imagemagick.org/index.php)
- [Free Photos](https://unsplash.com/)
- [Verificateur de lien](https://validator.w3.org/checklink)
- [Google Analytics check](http://www.gachecker.com/)
- [SimpleSharingButtons](https://github.com/fourtonfish/SimpleSharingButtons)

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

- [Isso / Disqus alternative](https://posativ.org/isso/)
- [Visual Captcha](https://visualcaptcha.net/)
- [Invisible-recaptcha-validator / self-hosted](https://github.com/andrewrmn/invisible-recaptcha-validator)
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
- keywords (peu utile)
- RSS
- Canonical
- Description
- Autheur
- Vos ressources
- Votre URL

*Outils*

- [HTML / XHTML / XML Validator](https://validator.w3.org/)
- [Google test robots.txt](https://support.google.com/webmasters/answer/6062598)
- [HTML Ressources](https://htmlhead.dev/)
- [Tuto hugo tags](https://www.skcript.com/svr/perfect-seo-meta-tags-with-hugo/)
- [Exemple Head](https://github.com/subversive-eu/site/blob/master/themes/PaperMod/layouts/partials/head.html)
- [HTML Documentation](https://html.spec.whatwg.org/multipage/)

### Accessibilité

- [Colors](https://clrs.cc/)
- [Randoma11y - Générateur de contraste aléatoire](https://randoma11y.com/)
- [Couleurs et Couleurs de fond](http://foutchy.com/articles/article00006.asp)
- [tota11y](https://github.com/Khan/tota11y)
- [Tools from We have web accessibility in mind](https://webaim.org/resources/)
- [Wawe from webaim](https://wave.webaim.org/)
- [contrast Ratio](https://contrast-ratio.com/)

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
alt="description de l'image"
```
- alt pour une vidéo
```
alt="description de la vidéo"
```
- rel pour une pagination
```
 rel="next"
 OU
 rel="prev"
 ```

### Ressources

Tout ce qui ne rentre pas dans les autres catégories.

- [Danstools](https://www.danstools.com/)
- [HUGO BEST PRACTICES](https://github.com/spech66/hugo-best-practices)
- [AWESOME INCLUSIVE](https://github.com/sindresorhus/awesome)
- [Lipi static blog generator](https://sohanchy.com/Lipi/)
- [A free web scraper](https://www.parsehub.com/)
- [awesome-static-generators](https://github.com/phamap/awesome-static-generators)
- [awesome-hugo](https://www.awesome-hugo.dev/)
- [Larges listes d'outils gratuit](https://www.internetmarketingninjas.com/tools/free-tools/category/free-seo-tools)
- [W3C Outils](https://w3c.github.io/developers/tools/)
- [Make Perfect Readme](https://medium.com/swlh/how-to-make-the-perfect-readme-md-on-github-92ed5771c061)
- [Simple Favicon Generator](https://freelogomake.com/favicon.html)

*Outils Officiels Hugo*

- [Developer Tools](https://gohugo.io/tools/)
- [Outils pour Editeurs](https://gohugo.io/tools/editors/)

*Outils Educatif*

- [Hugo Mini Course [EN]](https://hugo-mini-course.netlify.app/)
- [Go Hugo Hq [EN]](https://gohugohq.com/)

*Editeur de contenu*
- [Sublime Text](https://www.sublimetext.com/)
- [Atom](https://atom.io/)

*Thèmes pour documentation*

- [Docsy](https://docsy.dev)
- [Docuapi](https://docuapi.netlify.app)
- [Learn](https://learn.netlify.app)
- [Hyas](https://gethyas.com)
- [Zdoc](https://zzo-docs.vercel.app/)
- [Compose](https://docs.neuralvibes.com/)

*Thèmes pour cv*

- [Resume A4](https://gitlab.com/mertbakir/resume-a4)
- [Simple Resume](https://github.com/tylerjlawson/simple-resume)
- [Editeur de contenu github a distance](https://prose.io/)
- 
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
- [Scrollbar_css](https://github.com/cntrump/scrollbar_css)
- [Include Media](https://github.com/eduardoboucas/include-media)
- [Materialize](https://materializecss.com/)
- [Tachyons](https://tachyons.io/)

*Icones*

- [Feathericons](https://feathericons.com/)
- [Fontawesome](https://fontawesome.com/)
- [IcoMoon](https://icomoon.io/)
- [Simpleicons](https://simpleicons.org/)
- [Octicons](https://primer.style/octicons/)

[*Cette merveilleuse photo*](https://subversive-eu.github.io/awesome-hugo-book/media/winter-photo.webp)

*Vrac*

- [Page de status microservices](https://github.com/valeriansaliou/vigil)
- [Supabase / Firebase Alternative](https://supabase.io/)
- [Editorial revue](https://www.getrevue.co/)
- [Mail List](https://substack.com/)
- [mydevice](https://www.mydevice.io/)

*Data Service*

- [DataStudio by google](https://datastudio.google.com/overview)

*Outils sur chrome web store*

- [Viewport Resizer – Responsive Testing Tool](https://chrome.google.com/webstore/detail/viewport-resizer-%E2%80%93-respon/kapnjjcfcncngkadhpmijlkblpibdcgm)
- [Dimensions](https://chrome.google.com/webstore/detail/dimensions/baocaagndhipibgklemoalmkljaimfdj)
- [Responsive Viewer](https://chrome.google.com/webstore/detail/responsive-viewer/inmopeiepgfljkpkidclfgbgbmfcennb)

*Outils offrant une vue d'ensemble pour Audit*

- [technicalseo.com](https://technicalseo.com/tools/)
- [nibbler](https://nibbler.silktide.com/)
- [seotesteronline](https://www.seotesteronline.com/)
- [outiref](https://www.outiref.fr/)
- [alyze](https://alyze.com/)
- [webpagetest](https://www.webpagetest.org/)  
- [Google text-enrichis tools tester](https://search.google.com/test/rich-results)

### Audit

Faire un audit est assez long, car il faut être précis. Vous ne devez pas oublier de vous fixer un objectif mesurable dans le temps et quantifiable. A partir de là, vous êtes dans la bonne direction.

Tois procédures en fonction de votre point de départ.

Plus vous êtes en difficulté plus la procédure est simple et courte surtout. Autant dire que plus vous avancerez, plus ce sera long et difficile.

A cela, vous ne devrez pas oublier l’architecture de votre site !

**Procédure 1**

Celle de Google.

- Le site est-il visible sur internet ? site:example.com
- Votre contenu est-il unique ?
- Votre commerce est-il visible sur google.com/business
- Votre site s’adapte-t-il aux mobiles ? <g.co/friendly>
- La connexion a votre site est-elle sécurisée ? https ?

Avant de passer à la suite, vous devez intégrer celle-ci entièrement.

**Procédure 2**

Cette vérification se divise en deux sous-procédures. La 2.1 vous correspondra le plus.

*Procédure 2.1*

Celle du propriétaire (vous).

- Avez-vous un objectif ?
- Quel est votre but ?
- Comment le mesurer ?
- Votre url correspond-il a votre sujet ?
- Est-il trop complexe ?

Maintenant vérifions la base. Comment les robots voient votre site. Car votre site a un objectif, s’afficher sur les moteurs de recherche.

*Procédure 2.2*

Tous les outils se trouve ici est là sur la page.

- Le sitemap fonctionne ?
- Le robots.txt est ouvert ?
- Quels sont vos perfs ?
- Votre site est-il responsive ?

En gros les deux derniers points sont trés important, je ne connais pas le vocabulaire google attribué. Mais vous devez comprendre que même si votre site s’adapte aux mobiles, s’il réponds mal au changement de taille d’écran alors il ne sera pas mis en avant. Il doit être fluide dans n’importe qu’elle circonstance. La majorité des gens surfent sur mobile mais d’autres sont sur de grands écrans.

**Procédure 3**

Celles publiques et pointilleuses.

- [Public OPQuast](https://checklists.opquast.com/fr/)
- [Web-Quality-Assurance](https://checklists.opquast.com/en/web-quality-assurance/)
- [Front-End-Checklist](https://github.com/thedaviddias/Front-End-Checklist)
- [Front-End-Performance-Checklist](https://github.com/thedaviddias/Front-End-Performance-Checklist)
- [Scan tout le site](https://webhint.io/scanner/)

---

## English (draft)

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
