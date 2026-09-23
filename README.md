# Recorrido 3D · Piso García

Sitio estático compatible con GitHub Pages. No requiere compilación ni servidor de aplicación.

## Publicar

1. En el repositorio de GitHub, abrir **Settings → Pages → Build and deployment** y seleccionar **GitHub Actions** como Source.
2. Subir estos cambios a la rama `main`.
3. Esperar a que termine el workflow **Publicar sitio en GitHub Pages**, en la pestaña **Actions**. También se puede ejecutar manualmente con **Run workflow**.

URL prevista: https://josecaicedodev.github.io/lifitiglobal/

`index.html` redirige al recorrido. También se puede acceder directamente a `recorrido_3d.html`. Los enlaces relativos mantienen la navegación dentro de la ruta del repositorio.

El workflow publica únicamente la entrada, el recorrido, el presupuesto HTML y el Excel. Three.js, OrbitControls y TWEEN se cargan desde CDN mediante HTTPS; el visor requiere conexión a internet y WebGL.

## Vista previa local

Desde la carpeta del repositorio:

```sh
python -m http.server 8000
```

Abrir http://localhost:8000/ y comprobar la navegación al recorrido y al presupuesto.

Configuración basada en la [documentación de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages).
