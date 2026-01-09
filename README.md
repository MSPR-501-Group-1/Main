# Pour lancer le projet complet :

Dans VSCODE :
- git clone --recurse-submodules https://github.com/my-project-org/deploy.git
- cd deploy
- docker compose up --build

# Pour push depuis un submodule sur le repo "Deploy" :

- Aller à la racine du submodule (ex : cd backend)
- git pull

- cd ..
- On ajoute le submodule avec git add (ex : git add backend)
- git commit -m "Update backend version"
- git push