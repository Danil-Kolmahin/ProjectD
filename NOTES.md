# Steps to start a new project
    code ./
    npx create-nx-workspace --preset=apps
    git remote add origin git@github.com:KolmaginDanil/ProjectD.git
    git branch -M main
    git config user.email "43148295+KolmaginDanil@users.noreply.github.com"
    git config user.name "dkolmagin"
    git push -u origin main

    npm install -D @nrwl/react
    npx nx g @nrwl/react:app client
    git add -A && git commit -m "Add client application" && git push

# Run current project
    npx nx build client:build:production
    npx http-server ./dist/apps/client

    npx nx build server:build:production
    node ./dist/apps/server/main.js
