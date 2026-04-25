# 🚀 Cómo publicar Silver Dawn Creator en Vercel

## Lo que vas a necesitar
- Una cuenta en GitHub (gratis): https://github.com
- Una cuenta en Vercel (gratis): https://vercel.com
- Tu API key de Anthropic: https://console.anthropic.com

---

## PASO 1 — Subir el proyecto a GitHub

1. Abrí https://github.com y logueate
2. Click en el botón verde **"New"** (esquina superior izquierda)
3. Nombre del repositorio: `silver-dawn-creator`
4. Dejalo en **Public** y click en **"Create repository"**
5. En la página que aparece, buscá la sección **"…or upload an existing file"**
   y hace click en **"uploading an existing file"**
6. Arrastrá TODA la carpeta `silverdawn` (o subí los archivos uno por uno):
   - `vercel.json`
   - `package.json`
   - `api/chat.js`
   - `public/index.html`
7. Click en **"Commit changes"**

---

## PASO 2 — Conectar con Vercel

1. Abrí https://vercel.com y logueate con tu cuenta de GitHub
2. Click en **"Add New Project"**
3. Buscá tu repositorio `silver-dawn-creator` y click en **"Import"**
4. En la pantalla de configuración, no cambies nada — click en **"Deploy"**
5. Vercel va a construir y publicar la app automáticamente
6. Al terminar te da una URL tipo: `https://silver-dawn-creator.vercel.app`

---

## PASO 3 — Agregar tu API key de Anthropic (para que funcione la IA)

1. En Vercel, abrí tu proyecto
2. Click en **"Settings"** → **"Environment Variables"**
3. Click en **"Add New"**
4. Completá:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** (pegá tu API key — empieza con `sk-ant-...`)
   - **Environment:** seleccioná los tres: Production, Preview, Development
5. Click en **"Save"**
6. Ahora vas a **"Deployments"** y click en **"Redeploy"** para que tome la variable

---

## PASO 4 — Listo 🎉

Entrá a tu URL (ej: `https://silver-dawn-creator.vercel.app`) y la IA va a funcionar.

Cada vez que quieras actualizar la app:
1. Reemplazá el archivo `public/index.html` en GitHub
2. Vercel lo republica automáticamente en segundos

---

## Dónde obtener tu API key de Anthropic

1. Abrí https://console.anthropic.com
2. Logueate con tu cuenta
3. Click en **"API Keys"** en el menú lateral
4. Click en **"Create Key"**
5. Copiá la key (solo se muestra una vez)

---

## ¿Dudas?

Preguntame en claude.ai y te ayudo paso a paso.
