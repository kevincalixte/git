# COMMANDES GIT

* git init
* git remote add origin url
* git status
* git add . ou git add nomdufichier
* git commit -m "message"
* git log
* git push -u origin branche
* git push origin branch
* git branch nombranche
* git checkout -b branche
* git branch
* git checkout branche
* git merge branche
* git branch -d branch
* git pull
* git fetch

# UTILISER GIT EN GROUPE
* git fetch permet de voir ce qui a changé sans fusionner, non obligatoire si git pull (car pull = fetch + merge)
* git status permet de savoir si on doit faire un pull
* après un push on doit aller sur github pour créer le pull request et merge si on a les droits, ou l'autre doit valider
* behind = je dois pull / ahead = je dois push
* behind = risque de conflits / ahead = les autres pourraient avoir besoin de tes changements

- NE JAMAIS TRAVAILLER SUR MAIN

- Cloner le depot
git clone url
cd dossier

- Creer une branche

git checkout -b nombranche

- Apres modifications
git add .
git commit -m "message"

- Pour mettre à jour le main et le rammenner dans la branche où on travaille
git checkout main
git pull
git checkout nombranche
git merge main

- Si on souhaite push
git push -u origin nombranche (la premiere fois)
git push