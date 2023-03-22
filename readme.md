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
- config/shield.ts: Commented this line: import Env from '@ioc:Adonis/Core/Env'

===========

Push to github and deploy to vercel:

- git add . && git commit -m "c" && git push origin main
- npm run build
- node ace dump:rcfile # to create .adonisrc.json file in the project's root directory
- cd build
- npm ci --production
- (Copy-pasted .env.example file as .env file in build folder)
- (Copy-pasted .adonisrc.json file in "node_modules/@adonisjs/application/build")
- node server.js
- vercel --prod
