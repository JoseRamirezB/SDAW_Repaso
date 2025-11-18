# Proyecto SDAW_8951

## Descripción del proyecto de repaso

Este proyecto forma parte de la práctica de la asignatura **SDAW**.\
Consiste en una pequeña aplicación web servida con **Node.js** y
**Express**, que muestra un mensaje al usuario con mi nombre (José Luis Ramírez Barrios) al pulsar un botón.

------------------------------------------------------------------------

## Estructura del proyecto

    /SDAW_8951
    ├── index.html       # Página principal
    ├── script.js        # Código JavaScript que muestra el mensaje
    ├── server.js        # Servidor con Express
    ├── package.json     # Configuración del proyecto Node.js
    ├── .gitignore       # Archivos ignorados por Git
    └── README.md        # Documentación del proyecto

------------------------------------------------------------------------

## Comandos utilizados

### Node.js

``` bash
# Inicializar el proyecto Node.js
npm init -y

# Instalar Express como dependencia
npm install express

# Iniciar el servidor
npm start
```
## Información técnica añadida desde rama 1

En esta sección se describen los principales comandos de Git utilizados durante la práctica:

- git init: Sirve para inicializar un nuevo repositorio local en el directorio actual.
- git add: Permite añadir ficheros al área de preparación (staging area) para incluirlos en el próximo commit.
- git commit: Registra los cambios añadidos en el repositorio, creando un punto en el historial de commits.
- git branch: Sirve para crear, listar o eliminar ramas en el repositorio.
- git merge: Combina los cambios realizados en una rama en otra.
- git push: Envía los commits locales al repositorio remoto.
------------------------------------------------------------------------

## Fragmentos de código relevantes

### `index.html`

``` html
<button id="saludoBtn">Haz clic aquí</button>
<script src="script.js"></script>
```

### `script.js`

``` js
document.getElementById("saludoBtn").addEventListener("click", function() {
  alert("Hola José Luis Ramírez Barrios");
});
```

### `server.js`

``` js
const express = require('express');
const app = express();
const path = require('path');
const PORT = 3000;

app.use(express.static(__dirname));

app.get('/', (req, res) => {
  res.sendFile(path.join(__dirname, 'index.html'));
});

app.listen(PORT, () => {
  console.log(`Servidor corriendo en http://localhost:${PORT}`);
});
```

------------------------------------------------------------------------
## Información técnica añadida desde rama 2 
5327259 (HEAD -> rama2_JoseLuisRamirez, main) Revert "chore: Añadido log para depuración en script.js"
0531076 chore: Añadido log para depuración en script.js
7f23b57 feat: Añadido párrafo en index.html
97cd66f docs: Modificar comentario informativo en server.js
1072718 (origin/main) Primer commit del repositorio SDAW_8951
## Conclusiones personales

Durante esta práctica he aprendido a: 
- Crear la estructura básica de un
proyecto Node.js.
- Realizar el control de versiones de un proyecto manejando repositorios local y remotos, así como la creación de ramas y de pull request.
- Levantar un proyecto web en local haciendo uso de Node JS.

Además, he aprendido la importancia a formatear documentación de proyectos en READMEs y a usar `.gitignore` para evitar subir archivos innecesarios al
repositorio.

------------------------------------------------------------------------

## Ejecución del proyecto

1.  Clonar o descargar este proyecto.

2.  Abrir una terminal dentro de la carpeta `SDAW_8951`.

3.  Instalar las dependencias ejecutando:

    ``` bash
    npm install
    ```

4.  Iniciar el servidor con:

    ``` bash
    npm start
    ```

5.  Abrir el navegador y acceder a:

        http://localhost:3000


## Autor

**José Luis Ramírez Barrios**
## Estructura del proyecto de repaso

    /SDAW_8951
    ├── index.html       # Página principal
    ├── script.js        # Código JavaScript que muestra el mensaje
    ├── server.js        # Servidor con Express
    ├── package.json     # Configuración del proyecto Node.js
    ├── .gitignore       # Archivos ignorados por Git
    └── README.md        # Documentación del proyecto

------------------------------------------------------------------------