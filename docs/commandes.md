# Commandes

De nombreuses commandes sont accessibles depuis le chat (touche `T`). La plupart ne sont accessibles que depuis le monde créatif. Pour plus d'informations sur les commandes listées, se référer au [Wiki Minecraft](https://minecraft.fandom.com/fr/wiki/Commandes).

??? info "Paramètres de commandes"

    Les commandes ont quasiment toutes des paramètres, en voici la syntaxte:  

    | Syntaxe | Signification |
    |:-------:|:--------------|
    | `<param>` | Paramètre requis |
    | `(choix1|choix2|...)` | Paramètre requis parmis une liste |
    | `[param]` | Paramètre optionnel |
    | `[choix1|choix2|...]` | Paramètre optionnel parmis une liste |

??? info "Coordonnées"

    Les coordonnées sont toujours renseignées au format `X Y Z`. Il est possible de renseigner des coordonnées relatives grâce au symbole `~`. `~ ~ ~` correspond à la position du joueur, pour spécifier un décalage par rapport à celle-ci: `~dX ~dY ~dZ`.  
    Exemple: `~ ~3 ~-64` correspond à `XduJoueur / YduJoueur+3 / ZduJoueur-64`.  
    Coordonnées absolues et relatives peuvent être mêlées.  
    Exemple: `2160 128 ~30`  

??? info "ID"

    Les noms des blocs, items, entitées, biomes, etc. sont à renseigner sous la forme `minecraft:nom` où `nom` est l'ID nominal de l'élément. Il s'agit en général de son nom en anglais.  
    Exemple: `minecraft:stone` correspond à la roche, `minecraft:pig` au cochon.  
    Pour avoir l’ID d’un élément: chercher cet élément dans le [Wiki Minecraft](https://minecraft.fandom.com/fr/wiki/Minecraft_Wiki), regarder dans le carton d’information en haut à droite de la page, voir “ID nominal”.

??? info "Sélecteurs"

    Quand un joueur où une entité est demandée, il est possible de les remplacer par un sélecteur.  

    | Sélecteur | Signification |
    |:---------:|:--------------|
    | `@p` | Cible le joueur le plus proche. |
    | `@r` | Cible un joueur au hasard. |
    | `@a` | Cible tout les joueurs. |
    | `@e` | Cible toutes les entités, joueurs compris. |

    Les sélecteurs peuvent être complétés d'un ou plusieurs arguments. Pour plus d'infos, voir la [page Wiki associée](https://minecraft.fandom.com/fr/wiki/Commandes#Arguments_de_s%C3%A9lecteurs).  
    Exemple: `@e[type=minecraft:creeper]` cible tout les creepers.  

## Multiverse

Voir [section Multiverse](multiverse.md#commandes).  

## Monde survie  

* `/tpa <joueur>`  
Envoie une demande de téléportation à un joueur.  

* `/tpahere <joueur>`  
Envoie une proposition de téléportation sur soi à un joueur.  

* `/tpahereall`  
Envoie une proposition de téléportation sur soi à tout les joueurs.  

* `/tpatoggle [joueur]`  
Autorise/interdit les demandes de téléportations à soi, possibilité de paramétrer pour chaque joueur.  

* `/tpaccept` | `/tpdeny`  
Accepter/refuser la demande de téléportation à soi.  

* `/tpcancel [joueur]`  
Annule la demande de téléportation à un joueur.  

## Monde créatif

* `/fill <pos1> <pos2> <bloc> (destroy|hollow|keep|outline|replace)`  
Remplie la zone spécifiée par un type de bloc. Le remplissage varie selon le mode. `<pos1>` et `<pos2>` désignent deux coins opposés d'une zone cubique.  

* `/locatebiome <biome>`  
Localise le biome spécifié le plus proche.  

* `/gamemode (survival|creative|spectator|adventure)`  
Change le mode de jeu.  

* `/give <receveur> <item> <quantité>`  
Donne un item à quelqu'un.  

* `/setblock <pos> <bloc>`  
Fait apparaître un bloc.  

* `/summon <entitée> <pos>`  
Fait apparaître une entité.  

* `/mv modify (set|add) time <temps>` ou `/mv modify set time (day|night|noon|midnight)`  
Modifie l'heure du jeu. `<temps>` est une heure à spécifier avec ou sans unité. Unités disponibles: `d` pour jour, `s` pour secondes. Sans unité: temps en ticks (1/20e de seconde), un jour Minecraft durant 24000 ticks.  
Exemples: `/mv modify set time 12000` est equivalant à `/mv modify set time 0.5d`.  

* `/tp [cible] <destination>`  
Téléporte la cible vers une destination (joueur, entité, position).  

* `/mv modify set weather (true|false)`  
(Des)active les précipitations (pluie, neige, orage).  


