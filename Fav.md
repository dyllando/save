![Git](http://git-scm.com/images/logo@2x.png)

Lexique :
---------
* HEAD : la révision courante (normalement le dernier commit)
* untracked : pas encore versionné
* unmodified : versionné mais pas modifié
* modified : ayant des modifications pas encore ajouté au repo local
* staged : sur le repo local
* fast-forward (ou ff) : [explication](http://tech.m6web.fr/tentative-d-explication-des-fast-forward-sous-git)


Catastrophe, j'ai tout perdu : 
------------------------------

A moins de ne pas avoir poussé sur un repo distant et d'avoir supprimer le dossier ````.git````, il est théoriquement impossible de perdre quelques choses avec Git : 

1. ````$ git reflog```` pour voir les dernières actions exécuté (numéroté)
2. ````$ git reset 'HEAD@{1}'```` pour revenir au HEAD a l'état précédent la catastrophe
3. Le HEAD est maintenant à l'endroit voulu mais les fichiers en local sont toujours ceux précédent la catastrophe, donc il faut les annuler en faisant ```$ git checkout nomBrancheCourante``` 


Repo local :
------------

Voir quels fichiers sont "untracked" et "modified"
    
````$ git status````

---

Ajouter un fichier "untracked"/"modified"
    
````$ git add fileName````

---

Ajouter toutes les fichiers "untracked"/"modified"
    
````$ git add .````

---
