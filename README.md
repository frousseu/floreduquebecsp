# Flore du Québec

Ce dépôt contient les comptes-rendus pour toutes les espèces présentées sur le site de la Flore du Québec. Les comptes-rendus sont organisés par famille, puis par genre. Pour chaque espèce, l'information est contenue dans un seul fichier _markdown_ (`.md`) portant le nom de l'espèce (e.g. _Abies_balsamea.md_). Le format `markdown` facilite la mise en forme de texte en vue de l'intégration dans une page web.

## Structure du fichier `.md`

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

La seconde partie du fichier `.md` contient le compte-rendu de l'espèce qui apparaîtra sur le site internet. Les titres sont précédés par `##` pour la formatin du titre. Bien que les titres puissent être modifiés, il est impératif de conserver ces titres pour assurer l'uniformité du site. S'il n'y a aucune information pour une section, il est préférable de laisser un tiret `-` suite au titre. 

## Comment contribuer ?

Pour contribuer, il faudra d'abord vous créer un compte [GitHub](). GitHub est une plateforme principalement destinée à héberger du code et à la collaboraion. Par l'utilisation de [Git](), elle permet également d'assurer un suivi des modifications de fichiers et de quantifier les modifications sur ces fichiers. 

La façon la plus simple pour éditer le contenu pour une espèce est d'utiliser le bouton *Edit this file* (le petit icône de crayon) sur la page de l'espèce pour proposer directement sur GitHub des changements au texte ou aux figures. Par la suite, il faudra cliquer sur le bouton vert *Commit changes* (en haut à droite) pour proposer les changements. Dans la plupart des cas, une branche (*fork*) sera créée sur votre compte GitHub à partir de laquelle vous pourrez faire une *Pull request* pour proposer d'intégrer les changements aux site. Ce processus peut paraître très complexe la première fois, mais après quelques fois cela devrait vous paraître beaucoup plus facile. À noter que les changements que vous proposerez devront être approuvés par un membre de l'équipe des réviseurs. Ceci permettra notamment de s'assurer de l'unformités du contenu et de repérer d'éventuelles erreurs de syntaxe *markdown* ou d'orthographe. Si vous êtes un contributeur régulier, vous pourriez également avoir les droits pour intégrer directement vos modifications sur le site sans passer par le processus de *fork* ou de *pull request*.  



À que les changements proposés

### À partir de la plateforme en ligne




### À partir d'un éditeur de texte



## Section photo

## Section Description


