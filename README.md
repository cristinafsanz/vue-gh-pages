# vue-gh-pages

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

## Instrucciones:

Seguido el tutorial [Simple Deployment to GH Pages](https://discourse.gohugo.io/t/simple-deployment-to-gh-pages/5003).

- Se incluye el directorio /dist de .gitignore para que no se suba a la rama master.

- Borrar el directorio dist para que esté vacío:

	- rm -fr dist

- Crear una rama gh-pages vacía y subir a GitHub

	- git checkout -b gh-pages

	- rm -fr * //borrar los ocultos que nos sean necesarios también

	- git add . && git commit -m "Initial branch" && git push origin gh-pages

- Clonar la rama gh-pages desde el repositorio local a un repositorio localizado en dist.

	- git clone .git --branch gh-pages dist

- Generar el directorio de salida.

	- npm install //la primera vez

	- npm run build

- Hacer commit de los cambios en el directorio creado y hacer push a la rama local gh-pages.

	- cd dist

	- git add --all -f

	- git commit -m "Publishing to gh-pages"

	- git push origin gh-pages

Resultado en https://cristinafsanz.github.io/vue-gh-pages/#/.
