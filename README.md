# Pour lancer le projet complet :

Dans VSCODE :
- git clone --recurse-submodules https://github.com/MSPR-501-Group-1/deploy.git
- cd deploy
- docker compose up --build

# Pour push depuis un submodule sur le repo "Deploy" :

- Aller dans la racine du projet Deploy
- Taper la commande : "git submodule update --remote NOM_DU_SERVICE"
- Faite un commit du genre "Update latest commit from NOM_DU_SERVICE"