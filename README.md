# H1 Exercice 2
Manuel:
1. La commande which permet de retourner le chemin de la commande.
2. On utilise la commande man -k 'option' pour trouver les endroits ou le mot option est utilisé
3. On quitte le manuel en appuyant sur la touche q
4. On utilise la commande man 6 'intro' pour aller au début de la section 6, la section parle de jeux.

Navigation:
1. on utilise la commande cd /var/log pour ce déplacer dans ce dossier
2. On utilise cd .. qui nous fait retourner un dossier en arrière.
3. On utilise cd ~ pour retourner au dossier personnel.
4. On utilise cd – pour retourner au dossier précèdent
5. Nous n’avons pas les permissions pour aller dans le dossier root
6. La commande cd est interne a bash, il n'est pas associé à un PATH et n'est donc pas retrouvé.
7. On utilise mkdir pour créer les dossier, touch pour créer les fichier et cd pour se déplacer dans les dossiers
8. Le fichier est bien supprimé avec ‘rm’ pour les fichier et la commande 'rm' ne permet pas de supprimer les dossiers.
9. Pour supprimer les dossiers il faut utiliser la commande 'rmdir'
10. On ne peux pas supprimer le Dossier2 car il n'est pas vide.
11. on utilise la commande 'rm -rf Dossier2'

Commande importante:
1. On utilise la commande 'date +%T', time affiche les ressource utiliser par le paramètre rentré
2. Les dossiers cachés sont les dossiers commençant par un point.
3. Le chemin est /usr/bin/ls
4. Il n'existe pas d'entrée pour man ll, mais en utilisant alias ll on voit que c'est l'équivalent de ll -alF
5. On se place dans bin et on utilise ls.
6. ls .. permet de voir les fichiers et dossiers qui sont une fois en arrière
7. La commande pwd permet de voir le chemin du dossier courant
8. la commande echo 'bip' > plop exécutée 2 fois permet d'écrire bip dans le fichier plop, le contenu est effacé puis réécris
9. la commande echo 'bip' >> plop exécutée 2 fois, permet d'écrire bip a la fin du fichier plop et donc écris plusieurs fois bip
10. la commande sleep 10 | echo 'toto' permet d'écrire toto puis la commande se met en pause pendant 10 sec.
11. file permet d'avoir des informations sur un fichier comme son type
12. La commande ln original lien_phy permet de lié les fichiers, quand original est modifié lien_phy l'est aussi et quand il est supprimé lien_phy ne l'est pas
13. En modifiant en fichier l'autre sera modifié, en supprimant lien_phy, lien_sym va toujours exister mais il redirigera vers un fichier n'existant pas et nous marquera no such a file or directory
14. Ctrl+q permet d'interrompre le défilement et ctrl+q le reprend.
15. On utilise la commande 'head -5 syslog; tail -15 syslog; sed -n '-10, -20 p' syslog
16. dmesg permet de visualiser les processus de démarage linux et laisse de les voir page par page
17. Ce fichier contient les utilisateur, mot de passe chiffrés et permission. On peut voir la commande passwd avec 'man passwd'
18. La commande est 'ls -1 | sort -r', nous n'avons pas besoin de classer par nom, cela s'effectue par défaut
19. On utilise la commande 'wc --1 passwd'
20. On utilise la commande 'man -k DESCRIPTION:conversion | wc -l
21. On utilise la commande 'find . name 'passwwd'' pour trouver les fichier appeler passwd
22.
23.
24. Il faut faire un sudo apt install plocate pour pouvoir utiliser la commande.puis on utilise locate history.log et il nous donne le chemin
25. Il ne le trouve pas car il cherche dans les dossier personnel.

Exercice 3:
1. Pour copier syslog dans notre repertoire on utilise 'cp syslog ~'
2. On utilise alt+r, 'kernel', puis 'noyau'
3. Il faut utiliser alt+A pour marquer ce qu'il faut couper donc les 10 premières ligne, puis ctrl+k pour couper, ctrl+fleche bas pour aller en bas, puis ctrl+u pour coller
4. On utilise alt+u pour annuler l'action
5. On utilise ctrl+x pour quitter et on appuie sur y pour valider le changement

Exercice 4:

1. On utilise 'sudo cp .bashrc .bashrc_bak' pour faire une copie.
2. On enleve les '#' pour décommenter la ligne
3. On utilise la commande 'source .bashrc' pour éviter de redémarrer
4. On modifie la ligne apres if color prompt yes, pour ajouter '\033[01;91m\] [\d] \033[00m\] -' au départ.
