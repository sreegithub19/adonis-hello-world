Steps to install and run:

- npm i create-adonis-ts-app -g
- npm init adonis-ts-app adonis-hello-world

            CUSTOMIZE PROJECT
            ❯ Select the project structure · web
            ❯ Enter the project name · hello-world
            ❯ Setup eslint? (y/N) · true
            ❯ Setup prettier? (y/N) · true
            ❯ Configure webpack encore for compiling frontend assets? (y/N) · true

- cd adonis-hello-world
- node ace serve --watch

===========

Push to github and deploy to vercel:

- git add . && git commit -m "c" && git push origin main
