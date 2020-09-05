# Curso de TypeScript by Platzi
En este curso se parenderá lo básico sobre cómo suar TypeScript para tener tipado en nuestro código de JavaScript.

## Instalación del TypeScript Compiler
```bash
npm install -g typescript
```
**Compilar un archivo de TypeScript a JavaScript**
```bash
tsc hello.ts
```
**Observar los cambios de un archivo de TypeScript y compilar a JS**
```bash
tsc --watch hello.ts
```
## Archivo de configuración de TS 
El `tsconfig.json` es un archivo que se especifica en la raíz de nuestro proyecto TypeScript. Este especifica opciones para el compilador.

**Generar archivo de configuración**
```bash
tsc --init
```
Con este archivo por ejemplo podemos especificar la versión de ES que queramos usar o decidir que directorios, o subdirectorios, formaran parte del proceso de compilación.

Para correr nuestro archivo de configuración, solo es necesario ejecutar el comando:
```bash
tsc
```
Este busca el archivo tsconfig.json en la carpeta raiz de dónde se ejecuta. Si el archivo `tsconfig.json` se encuentra en otra carpeta solo debemos ejecutar:
```bash
tsc --project path_directory
```
**Generar carpeta personalizada de la salida de la compilación**

Modifica esta línea en el archivo de configuración de TS de la siguiente forma.
```json
"outDir": "./dist", 
```
