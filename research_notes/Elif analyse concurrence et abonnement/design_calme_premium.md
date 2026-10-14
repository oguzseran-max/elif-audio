# Design « calme, premium, agréable à naviguer » — ce que les utilisateurs louent et critiquent, et comment l'appliquer à Elif School (état : 15 octobre 2026)

Notes de recherche pour la V2 d'Elif School (web app mobile, palette sable/marine/argile, tab bar, transitions slide, gros bouton « parler », CTA collant sur la landing). Les citations sont laissées dans la langue d'origine. Les sources antérieures à 2024 sont marquées « (ancien) ». Quatre pages primaires n'ont pas pu être ouvertes (restriction de provenance de l'outil) : la page HIG tab bars sur developer.apple.com (remplacée par le miroir developer-rno.apple.com), les tokens de motion sur m3.material.io (remplacés par la doc GitHub Material Components Android), l'article NN/g « animation-duration » (remplacé par Val Head, 2016) et caniuse.com/vibration (remplacé par un ticket mdn/browser-compat-data).

---

## Q1. Ce que les utilisateurs et les critiques louent (ou pas) dans Calm, Headspace, Balance, Waking Up, Finch, Fabulous et dans les meilleures apps de langues / tuteurs IA

### Takeaway
Ce qui est loué de façon récurrente n'est pas « la beauté » en soi mais la **réduction du nombre de décisions** : parcours linéaire clair, peu de couleurs vives, pas de menus encombrés, feedback immédiat et doux, onboarding court. Ce qui est critiqué : les carrousels superposés (Headspace Explore), les séries (streaks) qui transforment la motivation en « protection d'un chiffre », le paywall qui arrive après l'engagement sans signal préalable, et — pour les tuteurs IA — la lenteur, le bouton-pour-parler « clunky » et l'absence de mémoire des erreurs.

### Cited Findings

