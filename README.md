# vue-gh-pages

Repositorio creado a partir de la [demo de Jose Dongil](https://github.com/jdonsan/charla-aprendiendo-vuejs) y la [guía](https://github.com/cristinafsanz/vuejs-primeros-pasos) que hice a partir de ella.

El propósito del repositorio es subir a la rama gh-pages el contenido generado en el directorio de producción /dist y habilitar GitHub Pages para que lo publique desde esa rama.

## Instrucciones:

- Se ha cambiado la ruta en config.index.js: assetsPublicPath: '/vue-gh-pages/dist/'

- npm install

- npm run build

- Quito dist de .gitignore

- Seguir instrucciones de https://gist.github.com/cobyism/4730490 para subir el contenido de dist en gh-pages.

    - git add dist && git commit -m "Initial dist subtree commit"

    - git subtree push --prefix dist origin gh-pages

