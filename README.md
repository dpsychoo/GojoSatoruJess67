# Gojo-master — despliegue en Vercel

Este proyecto es un sitio estático (HTML/CSS/Assets). Aquí están las instrucciones breves para desplegarlo en Vercel.

Opciones de despliegue

- Opción A — Vercel (interfaz web, recomendado):
  1. Empuja este repositorio a GitHub (o GitLab/Bitbucket).
  2. Ve a https://vercel.com, inicia sesión y selecciona "Import Project" → conecta tu repositorio.
  3. En "Framework Preset" selecciona "Other" o "Static Site" y deja las opciones por defecto.
  4. Importa y Vercel desplegará automáticamente.

- Opción B — Vercel CLI (rápido desde tu máquina):
  1. Instala la CLI si no la tienes:

```bash
npm install -g vercel
# o
pnpm add -g vercel
```

  2. En la carpeta del proyecto (donde está `index.html`) inicia sesión y despliega:

```bash
vercel login
vercel
```

  3. Sigue las preguntas interactivas; acepta los valores por defecto o pon el nombre de proyecto que prefieras.

Notas
- He añadido `vercel.json` para asegurar que el sitio se sirva como estático y que todas las rutas regresen a `index.html` (útil si el proyecto tiene comportamiento tipo SPA).
- Si quieres, puedo:
  - Crear el repositorio en GitHub y empujar los archivos desde aquí (necesitaría permisos/credentials),
  - O guiarte paso a paso mientras ejecutas los comandos locales.
