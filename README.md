# vue-gh-pages

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

## Instrucciones:

Seguidos los tutoriales [Simple Deployment to GH Pages](https://discourse.gohugo.io/t/simple-deployment-to-gh-pages/5003) y [Setup GitHub Pages "gh-pages" branch and "master" branch as subfolders](https://gist.github.com/chrisjacob/833223/ee7cfb6413262754c79840c28b4202d461154658).

- Se incluye el directorio /dist de .gitignore para que no se suba a la rama master.

- Borrar el directorio dist para que esté vacío:

	- rm -fr dist

- Clonar el repositorio en dist y dejar sólo rama gh-pages vacía.

	- mkdir dist

	- cd dist

	- git clone https://github.com/cristinafsanz/vue-gh-pages.git .

	- git checkout origin/gh-pages -b gh-pages

	- git branch -d master

	- rm -fr * //también borrar los ficheros ocultos menos el .git

- Generar el directorio de salida.

	- cd ..

	- npm install //la primera vez

	- npm run build

- Hacer commit de los cambios en el directorio creado y hacer push a la rama local gh-pages.

	- cd dist

	- git add .

	- git commit -m "Publishing to gh-pages"

	- git push origin gh-pages

Resultado en https://cristinafsanz.github.io/vue-gh-pages/#/.

