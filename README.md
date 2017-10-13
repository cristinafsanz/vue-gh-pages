# vue-gh-pages

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

## Instrucciones:

Seguido el tutorial [Setup GitHub Pages "gh-pages" branch as a subfolder within the "master" project](https://gist.github.com/chrisjacob/825950).

- Se incluye el directorio /dist de .gitignore.

- Generar el directorio de salida.

	- npm install //la primera vez

	- npm run build

- git add, git commit y git push origin master.

- cd dist

- git checkout -b gh-pages

- git add, git commit y git push origin gh-pages.

Resultado en https://cristinafsanz.github.io/vue-gh-pages/#/.

