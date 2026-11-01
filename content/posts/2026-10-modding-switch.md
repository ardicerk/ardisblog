+++
title = "comment hacker sa switch lite grâce à lidl"
date = "2026-10-31T22:59:28+01:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
cover = ""
description = "imaginez faire de la micro-soudure sur une console de jeu avec des outils lidl, c'est aussi terrifiant que vous le pensez"
showFullContent = false
readingTime = true
hideComments = false
draft = false
+++

cela va faire un peu plus de 4 ans que j'essaie de lutter contre le fait de doomscroller dans le train. pour aller à l'uni, je dois faire 30 minutes (ressenti 2h40) de train aller, puis 30 minutes retour, temps durant lequel je n'arrive pas à faire grand chose mis à part ouvrir instagram, scroller, puis regretter d'avoir ouvert instagram. j'ai pas particulièrement envie d'étudier durant ce trajet, ayant soit la tête dans le cul, encore entrain de me réveiller (à l'aller) ou au bord du sommeil (au retour). 

j'ai essayé des trucs, j'avais une grande période Tetris (qui était devenu mon jeu "braindead", vous savez, ce jeu que vous jouez quand vous voulez débrancher votre cerveau, un peu comme candy crush, 2048, ces jeux de puzzle sur mobile) (bon après je trouvais l'appli mobile de tetris tellement insupportable que j'avais fini par installer un émulateur gameboy pour jouer à la version de 1989).

j'avais fini par ressortir ma vieille 3DS moddée, mais j'avais l'impression que l'ayant depuis 15 ans (putain déjà), j'avais fini par épuiser les jeux qui m'intéressaient de toute la bibliothèque de la console. à vrai dire, j'ai jamais été un grand fan de pokemon ou d'autres rpg, du coup bon... on fait vite le tour. (dites vous que je me faisais tellement chier que j'avais installé nintendogs), je me suis dit qu'il faudrait que je trouve autre chose

il y a le steamdeck et toutes ces consoles portables sous android, mais le 1er est beaucoup trop cher et trop grand pour ce que je voulais en faire (arreter de me faire chier dans le train), et ces consoles sous android étaient toutes moins puissantes que mon téléphone (un samsung galaxy milieu de gamme qui a deja 2 ans) (ca + y a aucun bon revendeur de confiance en suisse et Je Refuse Catégoriquement de faire une commande à +100frs sur aliexpress, par principe). (meme si, entre nous, j'adore visuellement le ayn thor mais vazy vous avez vu le prix de ces trucs)

du coup, jme suis dit, une petite console moderne pas trop cher? et si je me prenais une nintendo switch lite d'occasion?

après de longues recherches sur facebook marketplace, vinted et les magasins d'occasion qu'offre le Grand Lausanne, j'avais fini par trouver cette petite switch lite jaune pétant au hop'n'cash (anciennement cash converter) de lausanne vers Chauderon (je me demande sincèrement comment ils ont fait pour perdre leur license de se nommer Cash Converter) (quoique, je préfère pas savoir.).

![targets](/ardisblog/images/202610/switchlite.jpg)
<p style="text-align:center;">regardeeez elle est jaune</p>

elle est pas dans un super état, avec un petit bout de plastique explosé, mais pour une switch à 70frs sans joy-con drift, je reste content de ma trouvaille

maintenant! faut bien jouer à des jeux dessus! ...et vous pensez que je vais payer 60frs mes jeux?

.

.

.

.

ha.

> DISCLAIMER: faire des modifications sur sa switch est DANGEUREUX, ce qui suit est une manipulation faite par un PROFESSIONNEL (ptdrrrrrrrrr si vous me voyiez)
>
> par contre /srs y a une chance non-nulle (même assez moyenne voir haute si c'est du hardmod) de bricker votre console (la rendre aussi utile qu'une brique) si vous la modifiez, du coup si vous voulez le faire, soyez sûr-es de savoir ce que vous faites. je vous aurais averti.
>
> ah et installez seulement des jeux que vous avez acheté avec vos propres dumps haha ouai ne téléchargez surtout pas illégalement ouaaaaai je vous en supplie nintendo portez pas plainte jai pas encore mis ma daronne à l'abri oh putain ils sont à ma porte

# tuto: comment modder sa switch

le homebrewing, c'est le développement de logiciels non-officiels et lancé sans autorisation du constructeur du matériel sur lequel il est lancé

et nintendo et sa communauté homebrew, c'est un splendide "je t'aime, moi non plus".

j'ai toujours eu une petite fascination sur la manière dont la communauté arrive à trouver des failles dans ces consoles, comme la wii qui fût crackée [grâce à une pincette en métal dans son lecteur dvd](https://youtu.be/4BlpONgj74A) ou le homebrew sur 3ds qui était [un énorme bras de fer entre les constructeurs de cartouches R4 et la communauté libre](https://youtu.be/ImR-TdDAIJE) (vraiment, ces histoires sont fascinantes)

et la switch? sa faille a été trouvée avec [un trombone](https://youtu.be/xQmN-cxg21M).

et c'est incroyable, une faille hardware qui ne peut pas être fix, et super simple à utiliser! ca serait dommage que nintendo remarque et corrige cette erreur sur tous les modèles construits après 2018...

...évidemment que ca a été fix à la sortie de la switch lite.

mais c'est pas grave! il doit bien y avoir un moyen de modifier le code de démarrage pour pouvoir lancer un firmware modifié!...

...en soudant directement une puce sur le processeur pour le faire halluciner au démarrage, bien sûr...?

### Étape 1: Commander sur aliexpress

bon. dès l'achat, j'avais déjà accepté le risque que ça implique d'essayer de souder une puce sur une carte mère et un processeur aussi minuscules que celles dans la switch lite, en me disant que sur un malentendu, ça pourrait _peut-être_ passer. appelez ca être délirant ou de l'égo masculin mal placé, mais on sait jamais!! on sait rien tant qu'on essaie pas!!! 

alors, comme le conseillait [le guide](https://guide.nx-modchip.info/), j'ai commandé ma Picofly (8frs, livraison incluse si mes souvenirs sont bons), et j'ai attendu patiemment mon colis.

et il est arrivé.

et putain qu'est-ce que c'est minuscule.

![targets](/ardisblog/images/202610/puce_switch.jpg)
<p style="text-align:center;">dans le sens des aiguilles d'une montre, en commençant à 12h, la fiche à souder sur la carte mère de la switch lite, la même pour la switch "normale", celle pour la switch oled, la fiche à souder sur le System-on-Chip, l'adapteur usb-c pour update le firmware de la puce, et la puce en elle-même</p>

### Étape 2: Sortir son fer à souder Parkside de Lidl

le guide dit précisement "vous devez avoir de l'expérience en micro-soudure". or, mon expérience en soudure se limitait sur des jumper cables reliant des arduinos, et quelques pcb d'entraînement bien assez larges. mais alors, micro?? la seule chose micro ici c'est- non. je pensais que la switch lite me donnerait suffisament d'espace de travail, mais je vous avoue qu'une goutte de sueur a coulé de mon front en voyant la taille de cette puce.

j'ai pris mon courage à deux mains, et j'ai sorti mon matériel de "bricolage tech", entièrement issu du rayon bricolage et jardinage de lidl. ce n'est pas une vanne.

#### aparté lidl

vous connaissez peut-être la sous-marque Parkside de lidl, qui est un peu devenu la marque m-budget/eco+ du monde du bricolage, et qui a fini par avoir sa petite communauté de fidèles. et depuis un petit moment, ils ont commencés à faire des outils aussi destinés à la tech, surtout au niveau démontage et réparation. ils avaient sorti une fois un set d'embouts de précision pour vraiment pas beaucoup

et aldi aussi s'y est mis, en sortant un vrai kit de réparation pour téléphones à seulement 6frs, avec quand même du PH000, T4 à T10, et surtout un embout Y2, ce qui tombait à pic pour la switch lite, ce qui, avec le kit de lidl, me donnait une vraie trousse à outil, pour une fraction du prix de celle d'ifixit

et lidl avait aussi sorti une station de soudure à 13frs (!!!!), ce qui me donnait de quoi essayer de me lancer dans ce puçage de la switch

![targets](/ardisblog/images/202610/setup.jpg)
<p style="text-align:center;">#bricolage</p>

est-ce que ce sont des outils de qualité? ...bof, la pince du set parkside a tendance à se déformer facilement, et le metal utilisé pour les embouts d'aldi et lidl est pas dingue, mais putain pour le prix que c'est, c'est une dinguerie folle que ça marche, pareil pour le fer à souder, et ca en vaut chaque centime. (je suis même pas payé pour dire ça)

#### fin de l'aparté lidl

après beaucoup (trop) de temps à démonter cette switch, j'avais enfin réussi à atteindre la carte mère et le system-on-chip, désormais nu et nettoyé de toute sa pâte thermique avec le peu d'alcool isopropylique qu'il me restait (si vous voyiez l'état du plastique c'est un carnage, j'avais mal lu le tuto de démontage il restait 2 vis j'ai failli tout casser)

![targets](/ardisblog/images/202610/buro.jpg)
<p style="text-align:center;">#bricolage2</p>

et là, je continue de regarder le guide et je vois dans la vraie vie la taille des points de soudure. et je les compare à la taille de la pointe de mon fer à souder. je me retrouvais à devoir utiliser des gants de boxe pour faire de la broderie. et je re-regarde la liste des "requirements" du guide.
```
Requirements:
- A soldering iron with a small(er) tip
- Soldering tin (leaded is recommended, unleaded will 
  work depending on your skill level)
- Good quality flux
- A microscope (optional but recommended)
[...]
```

j'ai une pointe classique, mon étain à souder est sans plomb, je n'ai pas de flux et encore moins un microscope. qu'est-ce qu'il peut mal se passer????

![targets](/ardisblog/images/202610/buro2.jpg)
<p style="text-align:center;">j'adore la fumée de soudure</p>

pour la petite histoire, ces 2 images viennent d'une tentative d'essayer de faire un timelapse de toute la manoeuvre, mais la batterie de ma caméra m'a lâché au plein milieu du soudage et j'étais bien trop concentré à essayer de ne pas faire exploser la batterie en lithium de la switch avec ma pointe à 400°C.

après _beaucoup_ de sueur, j'avais enfin réussi à souder la fiche sur les 2 pins du SoC et sur les autres points de la carte mère (pour accéder au flux de la carte microsd ainsi qu'à 3 volts pour s'alimenter, si j'ai bien compris?)

![targets](/ardisblog/images/202610/switch_mobo.jpg)
<p style="text-align:center;">l'état de la carte mère après mon passage</p>
 
![targets](/ardisblog/images/202610/soc.jpg)
<p style="text-align:center;">et l'état de la SoC nvidia tegra</p>

### Étape 3: Prier.

il ne restait plus qu'à rebrancher la batterie à la carte mère, allumer la switch et espérer que ca marche. je l'ai donc rebranché et allumé...

...et rien.

je débanche, rebranche, redébranche, rerebranche, je panique légèrement, et il se rallume enfin!!...

...avec le logo de la nintendo switch, sans faire apparaître le menu de la puce.

mais ça voulait dire que la console n'était pas morte!! et je vois que la puce fait des signes de vie avec sa led, ce qui voulait dire que mes soudures aux points pour les 3 volts étaient bonnes (et tant mieux, parce que c'était les pires), et qu'il fallait juste retravailler _tout le reste._

et après plusieurs tentatives...

![targets](/ardisblog/images/202610/imin.jpg)
<p style="text-align:center;">La puce marche.</p>

après un énorme soupir de soulagement, j'ai remis de la pâte thermique toute neuve, remonté entièrement cette switch et je suis allé chercher une carte microsd elle aussi toute neuve

### Étape 4: Installer le custom firmware

pouvoir contourner le bootloader (le programme de démarrage de la switch), c'est bien, mais mettre un autre bootloader, c'est mieux!

j'ai alors simplement suivi le reste du guide pour tout l'aspect software en mettant en place le nouveau bootloader (hekate) et le custom firmware (Atmosphère). c'est un peu comme un autre système d'exploitation

![targets](/ardisblog/images/202610/hekate.jpg)
<p style="text-align:center;">Hekate, tournant sur cette switch lite</p>

et après de longs temps de chargements et d'attente d'installations...

![targets](/ardisblog/images/202610/homebrew.jpg)
<p style="text-align:center;">le menu du Homebrew Launcher, lancé depuis Atmosphère</p>

et, depuis là, il suffit juste d'installer n'importe quel fichier .nsp avec Goldleaf, et c'est fini...

...fichiers trouvés légalement bien sûr haha ouai

#### aparté guides

j'aimerais quand même donner un shoutout aux guides de modding qui sont vraiment de qualité et aux scripts d'installation, qui ensemble permettent à des gens pas forcèment tech-savy de faire des choses super techniques et aussi simple à installer. 

c'est le [3ds Hacks Guide](https://3ds.hacks.guide/) qui, me semble, a été le 1er, a lancé et uniformisé ce types de guides, et qui fait faire des choses quand même très technique (on parle quand même d'override un bootloader à partir d'une faille du processeur de compatibilité de la nintendo ds), et [celui pour la switch](https://switch.hacks.guide/) ne fait pas exception dans sa qualité, l'ayant utilisé

si vous voulez vous aussi modder vos consoles nintendo, je vous conseille largement de passer par ces guides de [hacks.guide](https://hacks.guide/), écrit par la communauté de Nintendo Homebrew, plutôt qu'avec des tutos youtube qui pourraient être out-dated

#### fin de l'aparté guides

### est-ce que tu conseillerais cette manip' à quelqu'un d'autre?

franchement, je sais pas. je reste convaincu que j'ai été gracié par le Tout-Puissant et que c'est pas normal que ça ait marché. ca va faire 4 jours que je l'ai pucée, et la switch marche toujours. vous verrez une update ici si un jour mes soudures lâchent. mais si vous avez le matos et l'expertise, si moi j'ai réussi, j'pense que vous pourriez aussi réussir.

sur ce, je vais aller me refaire super mario galaxy 2 dans le train (je ne vais PAS payer 70 balles pour un jeu qui a 16 ans.)

(putain comment ca mario galaxy 2 a 16 ans)

<script src="https://utteranc.es/client.js"
        repo="ardicerk/ardisblog"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>