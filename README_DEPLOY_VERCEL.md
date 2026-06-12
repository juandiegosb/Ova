# Deploy en Vercel

Este paquete ya está preparado como sitio estático para Vercel.

## Opción 1: desde el panel de Vercel

1. Sube esta carpeta a un repositorio de GitHub.
2. En Vercel, selecciona **Add New > Project**.
3. Importa el repositorio.
4. En configuración del proyecto deja:
   - Framework Preset: **Other**
   - Build Command: vacío o `echo Static site: no build step required`
   - Output Directory: `.`
5. Haz clic en **Deploy**.

## Opción 2: con Vercel CLI

```bash
npm i -g vercel
vercel
```

Cuando pregunte por el directorio/output, usa la raíz del proyecto.

## Archivos importantes

- `index.html`: archivo principal.
- `runtime-data.js`: datos del curso.
- `assets/`: imágenes y PDFs.
- `lib/`: librerías exportadas por el paquete.
- `vercel.json`: configuración para despliegue estático sin build.

## Nota

El contenido fue reorganizado para que Vercel lo sirva desde la raíz. No necesita backend ni variables de entorno.
