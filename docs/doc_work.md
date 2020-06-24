# WORKFLOW

Voici comment travailler avec le flow git pour éditer en local le site.

## Prérequis

1. Avoir git sur son PC : https://git-scm.com/downloads (pour vérifier que l'install s'est bien déroulé, on peut lancer une invite de commande et taper `git`).
2. Installer jekyll : https://jekyllrb.com/docs/installation/ (c'est le générateur de site utilisé). (si ça ne marche pas, on peut toujours se référer à https://gist.github.com/arthurattwell/281a5e1888ffd89b08b4861a2e3c1b35 mais c'est bourrin).

## Obtenir le code du site en local sur son PC

1. Choisir le dossier où se trouvera le site. Par exemple, si je veux que le dossier soit dans `Documents/siubiparis_blog` (même si le dossier `siubiparis_blog` n'existe pas encore), alors je dois aller dans le dossier `Documents` avec l'invite de commande (en utilisant `cd`).
2. Une fois dans le dossier `Documents` (pour l'exemple), taper `git clone https://github.com/siubiparis/siubiparis.github.io siubiparis_blog`. Cela téléchargera le code du site en créant un dossier nommé comme le dernier mot de la commande (dans l'exemple : `siubiparis_blog`).
3. Voilà ! 

## Tester le code en local

1. Une fois que le code est en local, on peut le modifier comme bon nous semble sans impacter le site final.
2. Pour tester un changement (comme un nouvel article), alors il faut être dans le répertoire principal du site (`Documents\siubiparis_blog` dans notre exemple) et taper `jekyll serve --watch` dans l'invite de commande à cet endroit.
3. Ensuite, se rendre sur le site `https://localhost:4000` qui fera apparaître le site en local avec le changement.

## Mettre une modification du site testée en ligne

Une fois les changements testés, il est temps de mettre en ligne les modifications.

1. Être dans le répertoire principal du site (`Documents\siubiparis_blog` dans notre exemple) dans l'invite de commande
2. Taper `git add *` pour dire que toutes les modifications effectuées seront dans la changelist.
3. (Facultatif) On peut taper `git status` pour vérifier les fichiers ajoutés.
4. Taper `git commit -m mon_message_de_commit`. Evidemment, on peut changer `mon_message_de_commit`.
5. Taper `git push` pour pousser les modifications finales dans le site en ligne.
6. Attendre quelques minutes le temps que github update la page. Ensuite, on peut voir le résultat en ligne :)
