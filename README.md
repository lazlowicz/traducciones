# Traducciones

Sitio Quarto preparado para publicar en GitHub Pages, escribir en castellano rioplatense y usar notas al margen.

## Uso local

Instalá las herramientas declaradas con mise:

```bash
mise install
```

Vista previa local:

```bash
mise run preview
```

Renderizar el sitio:

```bash
mise run render
```

Revisar textos con `typos` y `vale`:

```bash
mise run check
```

## Notas al margen

- Las notas al pie de Quarto se muestran en el margen por la configuración `reference-location: margin`.
- Para notas laterales explícitas usá:

```markdown
::: {.column-margin}
Texto de la nota al margen.
:::
```

## Publicación en GitHub Pages

El workflow `.github/workflows/pages.yml` renderiza Quarto y despliega `_site` en GitHub Pages al hacer push a `main`.

En GitHub, activá **Settings → Pages → Build and deployment → Source: GitHub Actions**.
