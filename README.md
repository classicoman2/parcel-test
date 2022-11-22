# parcel-test
Proves amb Parcel JS.
- Live Server amb Parcel
- SCSS integrat
- Crea una versio `build` en qüestió de segons

El servidor de desenvolupament disposa d'un _live server_ propi que fa  _hot reloading_ també en els canvis que facem en SCSS. As you make changes to your code, Parcel automatically rebuilds the changed files and updates your app in the browser

Documentació de Parcel emprada disponible [aqui](https://parceljs.org/getting-started/webapp/)

Per configurar el projecte en Parcel,

```bash
npm init -y

npm install --save-dev parcel
```

Contingut recomanat del `package.json`:

```json
{
  "name": "my-project",
  "source": "src/index.html",
  "scripts": {
    "start": "parcel",
    "build": "parcel build"
  },
  "devDependencies": {
    "@parcel/transformer-sass": "^2.8.0",
    "parcel": "latest"
  }
}
```



Per posar en marxa el live server, 

```bash
npx parcel src/index.html
```

Emprar SCSS amb parcel: [Explicat aqui](https://parceljs.org/languages/sass/)