**Apps « calme »**
- Balance : interface notée 5/5, « polished and very well-designed » ; les utilisateurs la décrivent comme « soothing and calm », sans couleurs vives, menus encombrés ni graphismes distrayants ; installation « simple and takes less than five minutes ». Critiques : obligation de suivre les sessions dans l'ordre, mauvais placement de niveau (personnalisation 3,5/5), annulation uniquement via le store, pas de remboursement — [ChoosingTherapy, 2022, mis à jour mai 2024](https://www.choosingtherapy.com/balance-meditation-app-review/)
- Balance (avis App Store US, échantillon de 6 avis visibles) : NPS 86 ; « Love the quick exercises and daily streak! » (12 oct. 2024) ; critiques : bugs de suivi de série, difficulté à se désabonner — [Kimola](https://kimola.com/reports/explore-key-insights-from-balance-meditation-sleep-user-reviews-app-store-us-154038)
- Waking Up : « incredibly easy-to-understand », contrôles « simple », pas de « singing bowls, chants, or soundscapes playing in the background » — [iMore, 13 nov. 2023 (ancien)](https://www.imore.com/apps/this-is-the-best-meditation-app-ive-ever-used-and-ive-tried-them-all) ; MetaLab (agence) : « A clear mind is free from clutter », 3 méditations gratuites avant abonnement — [MetaLab archive](https://archive.metalab.com/projects/waking-up)
- Headspace (critique Pratt, 4 fév. 2026) : loué — cours verticaux linéaires (« journey step by step »), barre de progression, cartes dont taille/contraste/espacement signalent la tappabilité, animations subtiles + coche en fin de session. Critiqué — l'onglet Explore aux carrousels superposés est « visually cluttered and hard to navigate » ; les séries déplacent la motivation vers « protéger un chiffre » (proposition : séries visibles sur demande seulement) ; paywall qui apparaît après l'engagement (proposition : cadenas / étiquette « Premium » sur les vignettes avant ouverture) ; proposition de 3 gros boutons d'intention (« Calm Down Fast », « Focus Boost », « Sleep Now ») — [Pratt IXD](https://ixd.prattsi.org/2026/02/design-critique-headspace-ios-app-2/)
- Headspace (Raw.Studio, 10 mai 2021, ancien) : personnages non humains, volontairement ambigus ; formes courbes « no sharp edges » ; émotions montrées par métaphore (vapeur, éclairs) plutôt que par visages ; GIF courts en boucle à la place d'une vidéo d'instruction ; écrans d'intro quittables (« Tap anywhere ») ; première méditation embarquée dans le téléchargement pour ne pas attendre sur réseau lent ; onboarding final en 5 étapes ; faits scientifiques retirés de l'onboarding. Chiffres cités dans l'article (projet de 6 semaines ; impossible de confirmer qu'il s'agit de données officielles Headspace) : 38 % d'abandon entre début et fin d'onboarding, utilisateurs passant la semaine 2 « 5x » plus susceptibles de convertir, +10 % relatif d'engagement en semaine 2 après refonte — [Raw.Studio](https://raw.studio/blog/how-headspace-designs-for-mindfulness/)
- Headspace refonte 2017 (ancien) : hub « Your Journey », pistes spécialisées par situation, tooltips par onglet — [Appcues GoodUX](https://goodux.appcues.com/blog/headspaces-redesign-is-a-beautiful-expansion-of-the-core-product)
- Calm : dégradé doux bleu→violet sur l'accueil, paywall et confirmation d'achat sur dégradés bleu foncé ; principe énoncé : « visual calm should preserve legibility. » ; l'article précise que ces exemples « do not prove conversion, retention, or revenue impact » — [ScreensDesign](https://screensdesign.com/articles/calm-onboarding-design/)
- Finch (avis App Store US, échantillon de 6 avis) : NPS 90 ; « the pets are adorable » (2 fév. 2025) ; critiques : coût après l'essai — [Kimola](https://kimola.com/reports/transform-your-self-care-routine-with-finch-app-insights-app-store-us-155384)
- Principes du « design silencieux » (Figr, 16 oct. 2025) : palettes douces et sourdes (verts, bleus, neutres) « evoke tranquility and trust » ; « White space provides the silence » (Vignelli) ; feedback prévisible et immédiat ; interactions pardonnantes (undo) ; navigation stable ; notifications en périphérie ; divulgation progressive ; éviter les mouvements brusques — [Figr](https://figr.design/blog/the-ux-of-silence)

**Apps de langues / tuteurs IA**
- Duolingo, refonte des onglets principaux (4 fév. 2026) : 4 directions testées à grande échelle — *Punchy* (en-têtes vifs), *Soft* (dégradés calmes), *Modular* (cartes), *Flat* (minimal, beaucoup de blanc) ; résultat : en-têtes à hauteur hiérarchisée mais titre à position fixe, système typographique réduit, « whitespace over containers » (l'espacement sépare, au lieu d'encadrer), cartes plus plates, suppression des bordures vives ; « Good design means knowing what to remove and what to keep. » ; « We see higher engagement across tabs while maintaining our core learning metrics. » (aucun chiffre) — [Duolingo Blog](https://blog.duolingo.com/core-tabs-redesign)
- Duolingo, critique du « path » (UX Collective, 27 nov. 2022, ancien) : « I believe the 2022 release is a major step in a wrong direction. » ; commentaires : perte de choix et d'agentivité, ligues/cœurs menant au burn-out — [UX Collective](https://uxdesign.cc/down-the-wrong-path-the-disaster-of-the-latest-duolingo-ui-update-a4cdd1e6ea1c)
- Babbel, rebranding (1er fév. 2024) : nouvelle police « Feature Text » choisie pour un rendu « premium » ; système à 3 éléments (images détourées/silhouettes, « product cards », photographie de vrais apprenants en situation) ; motivations issues de la recherche Human8 : Meaning, Security, Achievement — [Babbel press](https://babbel.com/press/en-us/releases/babbel-unveils-a-bold-new-chapter-a-transformational-rebranding) ; refonte 2019 (ancien) : cercle de progression, nombre de leçons terminées, les apprenants voulaient « more direction about what to do next », « a sense of accomplishment is a key part of staying motivated » — [Babbel Magazine](https://www.babbel.com/en/magazine/course-overview-update)
- Speak : onboarding en 14 étapes sous forme de conversation avec le tuteur IA, cartes récapitulatives montrant comment les réponses façonnent le programme, paywall « soft » après le quiz avec note 4,8 et témoignages, 2 paliers (Premium / Premium Plus) et un choix de plan étalé sur plusieurs écrans signalé comme friction ; tableau de bord qui sépare « prochaine leçon » et « Jump-in lessons » — [ScreensDesign](https://screensdesign.com/showcase/speak-learn-spanish-french) ; « Polished, intuitive interface and well-paced beginner content », mais « speech recognition is overly lenient », paliers « confusing and potentially expensive », l'IA finit chaque réponse par une question (effet « interrogation ») — [LanguaTalk, 19 fév. 2026 (site concurrent)](https://languatalk.com/blog/speak-app-review/)
- Praktika (Trustpilot, juillet 2026, note globale 3,7) : « very intuitive interface » ; tuteur « eerily human » ; « gave calm and polite feedback on my responses ». Critiques : « clunky button-to-talk », « really slow unnatural responses from the bot », texte affiché avant la voix (distrayant), voix du tuteur gratuit « a bit altered for no reason », « no memory on common errors », phrases coupées en fin, interstitiels « are you ready? » qui cassent le flux — [Trustpilot](https://www.trustpilot.com/review/praktika.ai?page=4)
- Loora (avis iOS compilés) : loué — score « about every syllable of my pronunciation », montre « my mistakes and the correct form ». Critiqué — « Bot's voice sounds cheep », limite de « 45 second » en entretien, essai de 2 conversations trop court, limites du gratuit non expliquées, onglet grammaire confus — [JustUseApp](https://justuseapp.com/en/app/1552708303/loora-speak-english-daily/reviews)

### Inferences
- La palette sable/marine/argile d'Elif correspond exactement au registre « soft, muted, neutrals » loué (Figr, Balance, Calm) ; la condition posée par toutes ces sources est la **lisibilité** (contraste, cf. Q6) — un fond sable avec texte argile clair est le piège typique.
- Les critiques convergentes (Headspace Explore, Duolingo path) montrent que le « calme » se perd dès qu'il y a **plus d'un carrousel par écran** ou que l'on retire du **choix** à l'utilisateur ; Elif devrait garder un seul chemin principal + un accès libre (« Jump-in » façon Speak).
- Une typographie « serif display + sans body » n'est attestée par aucune source directe sur les apps calmes ; Babbel justifie une police « premium » (Feature Text, probablement à empattements — à vérifier) ; à traiter comme choix de marque, non comme preuve.
- Les séries (streaks) sont un sujet polarisant : louées chez Balance (« daily streak! »), critiquées chez Headspace/Duolingo ; la version « douce » recommandée est une série **visible sur demande**, sans perte punitive.

### Gaps
- Fabulous : aucune source exploitable obtenue (pas de teardown ni d'avis récents trouvés dans le temps imparti).
- Design sonore (sons d'interface, earcons) de Calm/Headspace : rien de documenté ; Figr ne traite que des indices « ambient, non-intrusive ».
- Mode sombre : aucune donnée d'adoption ou de préférence trouvée pour ces apps.
- Illustrations vs photos : seule Babbel (photos d'apprenants, 2024) et Headspace (illustrations, 2021) sont documentées ; pas de comparaison testée.

---

## Q2. Patterns de navigation mobile web / PWA qui réduisent la réflexion

### Takeaway
Les guides plateformes convergent : 3 à 5 onglets avec libellés concrets (pas « Home »), tab bar toujours visible sauf en modal, bottom sheets pour les choix réversibles et répétés, modals seulement pour les actions coûteuses ; transitions de 200–300 ms pour les petits éléments et ~300 ms pour les changements d'écran, avec easing décéléré à l'entrée et accéléré à la sortie. L'API View Transitions est utilisable en production en octobre 2026 (≈93 % des navigateurs, iOS Safari 18+).

### Cited Findings
- Apple HIG (tab bars) : « three to five tabs in iOS » ; titres concis — noms concrets pour des catégories, verbes pour des contenus temporels (« Watch Now ») ; éviter les titres vagues comme « Home » ; éviter l'onglet de débordement « More » ; garder la tab bar visible pendant la navigation sauf dans une vue modale ; ne pas y mettre de contrôles d'action (utiliser une toolbar) ; la barre se masque quand le clavier est affiché ; icônes bitmap : 25×25 pt (circulaire, regular) / 18×18 pt (compact) — [Apple HIG (miroir)](https://developer-rno.apple.com/design/human-interface-guidelines/components/navigation-and-search/tab-bars)
- Material 3 Expressive (14 mai 2025) : la navigation bar d'origine est dépréciée au profit d'une « flexible navigation bar » **plus basse** ; libellés à droite de l'icône sur écrans moyens ; les navigation drawers sont dépréciés au profit du rail (sans remplacement explicite sur téléphone) — [9to5Google](https://9to5google.com/2025/05/14/material-3-expressive-navigation/)
- Duolingo (fév. 2026) : barre d'en-tête cohérente entre onglets, titres à position fixe, « whitespace over containers », cartes plus plates — [Duolingo Blog](https://blog.duolingo.com/core-tabs-redesign)
- Babbel (2019, ancien) : vue d'ensemble montrant ce qui est fini et « what comes next », cercle de progression, retour au cours principal en un tap — [Babbel Magazine](https://www.babbel.com/en/magazine/course-overview-update)
- Bottom sheet vs modal : test en 3 questions (réversible ? répété dans la session ? besoin de lire sans distraction ?) — au moins 2 « oui » → bottom sheet ; modal pour l'irréversible/coûteux (paiement, permissions, suppression) ; sheet dimensionnée au contenu, fermeture par glissement vers le bas + bouton explicite ; ne jamais empiler un modal sur une sheet ; cibles tactiles 44×44 pt iOS / 48×48 dp Android — [Dolfy](https://www.dolfy.ai/blog/bottom-sheet-or-modal-mobile-interruption-pattern)
- Durées (Val Head, mai 2016, ancien) : plage de départ « 200ms to 500ms » ; petits éléments 200–300 ms ; grands déplacements ou easing élastique 400–500 ms ; rappel NN/g : « 100ms is perceived as instant », 1 s = limite du flux de pensée ; perception visuelle ≈230 ms — [valhead.com](https://valhead.com/?p=2978)
- Tokens Material 3 (doc GitHub Material Components Android) : short4 = 200 ms, medium2 = 300 ms, medium4 = 400 ms, long2 = 500 ms ; easing standard `cubic-bezier(0.2, 0, 0, 1)`, emphasized-decelerate `cubic-bezier(0.05, 0.7, 0.1, 1)` (entrées), emphasized-accelerate `cubic-bezier(0.3, 0, 0.8, 0.15)` (sorties) ; « duration should increase as the area/traversal of an animation increases » ; patterns par défaut : shared axis et fade-through à 300 ms / easing standard, fade entrant 150 ms linéaire (la doc cite « long1 (300ms) » alors que la table donne long1 = 450 ms — incohérence de la source) — [GitHub material-components-android](https://github.com/material-components/material-components-android/blob/master/docs/theming/Motion.md?ref=androidweekly.io)
- View Transitions (même document) : 92,9 % des utilisateurs mondiaux ; iOS Safari 18.0+ ; Chrome Android 154 ; Samsung Internet 23+ ; Firefox 144+ — [caniuse](https://caniuse.com/view-transitions) ; Baseline « Newly available » avec Firefox 144 le 14 oct. 2025 ; cross-document livré en 2024 ; `view-transition-name: match-element` (Chrome 137, Firefox 144, Safari 18.4) ; groupes imbriqués Chrome 140 seulement ; aucune recommandation officielle de durée (exemples à 0,25 s et 0,5 s) — [Chrome Developers, 2025](https://developer.chrome.com/blog/view-transitions-in-2025)
- Passage web → app : « deep link and auto-login » pour une remise en main fluide — [RevenueCat, 11 déc. 2025](https://www.revenuecat.com/blog/growth/web-to-app-funnels.md)

### Inferences
- Pour Elif : 3 ou 4 onglets maximum (ex. « Parler », « Leçons », « Progrès », « Profil ») avec libellés **toujours visibles** (HIG : titres concis ; M3 : barre plus basse) ; mettre le bouton « parler » dans le contenu, pas dans la tab bar (HIG : pas d'action dans la tab bar).
- Slide **latéral** pour la hiérarchie (entrer dans une leçon → retour), fade-through (≈300 ms, standard easing) pour changer d'onglet : c'est le pairing M3 par défaut et il évite la sensation de « page qui saute ».
- Respect du bouton retour : avec View Transitions cross-document ou un router SPA qui pousse dans `history`, le geste retour Android/iOS doit fermer une bottom sheet avant de quitter l'écran (inférence d'après la règle « ne pas empiler » de Dolfy ; aucune source mesurée).
- Une carte « Reprendre où vous en étiez » en haut de l'accueil répond directement au besoin « more direction about what to do next » (Babbel) et à la structure « next lesson / jump-in » (Speak).

### Gaps
- Skeleton screens vs spinners et UI optimiste : aucune source primaire (NN/g) atteinte ; pas de chiffre.
- Comportement du bouton retour navigateur dans les PWA et liens profonds : aucune source dédiée trouvée.
- Nombre optimal d'onglets mesuré par A/B test : non trouvé (seuls les guides plateformes).

---

## Q3. Interaction vocale : le bouton « parler », transcriptions, corrections, bruit et permissions

### Takeaway
Les leaders grand public (ChatGPT, Gemini Live) ont basculé vers le **mains libres avec transcription en direct intégrée au fil de conversation** et des contrôles larges « Hold / End », tout en laissant un mode séparé optionnel ; les tuteurs IA sont surtout critiqués pour la **latence**, le **bouton-pour-parler maladroit**, le texte qui précède la voix, l'absence de mémoire des erreurs et des limites de durée arbitraires. Côté web, la gestion des permissions micro doit prévoir l'erreur `NotAllowedError`, le comportement différent de Safari, et l'absence d'API de vibration native sur iOS.

### Cited Findings
- ChatGPT (25 nov. 2025) : le mode vocal est intégré à l'interface principale ; transcription en direct (« watch answers appear »), relecture des messages précédents, images/cartes visibles pendant la conversation ; l'ancien écran séparé à « blue orb » reste disponible via « Separate mode » dans Réglages > Voice Mode ; conversation « hands-free » — [Android Authority](https://www.androidauthority.com/chatgpt-voice-mode-in-chat-3619633)
- Gemini Live (15 août 2024, ancien) : interface plein écran « quite clean » ; gros boutons « Hold » et « End » en bas ; on peut dire « stop » ; réglage « Interrupt Live responses » ; transcription disponible après la conversation dans l'historique ; fonctionne écran verrouillé avec notification « Live with Gemini » ; 10 voix décrites par ton/hauteur — [9to5Google](https://9to5google.com/2024/08/15/gemini-live-rolling-out/) ; test en cours (12 oct. 2026) : l'indicateur vocal en « pill » en bas est remplacé par une **animation en forme d'onde**, et un bouton **mute** (icône haut-parleur, coin supérieur droit) coupe la voix sans toucher au volume système — aujourd'hui les utilisateurs doivent activer les sous-titres et baisser le volume — [Android Headlines](https://www.androidheadlines.com/2026/10/google-tests-gemini-live-interface-mute-button.html)
- Praktika (juil. 2026) : « clunky button-to-talk » ; « really slow unnatural responses from the bot » ; « the conversation is sluggish even at the fastest speed setting » ; texte affiché avant que l'IA parle = distrayant ; phrases coupées (« last word is not understand ») ; « no memory on common errors » ; loué : « The ability to decrease or increase speed », feedback « calm and polite » — [Trustpilot](https://www.trustpilot.com/review/praktika.ai?page=4)
- Speak : « words light up as you say them » dans les Speaking Drills ; les roleplays se terminent automatiquement après 3 tâches ; résumé d'erreurs bref après le roleplay ; reconnaissance « overly lenient » (une phrase aux mots inversés peut avoir un score parfait) ; corriger l'élève sans qu'il s'en aperçoive est vu comme un défaut ; pas de suivi cumulatif des erreurs — [LanguaTalk, fév. 2026](https://languatalk.com/blog/speak-app-review/) ; comparaison de sa prononciation à l'exemple, chat tuteur avec saisie texte, speech-to-text et traductions — [ScreensDesign](https://screensdesign.com/showcase/speak-learn-spanish-french)
- Loora : note par syllabe louée ; « 45 second limit is worst » ; ne corrige pas un mot inventé ; change de sujet brusquement et oublie — [JustUseApp](https://justuseapp.com/en/app/1552708303/loora-speak-english-daily/reviews)
- Permissions micro (doc Daily.co) : `NotAllowedError` = prompt refusé par l'utilisateur **ou** micro non accordé au navigateur par l'OS ; Safari lève `OverconstrainedError` là où Chrome/Firefox lèvent `NotFoundError` ; sur iOS un rechargement de page suffit souvent à ré-afficher le prompt, certains Android exigent un passage par les réglages ; afficher des instructions adaptées à l'appareil ; pattern « lobby » de pré-vérification du micro ; icônes rouges avec libellé « Allow » qui ouvre les instructions — [Daily.co](https://docs.daily.co/docs/daily-js/guides/device-permissions)
- Haptique web : `navigator.vibrate` n'est pas pris en charge nativement par Safari iOS ; la vibration observée dans une démo provient d'un `<input type="checkbox" switch>` (Safari 17.4) qui déclenche un retour haptique — [mdn/browser-compat-data #29166](https://github.com/mdn/browser-compat-data/issues/29166)

### Inferences
- Le « gros bouton parler » unique d'Elif doit offrir **deux modes** : tap-pour-parler (par défaut, explicite, rassurant pour débutants) et mains libres optionnel avec interruption (Gemini « Interrupt Live responses ») ; les critiques « clunky button-to-talk » visent surtout l'obligation de tenir/appuyer à chaque tour.
- Afficher la **voix d'abord, le texte en même temps ou juste après** (streaming synchronisé), jamais le texte avant la voix (plainte Praktika), avec mots qui s'éclairent pendant la lecture (Speak).
- États à dessiner explicitement : *écoute* (onde), *réflexion* (pulsation douce ≤1 s avant un premier mot ou un son de remplissage), *parle* (onde + bouton mute/sous-titres façon Gemini), *erreur micro* (carte avec instructions iOS/Android).
- Corrections : résumé **après** le tour (pas d'interruption), avec forme fautive → forme correcte, et un carnet d'erreurs récurrentes (manque chez Speak, Praktika et Loora).
- Pas de limite de durée visible du type « 45 s » ; si une limite technique existe, la masquer par un minuteur doux ou la fixer bien au-delà.
- Haptique : utiliser `navigator.vibrate` sur Android uniquement, feature-detect, et accepter l'absence sur iOS (ou l'astuce du switch Safari 17.4, fragile).

### Gaps
- Environnements bruyants (suppression de bruit, détection de fin de phrase) : aucune source trouvée côté UX produit.
- Taille et placement précis du bouton vocal chez Speak/Praktika/Loora : non documentés dans les sources accessibles.
- Mesure de latence « acceptable » pour un tuteur vocal : aucune étude chiffrée trouvée (seules les plaintes qualitatives).

---

## Q4. Landing page web qui convertit (abonnement vendu hors store)

### Takeaway
Sur le web, les données 2025–2026 (vendeurs d'outils, donc à pondérer) indiquent que **les offres sans essai gratuit** l'emportent, qu'un **plan annuel unique** avec remise web-exclusive est la norme, que la majorité des pertes se fait **avant** le paywall, et qu'un **CTA collant en bas sur mobile** peut fortement augmenter la conversion. Sans App Store, la confiance doit être construite sur la page : démo, preuve sociale, conditions d'annulation claires.

### Cited Findings
- FunnelFox, *State of Web2App 2026* (15 janv. 2026, données 2025, éditeur de funnels) : conversion finale 3,0 % sur web vs 1,5 % in-app à produit/dépense égaux ; seuls 13 % atteignent le paywall, 3 % achètent ; la plus grande fuite est **avant** le paywall (quiz/onboarding) ; répartition du revenu par structure d'essai : sans essai 56,8 %, essai payant 28,9 %, essai gratuit 14,3 % ; « no-trial offers consistently outperform trial-based flows on the web » ; durée de plan : mensuel 48,8 %, hebdo 30,5 %, annuel 12,2 % ; indice de prix régional (US = 1,00) : Pays-Bas 1,62, **Turquie 0,29** ; upsells = +200 % de LTV (médiane ~9,31 $) ; plusieurs titres du rapport contredisent ses graphiques (« 0 % ») — à citer avec prudence — [FunnelFox](https://funnelfox.com/state-of-web2app-2026)
- RevenueCat (11 déc. 2025) : commencer par une « mini landing page » ; mobile-first ; Apple Pay ; **limiter le nombre de plans** ; « Lead with a single annual plan » et garder le mensuel in-app ; remise web-exclusive (Plantin : 30 %) ; les essais gratuits convertissent moins bien sur web (fraude, intention faible) → alternatives : essai payant 7 jours à 1 $, garantie remboursement, essai très court ; ~50 % de paiements échoués sur web (prévoir des relances) ; « video paywalls as mini demos » ; « Without app store credibility, you need to actively build trust on the web » ; frais 15–30 % store vs 2–3 % (≈6 % tout compris) web — [RevenueCat](https://www.revenuecat.com/blog/growth/web-to-app-funnels.md)
- CTA collant (Convertica, e-commerce, non daté) : barre fine fixée en bas, une ligne de texte + un bouton pleine largeur ; mobile : **+252,9 %** de taux de commande à 98 % de confiance ; desktop : aucun effet ; tailles d'échantillon non publiées — [Convertica](https://convertica.org/ecommerce-case-study-sticky-cta/)
- Headspace, tests de fiche store (déc. 2023 – mai 2024) : 15 séries d'A/B tests (US, UK, CA, AU, DE, FR) sur fonds **vifs**, légendes concises, zooms sur bénéfices, preuve sociale ; **+34 %** de conversion organique moyenne — [M&C Saatchi Performance](https://www.mcsaatchiperformance.com/case-studies/aso-case-study-for-headspace-mc-saatchi-performance/)
- Speak : paywall après le quiz avec note 4,8 et témoignages, graphique « progrès plus rapide en Premium », 2 paliers, sélection de plan sur plusieurs écrans signalée comme friction, programme de parrainage avec cash — [ScreensDesign](https://screensdesign.com/showcase/speak-learn-spanish-french)
- Essais « généreux » et friction d'annulation : Balance — essai d'un an loué (« a remarkable one-year free trial »), mais annulation via le store et absence de remboursement critiquées — [ChoosingTherapy](https://www.choosingtherapy.com/balance-meditation-app-review/) ; Waking Up — 3 méditations gratuites avant abonnement — [MetaLab](https://archive.metalab.com/projects/waking-up) ; Loora — essai de 2 conversations jugé trop court — [JustUseApp](https://justuseapp.com/en/app/1552708303/loora-speak-english-daily/reviews)
- Performance de page (seuils Core Web Vitals, mars 2026) : LCP ≤ 2,5 s, INP ≤ 200 ms, CLS ≤ 0,1, mesurés au 75e percentile des visites réelles — [bmad-plus CWV reference](https://cdn.jsdelivr.net/npm/bmad-plus@0.9.0/src/bmad-plus/packs/pack-seo/ref/cwv-thresholds.md)

### Inferences
- Pour Elif (vente web, audience TikTok francophone/turcophone) : hero avec **le visage/la voix d'Elif en démo jouable sans compte** (équivalent du « video paywall as mini demo » et des 3 méditations gratuites de Waking Up), puis CTA collant bas sur mobile (+252,9 % mesuré ailleurs, à retester).
- Sans preuve sociale : montrer à la place une démo réelle, un compteur honnête (« X conversations cette semaine » si vrai), le visage du fondateur, un prix annuel unique, et une phrase d'annulation en un clic — c'est la lecture directe de « actively build trust » (RevenueCat) ; **ne pas** fabriquer de notes ou d'avis.
- Tarification : un plan annuel mis en avant + mensuel discret ; envisager l'essai payant court (1 € / 7 jours) plutôt qu'un essai gratuit ; prix localisé pour la Turquie (indice 0,29).
- Le paywall doit être **annoncé** (cadenas sur les leçons premium — critique Pratt) et arriver après une première conversation réussie, pas au milieu d'une leçon (plainte Praktika).

### Gaps
- Aucune donnée sur l'effet d'un visage/vidéo dans le hero spécifiquement pour une app de langue ; seule la pratique « vidéo = mini-démo » est documentée.
- Aucun benchmark de vitesse de page spécifique aux landing pages d'apps d'abonnement sur Android milieu de gamme (seuls les seuils CWV génériques).
- « Que montrer sans preuve sociale » : aucune étude trouvée ; recommandations ci-dessus = inférences.

---

## Q5. Contraintes de performance (Android milieu de gamme, audience TikTok)

### Takeaway
Budget d'animation : **n'animer que `transform` et `opacity`**, promouvoir peu de calques, viser ~4–5 ms de compositing ; polices en WOFF2 avec `font-display: optional` pour le corps et `swap` pour les titres de marque, `size-adjust` pour éviter les sauts ; tenir LCP ≤ 2,5 s / INP ≤ 200 ms / CLS ≤ 0,1 au 75e percentile.

### Cited Findings
- Seules deux propriétés sont gérées par le compositeur seul : `transform` et `opacity` ; toute autre propriété déclenche layout ou paint ; promouvoir avec `will-change: transform` « within reason, don't overdo it! » ; chaque calque coûte de la mémoire et de la bande passante CPU→GPU, et « on low-memory devices » le coût peut dépasser le bénéfice ; cible ≈ 4–5 ms de compositing pendant scroll/transitions ; technique FLIP pour ramener d'autres propriétés à transform/opacity — [web.dev](https://web.dev/articles/stick-to-compositor-only-properties-and-manage-layer-count)
- Polices : WOFF2 (~30 % plus compact que WOFF) ; `preconnect` vers `fonts.googleapis.com` et `fonts.gstatic.com` (avec `crossorigin`) ; `font-display: swap` pour les éléments de marque, `optional` (100 ms de blocage, pas de swap) pour le corps de texte ; `size-adjust` sur la police de repli pour réduire le CLS ; `system-ui` pour le corps si possible ; pas de police d'icônes (SVG) ; `preload` avec parcimonie (ignore `unicode-range`) ; l'auto-hébergement n'est pas automatiquement plus rapide (données Web Almanac) — [web.dev](https://web.dev/articles/font-best-practices)
- Seuils Core Web Vitals (mars 2026) : LCP bon ≤ 2,5 s (mauvais > 4 s) ; INP bon ≤ 200 ms (mauvais > 500 ms) ; CLS bon ≤ 0,1 (mauvais > 0,25) ; évaluation au 75e percentile — [bmad-plus CWV reference](https://cdn.jsdelivr.net/npm/bmad-plus@0.9.0/src/bmad-plus/packs/pack-seo/ref/cwv-thresholds.md)
- iOS Safari zoome automatiquement sur un champ dont le texte rendu est < 16 px ; correctif : `font-size` ≥ 16 px sur les inputs ; le contournement `maximum-scale=1` bloque le pinch-zoom sur Android (accessibilité) — [Rick Strahl, 17 avr. 2023](https://weblog.west-wind.com/posts/2023/Apr/17/Preventing-iOS-Textbox-Auto-Zooming-and-ViewPort-Sizing)
- Headspace (2021, ancien) : première session embarquée dans le téléchargement « to reduce waiting on slow connections » ; GIF courts plutôt que vidéo — [Raw.Studio](https://raw.studio/blog/how-headspace-designs-for-mindfulness/)

### Inferences
- `backdrop-filter`/flou, parallaxe et ombres animées ne sont ni `transform` ni `opacity` : ils repassent par paint et sont donc à proscrire sur les surfaces qui bougent (inférence directe de la règle web.dev ; pas de benchmark chiffré trouvé). Un « verre dépoli » statique sur la tab bar reste envisageable si non animé.
- Transitions slide d'Elif : implémenter en `transform: translateX()` + `opacity`, 250–300 ms, et activer `will-change` seulement sur les deux écrans en transition.
- Vidéo hero : poster image + lecture à la demande, jamais en autoplay lourd ; privilégier une courte boucle muette ou l'audio d'Elif déclenché par tap (cf. GIF Headspace).
- Précharger les 2 premiers messages audio d'une leçon pendant l'écran d'accueil (équivalent de la « première méditation embarquée »).

### Gaps
- Formats d'image (AVIF vs WebP) : aucune source primaire consultée ; pas de chiffre.
- Pas de benchmark public « animation budget » spécifique aux téléphones Android à ~150–250 € ; la règle compositor-only est générique.
- `prefers-reduced-motion` : aucune donnée d'adoption trouvée ; à appliquer par principe (supprimer slides → fade court).

---

## Q6. Accessibilité et typographie pour le français et le turc

### Takeaway
Le vrai risque turc n'est pas l'absence de glyphes mais le **point du i** : capitales, petites capitales et ligatures `fi`/`ffi` effacent le point et rendent « Diyarbakır » illisible si la police n'a pas de substitution `locl` TRK et si le texte n'est pas balisé `lang="tr"`. Contraste : 4,5:1 (texte), 3:1 (texte ≥ 24 px ou ≥ 18,67 px gras, et composants UI dans chaque état), inputs ≥ 16 px, cibles 44 pt / 48 dp.

### Cited Findings
- Turc : « Dotted İi and dotless Iı are separate letters in Turkish (TRK) language. » — [Localfonts](https://localfonts.eu/typography-basics/fonts-the-importance-of-localisation/local-features/turkish-feature-locl/)
- Mise en capitales ou petites capitales : le point du i disparaît et « Diyarbakır » montre deux lettres identiques ; les ligatures `fi`/`ffi` enlèvent aussi le point ; correctif côté police : glyphe `idotaccent` + substitution `locl` pour TRK, KAZ, TAT, CRT, AZE ; le mécanisme dépend de la **balise de langue** appliquée au texte — [Glyphs](https://glyphsapp.com/learn/localize-your-font-turkish)
- Contraste WCAG : 4,5:1 pour le texte (#777777 = 4,47:1 échoue, pas d'arrondi) ; 3:1 pour le « large text » (≥ 18 pt ≈ 24 px, ou ≥ 14 pt ≈ 18,67 px en gras ≥ 700) ; 3:1 pour les composants UI et leurs états (focus, hover), chacun séparément ; AAA : 7:1 / 4,5:1 ; composants inactifs exemptés — [WebAIM](https://webaim.org/articles/contrast/)
- Inputs ≥ 16 px sur iOS Safari sinon zoom automatique — [Rick Strahl, 2023](https://weblog.west-wind.com/posts/2023/Apr/17/Preventing-iOS-Textbox-Auto-Zooming-and-ViewPort-Sizing)
- Cibles tactiles minimales : 44×44 pt (iOS) / 48×48 dp (Android) — [Dolfy, citant HIG et Material](https://www.dolfy.ai/blog/bottom-sheet-or-modal-mobile-interruption-pattern)
- Calm : « visual calm should preserve legibility. » — [ScreensDesign](https://screensdesign.com/articles/calm-onboarding-design/)

### Inferences
- Baliser `<html lang="fr">` et chaque segment turc en `<span lang="tr">` (ou `lang="tr"` sur l'écran de leçon) : nécessaire à la fois pour `locl` et pour que `text-transform: uppercase` donne « İ » et non « I » ; mieux : **éviter `text-transform: uppercase` et `font-variant: small-caps`** sur du turc, et désactiver les ligatures discrétionnaires (`font-variant-ligatures: no-discretionary-ligatures`, voire `none` pour le turc).
- Tester la police choisie avec « ışık / İstanbul / Diyarbakır / şğçöü » dans un titre en capitales et dans « fiil » avant de valider la V2 ; les familles Google Fonts majeures couvrent généralement le Latin étendu, mais la présence de `locl` TRK n'est pas garantie (à vérifier police par police ; aucune liste fiable trouvée).
- Palette sable/marine/argile : le marine sur sable passera 4,5:1 ; l'argile (terre cuite) en texte sur sable est à vérifier (risque < 4,5:1) → réserver l'argile aux grands titres (≥ 24 px, 3:1) ou aux surfaces, pas au texte courant.

### Gaps
- Interligne et tailles minimales recommandées pour le français/turc sur mobile : aucune source chiffrée trouvée (les sources accessibles ne traitent que du contraste et du zoom iOS).
- Diacritiques français (é, è, ç, œ) : aucun problème documenté ; absence de source spécifique.
- Liste de polices web avec `locl` turc vérifié : non trouvée.

---

## Q7. Le design « calme et premium » augmente-t-il réellement conversion et rétention des apps d'apprentissage ?

### Takeaway
Les preuves sont **indirectes et partielles** : une refonte « moins encombrée » chez Duolingo a donné « higher engagement » (sans chiffre), un onboarding allégé chez Headspace est associé à +10 % d'engagement en semaine 2 (chiffre non officiel), et les scores de satisfaction des apps calmes (Balance NPS 86, Finch NPS 90) sont élevés ; mais aucune étude A/B publique n'isole « l'esthétique calme/premium » comme variable, et un contre-exemple existe (fonds **vifs** gagnants sur les fiches store Headspace, +34 %).

### Cited Findings
- Duolingo (fév. 2026) : quatre directions testées (*Punchy*, *Soft*, *Modular*, *Flat*) ; la version livrée privilégie l'espace blanc et des cartes plus plates ; « higher engagement across tabs while maintaining our core learning metrics » ; aucun chiffre ni indication de la direction gagnante — [Duolingo Blog](https://blog.duolingo.com/core-tabs-redesign)
- Headspace (Raw.Studio, 2021, ancien ; attribution incertaine) : +10 % relatif d'engagement en semaine 2 après refonte de l'onboarding ; conversion en hausse sur 90 jours ; utilisateurs passant la semaine 2 « 5x » plus susceptibles de convertir — [Raw.Studio](https://raw.studio/blog/how-headspace-designs-for-mindfulness/)
- Headspace, fiches store (déc. 2023 – mai 2024) : +34 % de conversion organique avec, entre autres, des **fonds vifs** et des légendes concises — [M&C Saatchi Performance](https://www.mcsaatchiperformance.com/case-studies/aso-case-study-for-headspace-mc-saatchi-performance/)
- Satisfaction : Balance NPS 86 — [Kimola](https://kimola.com/reports/explore-key-insights-from-balance-meditation-sleep-user-reviews-app-store-us-154038) ; Finch NPS 90 — [Kimola](https://kimola.com/reports/transform-your-self-care-routine-with-finch-app-insights-app-store-us-155384) (échantillons de 30 avis)
- Babbel (2019, ancien) : la motivation dépend du progrès visible — « a sense of accomplishment is a key part of staying motivated » (recherche utilisateur, sans chiffre) — [Babbel Magazine](https://www.babbel.com/en/magazine/course-overview-update)
- Avertissement d'une source teardown : les exemples « do not prove conversion, retention, or revenue impact » — [ScreensDesign](https://screensdesign.com/articles/calm-onboarding-design/)
- Web2App : la majorité des pertes est avant le paywall (13 % y arrivent) — donc la **fluidité des premiers écrans** pèse plus que l'esthétique du paywall — [FunnelFox](https://funnelfox.com/state-of-web2app-2026)

### Inferences
- Ce qui est mesuré comme payant, c'est la **réduction de friction et de clutter** (onboarding plus court, un seul chemin, progrès visible), pas la « palette calme » en soi ; le calme visuel est surtout un **facteur de confiance et de satisfaction** (NPS), à combiner avec des éléments de contraste/énergie aux moments de conversion (cf. fonds vifs Headspace, bouton « Celebrate » Duolingo).
- Pour Elif : garder la base sable/marine calme, mais donner au bouton « parler » et au CTA d'abonnement un contraste franc (argile saturé ou marine plein) pour ne pas « éteindre » l'appel à l'action.

### Gaps
- Aucun A/B test public isolant « esthétique calme/premium » vs « vive » sur la conversion d'une app de langue (Babbel, Speak et Praktika n'ont rien publié de tel).
- Aucun chiffre de rétention attribuable à une refonte visuelle chez Calm, Balance, Waking Up ou Finch.
- Les chiffres Headspace 2021 proviennent d'un article tiers ; non confirmés par Headspace.

---

## Checklist « À faire / À éviter » pour la V2 d'Elif School (25 items)

### À faire
1. Limiter la tab bar à 3–4 onglets avec libellés concrets toujours visibles (pas « Accueil ») et la garder affichée sauf en modal — HIG, M3 Expressive.
2. Mettre une carte « Reprendre » en tête d'accueil + un accès libre « Parler maintenant » (next lesson / jump-in) — Babbel, Speak.
3. Un seul chemin principal linéaire avec progression visible (cercle ou barre) ; pas plus d'un carrousel par écran — Pratt/Headspace, Babbel.
4. Transitions : slide latéral `translateX` + `opacity`, 250–300 ms, easing décéléré à l'entrée `cubic-bezier(0.05,0.7,0.1,1)` et accéléré à la sortie `cubic-bezier(0.3,0,0.8,0.15)` ; fade-through 300 ms entre onglets — Material 3, Val Head.
5. Utiliser l'API View Transitions (iOS Safari 18+, Chrome 154, ≈93 % de couverture) avec repli fade court, et honorer `prefers-reduced-motion`.
6. Bottom sheets (glissement + bouton fermer) pour les choix réversibles ; modal seulement pour paiement, permissions, suppression ; jamais empilés — Dolfy.
7. Bouton « parler » : grand, dans le contenu (pas dans la tab bar), tap-pour-parler par défaut + mode mains libres optionnel avec interruption — HIG, Gemini Live.
8. États vocaux explicites : écoute (onde), réflexion (pulsation ≤ 1 s), parole (onde + bouton mute / sous-titres), erreur micro (instructions iOS/Android) — Gemini, Daily.co.
9. Diffuser voix et texte en synchro, mots qui s'éclairent ; jamais le texte avant la voix — Praktika (plainte), Speak.
10. Corrections après le tour (forme fautive → correcte) + carnet des erreurs récurrentes — lacune commune à Speak, Praktika, Loora.
11. Gérer `NotAllowedError` / `OverconstrainedError` (Safari) avec une page de pré-vérification du micro et un bouton « Autoriser » qui explique la marche à suivre — Daily.co.
12. Paywall annoncé par cadenas sur les leçons premium, déclenché après une première conversation réussie — Pratt/Headspace.
13. Landing : démo jouable sans compte dans le hero, CTA collant bas sur mobile (une ligne + bouton pleine largeur), un plan annuel unique, prix localisé Turquie — Convertica, RevenueCat, FunnelFox.
14. Préférer essai payant court (ex. 1 €/7 j) ou garantie remboursement à l'essai gratuit ; afficher « annulation en un clic » et la politique de confidentialité près du prix — RevenueCat, Balance (critiques).
15. Contraste : texte 4,5:1, titres ≥ 24 px 3:1, composants UI 3:1 dans chaque état ; inputs ≥ 16 px ; cibles 44 pt / 48 dp — WebAIM, Strahl, HIG/Material.
16. Baliser `lang="tr"` sur tout texte turc, choisir une police avec `locl` TRK, tester « İstanbul / ışık / Diyarbakır / fiil » en capitales — Glyphs, Localfonts.
17. Polices : WOFF2, `preconnect`, `font-display: swap` (titres) / `optional` (corps), `size-adjust`, ≤ 2 familles — web.dev.
18. Viser LCP ≤ 2,5 s, INP ≤ 200 ms, CLS ≤ 0,1 au p75 sur Android milieu de gamme ; précharger le premier audio d'Elif pendant l'accueil — CWV, Headspace 2021.

### À éviter
19. Animer autre chose que `transform`/`opacity` (flou `backdrop-filter` animé, parallaxe, ombres animées) et promouvoir des calques en masse — web.dev.
20. Vidéo hero en autoplay lourde ; préférer poster + lecture au tap ou boucle courte — Headspace (GIF), RevenueCat.
21. Séries punitives et compteurs omniprésents ; rendre la série visible sur demande — Pratt/Headspace, UX Collective/Duolingo.
22. Interstitiels « Prêt ? » et limites de durée visibles (type 45 s) qui cassent le flux — Praktika, Loora.
23. Choix de plan sur plusieurs écrans, paliers aux différences floues — Speak (LanguaTalk, ScreensDesign).
24. `text-transform: uppercase`, petites capitales et ligatures discrétionnaires sur du turc — Glyphs.
25. Fabriquer de la preuve sociale (notes, avis) ; montrer plutôt la démo, le visage du fondateur et les conditions d'annulation — RevenueCat (« actively build trust »).
