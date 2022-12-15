# curso-webpack-react

<a href="https://gitmoji.dev">
  <img src="https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg?style=flat-square" alt="Gitmoji">
</a>
<br/>

## Instalaciones necesarias y configuración
### Genéricas
> git init
> git config --local user.email "desarrolloaplicacionesweb.jmlb@gmail.com"
> git config --local user.name "JUANLUNABLANCO"
> git branch -M  main

En este punto debes crear un repositorio nuevo en github vacío y enlazarlo

<!-- > git remote add origin https://github.com/JUANLUNABLANCO/<tu-repo>.git -->
> git remote add origin https://github.com/JUANLUNABLANCO/webpack-react.git
> git config --list
> git add .
> git commit -m "scaffolding project with webpack"
> git push -u origin main

> npm init
### React instalations

> npm install -S react react-dom

### Otros

> mkdir src
> mkdir -p src/components

crear el archivo App.jsx dentro de components

--- App.jsx ---
import React from 'react';

const App = () => <h1>Hello React!</h1>

export default App;
--- ---
---  index.js ---
import React from 'react';
import ReactDOM from 'react-dom';
import App from './components/App';

ReactDOM.render(<App />, document.getElementById('app'));
--- ---

render coge un componente creado y lo inserta en el segundo parámetro

--- index.html ---
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <div id="app"></div>
</body>

</html>
--- ---

Ya tenemos la app

## Instalaciones de babel y webpack

> npm install @babel/core  @babel/preset-env @babel/preset-react babel-loader -D

> touch .babelrc
--- .baberc ---
{
  "presets": [
    "@babel/preset-env",
    "@babel/preset-react"
  ]
}
--- ---

> npm install -D webpack webpack-cli webpack-dev-server

## Frameworks librerias que funcionan con react

https://es.reactjs.org/docs/create-a-new-react-app.html

leer ese artículo del blog, es muy interesante




