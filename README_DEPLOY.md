# DJ López Remix — Sitio listo para publicar

Este paquete contiene la versión final del sitio (multilenguaje, reproductores, WhatsApp, políticas y ajustes de audio).

## 📦 Contenido
- `index.html` (sitio principal)
- `assets/` (imágenes y recursos)
- `netlify.toml` (configuración de Netlify con redirección a `index.html`)
- `.nojekyll` (para GitHub Pages)
- `404.html` (fallback para GitHub Pages redirigiendo a `index.html`)
- `README_DEPLOY.md` (esta guía)

---

## 🚀 Opción A — Publicar en Netlify (drag & drop)
1. Entra a **https://app.netlify.com/** y ve a **Add new site → Deploy manually**.
2. Arrastra **el contenido de esta carpeta** (no la carpeta en sí). Debe incluir `index.html`, `assets/`, `netlify.toml`, `.nojekyll`, `404.html`.
3. Abre la URL asignada. (Puedes renombrarla en **Site settings → Domain management**).
4. (Opcional) Conecta un dominio propio en **Domain management**.

> Nota: Ya incluimos `netlify.toml` para que todas las rutas apunten a `index.html` (útil si agregas rutas internas en el futuro).

---

## 🌐 Opción B — Publicar en GitHub Pages (interfaz web)
1. Crea un repositorio público (ej.: `dj-lopez-remix-site`).
2. Sube **el contenido de esta carpeta** a la raíz del repo (`index.html`, `assets/`, `.nojekyll`, `404.html`).
3. Ve a **Settings → Pages**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` / `/ (root)`
4. Guarda. Tras ~1–2 min verás la **URL** en la parte superior de **Pages**.

> Nota: `.nojekyll` evita que GitHub Pages procese Jekyll. `404.html` tiene una redirección hacia `index.html` para mejorar la navegación.

---

## 🛠️ Opción C — Publicar con Git (avanzado)
```bash
# 1) Crea y entra en el repo
git init
git remote add origin https://github.com/USUARIO/dj-lopez-remix-site.git

# 2) Copia estos archivos a la carpeta del repo y confírmalos
git add .
git commit -m "Deploy sitio DJ López Remix"

# 3) Sube a GitHub
git branch -M main
git push -u origin main
```

Luego activa **Pages** como en la Opción B.

---

## 🔁 Actualizaciones futuras
- Edita `index.html` (textos, links, políticas) y vuelve a subir los cambios.
- Para Netlify, re‑arrastra la carpeta para redeploy.
- Para GitHub Pages, sube un nuevo commit a `main`.

¡Listo! Tu sitio está preparado para producción. 🎛️
