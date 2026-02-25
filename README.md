# Pour lancer le projet complet :

Dans VSCODE :
- git clone --recurse-submodules https://github.com/MSPR-501-Group-1/deploy.git
- cd deploy
- docker compose up --build

# Pour push depuis un submodule sur le repo "Deploy" :

- ÉTAPE 1 — dans le dossier du submodule (ex: ./backend)
git add .
git commit -m "feat: mon changement"
git push origin main          # ← push sur le repo du submodule

- ÉTAPE 2 — dans la racine du repo Main (ou Deploy)
git submodule update --remote backend
git add backend               # ← le parent enregistre le nouveau hash
git commit -m "Update latest commit from backend"
git push

# Règles importantes :

Dans chaque repo enfant, il faut avoir :

- Un dossier app ou tout le code se situe.
- Le .gitignore / Dockerfile / package.json / package-lock.json / README -> à la racine du repo.
