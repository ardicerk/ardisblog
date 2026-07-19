+++
title = "comment faire un pc en bois"
date = "2026-07-19T11:51:54+02:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
cover = ""
description = "je raconte la fois où j'ai construit mon propre boîtier pc, parce qu'y en avait aucun qui me convenait"
showFullContent = false
readingTime = true
hideComments = false
+++

j'ai _énormèment_ d'e-waste chez moi. il y a 2 ans, j'ai pu changer mon ordinateur principal pour celui d'un pote qui changeait le sien. je pouvais alors enfin donner une retraite bien mérité au bateau de thésée qu'était mon ordinateur. acheté et monté en 2017, sous les conseils achat du jean-baptiste show. les seules choses qui restaient du build original était les 8gb de ram, le disque dur, l'alimentation et le boitier. 

la nouvelle carte mère et son processeur venaient du vieil Acer Predator d'un pote, la nouvelle carte graphique était juste la génération au dessus, lui aussi venant d'un upgrade d'un autre pote. techniquement, il était devenu un amas absurde de silicone, un monstre du dr frankenstein électronique.

au final, avant le changement final d'ordinateur, les specs étaient grossièrement:

```
Intel Core i7-6700
Radeon RX 560
24gb RAM DDR4
3.5TB au total sur 3 HDD (je suis un data hoarder)
```

il méritait enfin une belle retraite, après tant d'effort...

...jusqu'en décembre 2025, où je me suis dit qu'il méritait plutôt une 2ème jeunesse.

déjà, il était terriblement lent. genre: "je prends mon café pendant qu'il s'allume"-lent. le problème venait évidemment du disque dur où était installé windows, qui n'était qu'un hdd bas de gamme en fin de vie. je l'ai changé pour un ssd nvme d'1TB, et là déjà la différence était folle, il était redevenu tout neuf.

il manquait aussi la connectivité wi-fi (évidemment qu'il n'était pas integré à la carte mère, vous pensiez quoi). heureusement, la carte mère avait une entrée m.2, et j'y ai rajouté une carte réseau d'un ordinateur portable qui trainait et qui était voué à la déchetterie. l'écran de cet ordi portable, j'en ai profité pour lui rajouter un contrôleur pour l'utiliser comme moniteur (un tuto existe [ici](https://youtu.be/CfirQC99xPc), même s'il est beaucoup trop fancy à mon gout)

![target](/ardisblog/images/202607/moniteur_avant.jpg)
![target](/ardisblog/images/202607/moniteur_arriere.jpg)
<p style="text-align:center;">oui il est pas aussi "sleek" que dans le tuto du mec</p>


il y avait ensuite la tour, qui était beaucoup trop gros pour ce que c'était. il était logé dans un énorme boitier ATX, le moins cher que proposait PC-OstSchweiz à l'époque (rip au magasin de tech le moins cher du pays). sauf que du coup, il n'avait plus besoin de loger d'hdd, ni de loger une carte mère ATX, puisque celle que j'avais était une mATX.

![target](/ardisblog/images/202607/coolermastern300.jpg)
<p style="text-align:center;">cette grosse tour là</p>

moi, je voulais un ordinateur qui était aussi petit que possible, et aussi _sleek and design_ que possible, comme si c'était un meuble. j'avais pas envie de mettre de l'argent dans un boîtier mATX (dans cette économie???), alors je me suis dit qu'il fallait que je sois ingénieux...

...et je me suis rappelé que j'ai accès à une découpeuse laser à l'epfl.

## Tuto: Comment faire sa propre tour PC

### 1. Apprendre Autodesk Fusion

il existait déjà pas mal de plans de boîtiers à faire chez soi, mais aucun n'arrivait à me convaincre. les plus sleeks demandaient des rallonges de cables PCIe (que j'avais pas envie d'acheter), et de découper des planches d'aluminium (ce que je ne pouvais pas réalistiquement faire). je me suis dit alors que le meilleur choix, c'est le _bois_.

