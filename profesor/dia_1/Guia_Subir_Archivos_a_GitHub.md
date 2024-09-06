
# Guía: ¿Cómo Subir Archivos a GitHub?

## -1. Breve Descripción de Cómo Crear un Repositorio
Un **repositorio** es como una carpeta en la nube donde guardas todos tus archivos de un proyecto. Es un espacio en GitHub donde puedes almacenar, compartir y gestionar el código de tu proyecto.

### Pasos para Crear un Repositorio:
1. Inicia sesión en GitHub.
2. Haz clic en el botón "New" (Nuevo) para crear un nuevo repositorio.
3. Elige un nombre para tu repositorio y decide si quieres que sea público o privado.
4. Puedes añadir un README.md (archivo de descripción) si lo deseas.
5. Haz clic en "Create repository" (Crear repositorio) y listo, ya tienes tu repositorio.

## 0. Abrir la Consola de Git en la Carpeta Deseada
Antes de comenzar a trabajar con Git, debes abrir la consola (terminal) de Git en la carpeta donde deseas guardar o trabajar con tu proyecto. Esto te permitirá ejecutar comandos de Git directamente en ese directorio.

## 1. Clonar Repositorio Usando el Enlace
Para empezar a trabajar en un proyecto ya existente, necesitas clonar el repositorio en tu computadora. Para hacerlo:

1. Copia el enlace del repositorio desde GitHub (botón "Code" y luego "HTTPS").
2. En la consola de Git, escribe el comando:
    ```bash
    git clone https://github.com/usuario/nombre-del-repositorio.git
    ```
   Esto es como hacer una copia de la carpeta (repositorio) en tu computadora.

## 2. Crear un Archivo Desde la Consola del Code
Después de clonar el repositorio, puedes crear archivos directamente desde la consola. Por ejemplo, para crear un archivo llamado `archivo.txt`:

```bash
touch archivo.txt
```
Este comando crea un archivo vacío con el nombre y la extensión que le des.

## 3. Añadir el Archivo al Repositorio: `git add nombredelarchivo`
**Analogía**: Imagina que estás comprando cosas en una tienda. `git add` es como poner esos artículos en tu carrito de compras. Aún no has pagado (guardado los cambios), pero ya has decidido qué llevar.

Para añadir un archivo específico al carrito, usa:
```bash
git add nombredelarchivo.extensión
```
O para añadir todos los archivos modificados:
```bash
git add .
```

## 4. Guardar los Cambios: `git commit`
**Analogía**: `git commit` es como pagar en la caja. Ahora que tus artículos (cambios) están en el carrito (`git add`), `git commit` los guarda en el historial de tu repositorio.

Para hacer un commit, escribe:
```bash
git commit -m "Mensaje describiendo los cambios"
```
Este mensaje debe describir brevemente qué cambios has hecho.

## 5. Publicar los Cambios: `git push`
**Analogía**: `git push` es como enviar tu compra a casa. Después de haber pagado (`git commit`), `git push` envía esos cambios al repositorio en la nube (GitHub).

Para publicar los cambios, usa:
```bash
git push origin main
```
Esto enviará los cambios de la rama principal (`main`) a GitHub.

## 6. Descargar los Archivos del Repositorio a tu Computadora: `git pull`
**Explicación**: A veces, es posible que necesites actualizar tu copia local del repositorio con los cambios más recientes que alguien más ha hecho en GitHub.

**Traducción**:
- **Pull**: significa "jalar" o "traer", y en este contexto, significa traer los cambios más recientes de GitHub a tu computadora.
- **Push**: como mencionamos antes, significa "empujar" o "enviar" los cambios de tu computadora a GitHub.

Para traer los cambios más recientes del repositorio en GitHub, usa:
```bash
git pull origin main
```

Este comando sincroniza tu copia local con los cambios que han sido publicados en GitHub.
