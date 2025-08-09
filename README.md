# Tu Asesor Inmobiliario – Netlify + Decap CMS

## Estructura
- `index.html` (tu landing Bootstrap, lee `/data/propiedades.json`)
- `admin/` (panel Decap CMS)
- `data/propiedades.json` (listado editable desde /admin)
- `static/uploads/` (imágenes subidas desde el CMS)
- `netlify.toml` (evita cache en /admin)

## Despliegue rápido
1. Sube todo esto a un repo en GitHub.
2. En Netlify: **Add new site → Import from Git** → elige el repo.
   - Build command: *(vacío)*
   - Publish directory: `/`
3. Activa **Identity**: Project configuration → Identity → Enable.
4. **Identity → Services → Git Gateway → Enable**.
5. **Identity → Users → Invite user** (email de tu madre).
6. Abre `/admin` y edita **Propiedades (listado)**. Guarda → deploy automático.
