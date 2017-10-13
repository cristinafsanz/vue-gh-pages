# vue-gh-pages

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

## Instrucciones:

- Se incluye el directorio /dist de .gitignore.

- git add, git commit y git push origin master.

- Generar el directorio de salida.

	- npm install //la primera vez

	- npm run build

- git checkout -b gh-pages //-b la primera vez

- Dejar sólo index.html y los assets en la rama (método manual para probar resultado, pendiente investigar método para que no se suba /dist en master y subir ficheros a gh-pages).

	- rm -fr test static/ src/ package.json index.html config/ build/ node_modules/ README.md

	- mv dist/* .

	- rm -fr dist/

	- git add, git commit y git push origin gh-pages.

Resultado en https://cristinafsanz.github.io/vue-gh-pages/#/.