le semestre d'automne, j'ai eu la _chance_ de suivre le cours "Making Intelligent Things" qui, en plus de m'apprendre les notions de sagesse intérieur et de résistence face à l'adversité, m'a permis d'apprendre autodesk fusion (et d'avoir accès, pour le restant de mes études, à une découpeuse laser). je me suis mis alors au Travail. l'heure était au Design.

tout d'abords, il fallait un support sur quoi mettre la carte mère, je ne voulais pas directement la visser sur le boitier pc. j'ai pris alors le support de carte mère de [ce boitier](https://www.colinreay.org/monolith), pour partir sur une bonne base

![target](/ardisblog/images/202607/support-mobo.jpg.png)
<p style="text-align:center;">il se pourrait que j'ai scié la tige de bois du milieu pour faire la place à la backplate du processeur</p>

j'ai désossé mon ordi et mis ses entrailles sur une table, en essayant de trouver le moyen le plus compact possible de tout installer (cw: computer gore)

![target](/ardisblog/images/202607/desossement2.jpg)
![target](/ardisblog/images/202607/desossement1.jpg)

il fallait donc mettre tout ca dans une boite. du coup, j'ai ouvert autodesk fusion, et après une chiées de mesures approximatives, j'en suis arrivé à:

![target](/ardisblog/images/202607/pccase1.jpg)
![target](/ardisblog/images/202607/pccase2.jpg)
<p style="text-align:center;">oui, j'y tenais beaucoup à ce qu'il y ait un lecteur dvd</p>

### 2. Avoir accès à une découpeuse laser à plusieurs dizaines milliers de francs

j'ai choisi comme bois du contreplaqué de bouleau de 6cm d'épaisseur (c'était le moins cher et le plus stylé), et l'heure était maintenant à la découpe laser!!

![target](/ardisblog/images/202607/laser.jpg)

je ne voulais pas faire de joints pour attacher les planches entre elles, j'y suis allé au clou et à la colle à bois: d'abords je percais avec une petite meche le trou qui allait accueillir le clou, et ensuite j'y insérais le clou enduit de colle. surprenament, bien que ca soit peu catholique, ca tenait bien! et ca tient encore aujourdhui!

pour attacher la carte mère au boitier, jy suis allé avec des ecrous collés sur la planche avec de la colle forte

![target](/ardisblog/images/202607/schema.jpg)
![target](/ardisblog/images/202607/ecrous.jpg)
<p style="text-align:center;">et ca tient super bien?? pas eu un probleme alors que je le tiens à la verticale</p>

et comme vous pouvez voir, j'ai aussi mis des joints de porte (oui oui) pour pouvoir facilement accéder à l'intérieur du boîtier

une fois assemblé, je l'ai poncé et vernis, pour quand même lui donner un petit finish et le traiter pour éviter qu'il pourrisse

### 3. Monter le tout

et voici le résultat final

![target](/ardisblog/images/202607/pc1.jpg)
![target](/ardisblog/images/202607/pc2.jpg)
![target](/ardisblog/images/202607/pc3.jpg)
![target](/ardisblog/images/202607/pc4.jpg)

malheureusement, j'ai mal pris en compte l'épaisseur du bois, je n'ai pas pu installer le lecteur dvd là où je voulais, je l'ai alors caché à l'intérieur

![target](/ardisblog/images/202607/pc5.jpg)
![target](/ardisblog/images/202607/pc6.jpg)

et comparé à l'ancienne tour, il est un peu plus petit, mais pas aussi petit que j'aurais voulu, mais c'est pas grave

le bouton est un morceau de bois collé sur un simple bouton pressoir, qui est soudés à deux cables pour faire la liaison des 2 pins de démarrage de la carte mère

et niveau températures, le ventilateur en plus aide énormèment. en jeu, l'ordi reste a des températures raisonnables

et du coup, cet ordinateur est techniquement la combinaison de 6 ordinateurs différents

du coup, voila! maintenant, faut encore que je lui trouve une utilité, à cet ordi.

<script src="https://utteranc.es/client.js"
        repo="ardicerk/ardisblog"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>