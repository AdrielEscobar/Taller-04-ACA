# Guía de instalación de Astro — Sitio MkDocs

Sitio de documentación creado con **MkDocs** y **Material for MkDocs** para el
taller "Documentación técnica con MkDocs".

## Requisitos
- Python 3 y pip

## Uso local

```bash
# 1. (Opcional) entorno virtual
python -m venv .venv
source .venv/bin/activate        # En Windows: .venv\Scripts\activate

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Vista previa en vivo
mkdocs serve
# Abre http://127.0.0.1:8000

# 4. Generar el sitio estático
mkdocs build
```

## Publicar en GitHub Pages

```bash
# Dentro del repositorio ya creado en GitHub
git init
git add .
git commit -m "Sitio de documentación con MkDocs"
git branch -M main
git remote add origin https://github.com/USUARIO/REPOSITORIO.git
git push -u origin main

# Desplegar (crea/actualiza la rama gh-pages)
mkdocs gh-deploy
```

Luego en GitHub: **Settings → Pages**, fuente rama `gh-pages` y carpeta `/ (root)`.

## Requisitos del taller cubiertos
- ✅ Tabla (en `index.md`, `requisitos.md` y `verificacion.md`)
- ✅ Bloque de código con pestañas / tabs (`instalacion.md`, etc.)
- ✅ Enlace interno entre páginas (rutas relativas en todas las páginas)
- ✅ Imagen en `docs/img/` (`logo.png`, usada en `index.md`)
- ✅ Bloque de admonición (`!!! note`, `!!! tip`, `!!! warning`)
