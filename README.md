# 🚀 Template de Proyecto Node.js
Autor: Iván Talijancic

## 📋 Instrucciones de Uso

Para ejecutar este proyecto Template, sigue las siguientes instrucciones:

1. **Descargar el código del repositorio:** [Template](https://github.com/italijancic/pc-2024-template). Asegúrate de elegir la rama correcta al descargar.

2. **Descomprimir el código** en la ubicación que desees en tu computadora.

3. **Abrir la carpeta con VSCode:** **Asegúrate de estar dentro de la carpeta raíz.** Esto es muy importante, ya que de lo contrario no podrás ejecutar el código del proyecto.

4. **Instalar dependencias:** Si no se han instalado las dependencias del proyecto (si no ves la carpeta `node_modules` en tu proyecto), ejecuta en tu consola `npm install`.

5. **Ejecutar el proyecto:** En tu consola (terminal de VSCode), ejecuta `npm run dev`.

## 📂 Contenido del Repositorio

### 1. `package.json`
Este archivo define la configuración del proyecto, incluyendo las dependencias, scripts y metadatos.

- **name:** Nombre del proyecto.
- **version:** Versión del proyecto.
- **description:** Descripción del proyecto.
- **type:** Define que el proyecto usa módulos `ECMAScript`.
- **main:** Archivo principal del proyecto (`app.js`).
- **scripts:**
  - `dev:` Ejecuta el archivo `app.js` en modo de observación (watch mode).
  - `test:` Script de prueba (aún no configurado).
- **author:** Autor del proyecto.
- **license:** Licencia del proyecto.
- **devDependencies:** Dependencias para el desarrollo, incluyendo ESLint para análisis estático del código.
- **dependencies:** Dependencias del proyecto, en este caso `readline-sync` para leer entradas del usuario.

### 2. `eslint.config.mjs`
Configuración de ESLint para asegurar que el código siga las mejores prácticas. Usa el plugin `@eslint/js` y configura los globals necesarios.

### 3. `app.js`
Archivo principal que contiene ejemplos de cómo leer entradas desde la consola usando el módulo `prompt`.

**Ejemplos en `app.js`:**
- Leer una cadena de texto (nombre del usuario).
- Leer un número entero (edad del usuario).
- Leer un número flotante (altura del usuario).

### 4. `prompt.js`
Módulo que proporciona una función `prompt` para leer entradas desde la consola usando `readline-sync`.

## 📝 Ejemplos de Uso

### Leer una Cadena de Texto
El programa pedirá el nombre del usuario y luego lo saludarán.

```javascript
import { prompt } from './prompt.js';

const nombre = prompt('Escribe tu nombre: ');
console.log(`Hola, ${nombre}! Bienvenido al curso de Programación de Computadoras 2024 | UTN - FRRQ`);
```

### Leer un Número Entero
El programa pedirá la edad del usuario y la mostrará en consola.

```javascript
import { prompt } from './prompt.js';

const edad = parseInt(prompt('¿Cuántos años tienes?: '));
console.log(`${nombre} tiene ${edad} años.`);
```

### Leer un Número Flotante
El programa pedirá la altura del usuario en metros y la mostrará en consola.

```javascript
import { prompt } from './prompt.js';

const altura = parseFloat(prompt('¿Cuál es tu altura en metros?: '));
console.log(`${nombre} mide ${altura} metros.`);
```
