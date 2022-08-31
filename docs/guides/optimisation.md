# Optimisation de Minecraft

Optimiser Minecraft quand on a un PC pas ouf est indispensable. Pour ce faire, il est possible d'installer des mods (bouts de code additionnels créés par la communauté pour modifier le jeu) qui vont fluidifier le jeu et lui permettre de tourner correctement. Il est également possible de réaliser quelques autres optimisations fort sympatique. Suivez les différentes parties comprises dans ce guide pour exploiter le plein potentiel de votre machine !  

!!! tip "MultiMC"

    MultiMC est launcher alternatif crée par et pour la communauté. Il permet la création d'instances séparées très simplement et facilite grandement l'exécution du guide ci-dessous. En effet, avec MultiMC, il est bien plus simple d'installer Fabric par exemple (un seul boutton à appuyer !) ou encore de gérer ses mods (chaque version à son propre dossier `mods`, de même que son propre dossier `resourcepacks`, etc.). Avec MultiMC, on ne s'emmêle plus les pinceaux ! L'installation de ce launcher est très simple: suivez le [guide](multimc.md), et facilitez-vous la vie !

## Fabric et les mods

Fabric est ce qu'on appelle un modloader. C'est un programme qui va permettre d'ajouter facilement des mods au jeu. Ce n'est pas le seul, mais c'est celui qui est le plus en vogue en ce moment: il est facile à prendre en main pour les moddeurs et il est open-source ! Dans cette partie nous verrons comment l'installer, puis comment ajouter des mods visant à optimiser le jeu.

!!! question "D'autres modloaders ?"

    Oui, il en existe d'autres. Fabric est relativement récent, et il est encore en concurrence avec un autre rival bien connu: Forge. Si vous souhaitez modder lourdement votre jeu avec une plétore de mods et que votre machine le permet: c'est vers lui qu'il faudra plûtot se tourner, même si Fabric rattrape petit à petit son retard. Forge existe depuis 2011 et est le support d'un nombre tout bonne stratosphérique de mods tous plus variés les uns que les autres, certains étant devenu presque cultes.

1. **Télécharger l'installateur de fabric.** Si vous avez déjà installé Fabric auparavant, vous avez surement cet installateur qui traîne quelque part: c'est un fichier executable, il doit sûrement être dans le dossier `Téléchargements`. Si vous l'avez, ignorez cette première étape. Sinon, [téléchargez-le](https://fabricmc.net/use/).
 
2. **Installer Fabric.** Double-cliquez sur l'installateur de Fabric: pour "Version des mappings" sélectionnez la version de Minecraft que vous souhaitez utiliser: le serveur ChômageLand tourne sur Minecraft 1.18.1 actuellemment. Pour le reste ne changez rien.  

    !!! Attention
        
        Veillez à bien installer Fabric Client et non Server (voir barre de menu en haut de la fenêtre d'installateur).

    Cliquez sur "Installer" et suivez les instructions.  
 
3. **Vérification.** normalement si tout s'est bien installé, une nouvelle option est apparu dans votre launcher (le logiciel qui lance Minecraft): dans celui-ci quand vous le lancez, en bas, vous pouvez sélectionner la version de Minecraft: une ligne du genre `fabric-xxx...` est apparu: ça à fonctionné ! Ne lancez pas encore cette version cependant, vous verrez pourquoi à l'étape 5.
 
4. **Téléchargement des mods d'optimisation.** Téléchargez les mods nécéssaires à l'optimisation, et gardez les fichiers téléchargés précieusement. Soyez attentif à la version pour laquelle ils sont destinés.

    !!! info

        Les mods Phosphore et Starlight sont incompatibles entre eux. Si vous êtes en version 1.16.5 ou antérieur, utilisez Phosphore. Sinon, utilisez Starlight.

    | Mod | Description | Téléchargement |
    |:---:|:------------|:---------------|
    | Lithium | Optimisation générale | [1.16.5](https://modrinth.com/mod/lithium/version/mc1.16.5-0.6.6) / [1.18.1](https://modrinth.com/mod/lithium/version/mc1.18.1-0.7.8) / [1.19.2](https://modrinth.com/mod/lithium/version/mc1.19.2-0.8.3) |
    | Sodium | Optimisation générale | [1.16.5](https://modrinth.com/mod/sodium/version/mc1.16.5-0.2.0) / [1.18.1](https://modrinth.com/mod/sodium/version/mc1.18.1-0.4.0-alpha6) / [1.19.2](https://modrinth.com/mod/sodium/version/mc1.19.2-0.4.4) |
    | Starlight (v1.17+) | Refonte du moteur de rendu de la lumière | [1.18.1](https://modrinth.com/mod/starlight/version/1.0.0%2B1.18.0-1.18.1) / [1.19.2](https://modrinth.com/mod/starlight/version/1.1.1%2B1.19) |
    | Phosphore (v1.16.5) | Optimisation du moteur de rendu de la lumière | [1.16.5](https://modrinth.com/mod/phosphor/version/mc1.16.2-0.8.0) |
    | LazyDFU (optionnel mais conseillé) | Diminution du temps de lancement de Minecraft | [1.16.5](https://modrinth.com/mod/lazydfu/version/0.1.1) / [1.18.1](https://modrinth.com/mod/lazydfu/version/0.1.2) / [1.19.2](https://modrinth.com/mod/lazydfu/version/0.1.3) |
 
5. **Installation des mods.** Appuyez simultanément sur les touches :material-microsoft-windows: et `R`: une petite fenêtre apparaît: entrez `%appdata%` et appuyez sur `Ok`. Le dossier `AppData` s'ouvre: dans celui-ci, allez dans le dossier `.minecraft` puis dans `mods`: dans ce dossier, mettez-y les fichiers que vous avez téléchargés à l'étape précédente. Fermez le dossier, et le launcher si il était encore ouvert.
   
    !!! attention

        Il ne peut y avoir dans ce dossier `mods` que des mods pour une seule version ! C'est-à-dire que vous ne pouvez pas avoir des mods pour Minecraft 1.16.5 et en même temps des mods pour Minecraft 1.17.1 par exemple. Si vous tentez de lancer le jeu avec tout ça, il plantera. Si vous voulez jouez dans une version, mettez les mods de cette version dans le dossier `mods` et enlevez les autres ! N'oubliez pas de faire cette manip à chaque fois que vous changez de version. Si vous trouvez ça relou, essayez [MultiMC](multimc.md).
 
6. **Fin.** Normalement, les 3 mods ont bien étés installés ! En lançant le jeu, veillez-bien à sélectionner la version "fabric-xxx-...".

## Autres optimisations

1. **Augmenter la RAM.** De base, cette saloperie de launcher Minecraft officiel ne s'alloue que 1GB de RAM. C'est de la merde. On va plutôt passer ça à 2GB de RAM minimum. Pour ce faire: dans le launcher allez dans `Configurations` en haut, sélectionnez le profil dont vous voulez augmenter la RAM, sélectionnez les 3 petits points puis "Modifier". Une fois dans le menu "Modifier la configuration", cliquez sur `Plus d'options`. Dans la zone de texte `Arguments JVM`, modifier `Xmx1G` par la valeur de RAM souhaitée. Pour 2GB de RAM,
remplacer par `Xmx2G`. Une fois fait, cliquer sur `Enregistrer`.

    !!! attention

        Ne pas allouer plus de la moitié de la RAM du PC. Si votre PC est doté de 4GB de RAM, allouer au maximum 2GB.
    
    !!! attention

        Répéter cette opération à chaque nouveau profil crée ! C'est-à-dire à chaque fois que vous installez Fabric.