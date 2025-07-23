## INSTALACION

https://nextjs.org/docs/app/getting-started/installation

npx create-next-app@latest

yes (typescript, eslint, tailwind css, app router, src /directory, turbopack)
not (customize import @)

turbopack es un bundler, empaquetador que coge todos los archivos y los convierte en uno o varios que pueda interpretar el navegador.
Ejemplo:
Antes de bundle:
src/
index.js
utils.js
app.css
logo.png

Después de bundle:
dist/
bundle.js
bundle.css

## Fichero principal de configuración package.json

package => rango de dependencias compatibles
package-lock => dependencias exactas.
Al git no se sube el node modules (gitignore), solo el package, y con un npm install se reproducen todas las dependencias
Contiene: dependencias de desarrollo, scripts de ejecución (desarrollo, producción, eslint), versionado y nombre

## Tailwind 4

Todo se encuentra en app/globals.css

## Git for windows

https://git-scm.com/downloads/win
git --version
git init

git config --global user.name "roro"
git config --global user.email "rociold027@gmail.com"

git status
git add .
git commit -m "init"
git log

git branch -M main
git remote add origin https://github.com/ringostar027/the-road-to-next.git
git push -u origin main

Si yo modifico algo, puedo ver que hay diferentes versiones entre mi VSC y mi git:

git status
git diff

Entonces actualizo y compruebo de la siguiente manera:

git add .
git status

git commit -m "changes in roro.md"
git status
git log
