# Fixtroy
La página web de Fixtroy presenta una landing moderna y colorida que explica cómo crear una web usando inteligencia artificial. Incluye una sección principal con un mensaje llamativo, características destacadas, una guía sobre el uso de IA, un apartado de precio único y capturas de pantalla. Su diseño es limpio, dinámico y pensado para vender.

## Publicar en GitHub Pages

Pasos rápidos para desplegar el contenido de la carpeta `public/` usando el workflow creado:

1. Añade y confirma los cambios en la rama `main`:

```bash
git add public .github/workflows/pages.yml
git commit -m "Publicar sitio: añadir index y workflow de GitHub Pages"
git push origin main
```

2. El workflow `Deploy to GitHub Pages` se ejecutará automáticamente en `main`. Revisa la pestaña **Actions** en GitHub si necesitas ver el registro.

3. Después del despliegue, habilita GitHub Pages en la configuración del repositorio (si no está ya) y verifica la URL pública en la sección *Pages* del repositorio.

## Dominio personalizado (CNAME)

Si quieres usar un dominio propio, crea un archivo `CNAME` en `public/` con tu dominio (ejemplo: `midominio.com`) y empuja el cambio:

```bash
echo "midominio.com" > public/CNAME
git add public/CNAME
git commit -m "Añadir CNAME para dominio personalizado"
git push origin main
```

GitHub Pages gestionará el certificado HTTPS automáticamente para el dominio una vez esté correctamente configurado.

¿Quieres que cree el archivo `public/CNAME` ahora con tu dominio o prefieres que lo haga tú mismo cuando lo tengas listo?

<!-- trigger: re-run Pages workflow -->
