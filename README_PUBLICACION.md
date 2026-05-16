# Cómo modificar y publicar este portfolio en GitHub Pages

## 1. Instalar dependencias en Ubuntu

```bash
npm install
npm run dev
```

Abre el enlace local que aparece, normalmente `http://localhost:4321`.

## 2. Modificar el contenido

El contenido principal está en:

```bash
src/config.ts
```

Ahí puedes cambiar:

- `name`
- `title`
- `description`
- `social`
- `aboutMe`
- `skills`
- `projects`
- `experience`
- `education`

## 3. Configurar GitHub Pages

Edita `astro.config.mjs`.

Si tu repositorio se llama `TU_USUARIO.github.io`:

```js
site: "https://TU_USUARIO.github.io",
base: "/",
```

Si tu repositorio se llama, por ejemplo, `portfolio`:

```js
site: "https://TU_USUARIO.github.io",
base: "/portfolio",
```

## 4. Subir a GitHub

Crea un repositorio vacío en GitHub. Luego, desde esta carpeta:

```bash
git init
git add .
git commit -m "Initial portfolio website"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/NOMBRE_DEL_REPOSITORIO.git
git push -u origin main
```

## 5. Activar GitHub Pages

En GitHub:

Settings → Pages → Source → GitHub Actions

Luego revisa la pestaña Actions. Cuando termine correctamente, tu sitio estará publicado.
