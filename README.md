# Flore du Québec

Ce dépôt contient les comptes-rendus pour toutes les espèces présentées sur le site de la Flore du Québec. Les comptes-rendus sont organisés par famille, puis par genre. Pour chaque espèce, l'information est contenue dans un seul fichier _markdown_ (`.md`) portant le nom de l'espèce (e.g. _Abies_balsamea.md_). Le format `markdown` facilite la mise en forme de texte en vue de l'intégration dans une page web.

## Structure du fichier `.md`

### Section photos

Les photos sont un élément très important des comptes-rendus. Si les photos sélectionnées sont boien choisies (et si de bonnes photos sont disponibles), il est souvent possible de rapidement se faire une bonne idée de l'apparence et des éléments servant à identifier une espèce. Voici quelques critères à garder en tête lors de la sélection des photos:

- La première photo sert à représenter l'espèce sur le site. Cette photo doit être le plus représentatif possible de ce qu'un observateur peut voir lorsqu'il rencontre l'espèce pour une première fois
- Les photos suivantes devraient permettre de se faire une bonne idée de l'apparence d'une espèce à différents niveaux (aspect général, inflorescence, photos macros des fleurs, des fruits, photo de plus loin illustrant un parterre de l'espèce, etc.)
- Idéalement, les photos devraient illustrer les critères permettant l'identification

Toutes les photos proviennent de la plateforme iNaturalist et sont disponibles publiquement. Pour cette raison, il est impératif de sélectionner des photos ayant une license permettant leur utilisation. **Les photos pouvant être utilisées ont obligatoiremnt une licence CC0, CC-BY ou CC-BY NC**. Ces licences permettent une utilisation libre et non-commerciale dans le mesure où l'auteur de la photo est crédité. Les photos n'ayant pas une de ces licences seront rejetées.

#### Comment lister les photos?

La première partie du fichier `.md` contient les urls vers les photos qui sont présentées sur le site. Par exemple, le code suivant indique les photos à utiliser pour [_Cinna arundinacea_](https://github.com/frousseu/floreduquebecsp/blob/main/Esp%C3%A8ces/Poaceae/Cinna/Cinna_arundinacea.md). Plus spécifiquement, le code suivant indique que les photos 1, 3, 5 et 13 de l'observation iNaturalist [195220528](https://www.inaturalist.org/observations/195220528) doivent être utilisées, puis les photos 1 et 4 de l'observation [195220524](https://www.inaturalist.org/observations/195220524), la 5e photo de l'oservation [195226187](https://www.inaturalist.org/observations/195226187) et finalement la 4e photo de l'observation [195708914](https://www.inaturalist.org/observations/195708914). **Un nombre maximal de 8 photos seront utilisées et elles seront présentées dans l'ordre donné**. Il est primordial de respecter l'ordre voulu et la syntaxe présentée ici. À noter que si plusieurs photos proviennent d'une même observation, il faudra répéter les urls si les photos ne se suivent pas (_e.g._ 2 photos peuvent provenir d'une même observation avec la 1ère photo listée en premier et la 2e photo listée en 7e position) 

```
<!--

1-3-5-13-https://www.inaturalist.org/observations/195220528
1-4-https://www.inaturalist.org/observations/195220524
5-https://www.inaturalist.org/observations/195226187
4-https://www.inaturalist.org/observations/195708914

-->

```

À noter que cette section est circonscrite par les caractères `<!--` et `-->` pour éviter l'intégration des adresses dans le site. Ces caractères doivent être présents en tout temps dans le fichier `.md`.

### Section description

La seconde partie du fichier `.md` contient le compte-rendu de l'espèce qui apparaîtra sur le site internet. Les titres sont précédés par `##` pour la formatin du titre. Bien que les titres puissent être modifiés, il est impératif de conserver ces titres pour assurer l'uniformité du site. S'il n'y a aucune information pour une section, il est préférable de laisser un tiret `-` suite au titre. 

#### Traits distinctifs

Ici, on trouve une liste à points des traits distinctifs de l'espèce ou des éléments clés pour repérer et reconnaître l'espèce sur le terrain. En d'autres mots, que remarque-t-on de particulier chez cette espèce par rapport aux autres semblables? Pour cette partie, on sépare les éléments de la liste à points par des tirets `-`. Voir notamment en exemple le compte-rendu pour [_Cinna arundinacea_](https://github.com/frousseu/floreduquebecsp/blob/main/Esp%C3%A8ces/Poaceae/Cinna/Cinna_arundinacea.md?plain=1). 

#### Espèces semblables

Ici, on énumère les critères à regarder pour différencier cette espèces des autres espèces semblables. L'idéal est de cibler les espèces qui sont les plus semblables et de ne pas se perdre dans la description des autres espèces qui sont clairement différentes si on regarde attentivement les photos.

#### Habitat

Ici, on trouve une description sommaire de l'habitat et possiblement de la répartition de l'espèce. On peut se baser sur l'expérience personnelle.

#### Commentaires

Finalement, est-ce qu'il y a des remarques à faire pour l'espèce notamment en lien avec la distribution, la taxonomie, le statut ou en lien avec d'autres éléments intéressants concernant l'espèce? On peut aussi discuter des sous-espèces ou des variétés ou de certaines particularités de l'espèce.

## Comment contribuer ?

Pour contribuer, il faudra d'abord vous créer un compte [GitHub](https://github.com/). GitHub est une plateforme principalement destinée à héberger du code et à la collaboraion. Par l'utilisation de [Git](https://fr.wikipedia.org/wiki/Git), elle permet également d'assurer un suivi des modifications de fichiers et de quantifier les modifications sur ces fichiers. 

À noter que l'intégration des modifications au site ne sont pas automatiques. Elles doivent d'abord être approuvées par un membre de l'équipe de révision. Pour l'intégration des photos sélectionnées, un script doit également être utilisé pour récupérer les photos et effectuer la mise à jour.

### À partir de la plateforme en ligne

La façon la plus simple pour éditer le contenu pour une espèce est d'utiliser le bouton *Edit this file* (le petit icône de crayon) sur la page de l'espèce pour proposer directement sur GitHub des changements au texte ou aux figures. Par la suite, il faudra cliquer sur le bouton vert *Commit changes* (en haut à droite) pour proposer les changements. Dans la plupart des cas, une branche (*fork*) sera créée sur votre compte GitHub à partir de laquelle vous pourrez faire un *Create pull request* pour proposer d'intégrer les changements aux site. Ce processus peut paraître très complexe la première fois, mais après quelques fois, cela devrait vous paraître beaucoup plus facile. À noter que les changements que vous proposerez devront être approuvés par un membre de l'équipe de révisions. Ceci permettra notamment de s'assurer de l'unformités du contenu et de repérer d'éventuelles erreurs de syntaxe *markdown* ou d'orthographe. 

Si vous êtes un contributeur régulier, vous pourriez également avoir les droits pour proposer ou intégrer directement vos modifications sur le site sans passer par le processus de *fork* (création d'une branche sur votre compte) ou de *pull request*.  

### À partir d'un éditeur de texte





