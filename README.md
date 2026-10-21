# Calzados Scarleth — demo y plantilla de sitio web

Sitio de una sola página para una zapatería que vende por WhatsApp. Hecho en HTML, CSS y JavaScript puro, sin frameworks ni dependencias: se abre con doble clic y se publica en cualquier hosting estático (GitHub Pages, Netlify, Shopify no aplica).

**Demo:** activá GitHub Pages en este repositorio y el sitio queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Qué incluye

- Telón de carga con la bota cayendo y brillo de cuero (solo la primera vez por sesión).
- Portada con entrada línea por línea, parallax y bota que flota.
- Marquesina que reacciona a la velocidad del scroll.
- Catálogo con filtros y botón "Pedir esta" que abre WhatsApp con el mensaje listo.
- Escena fijada al scroll: la bota gira y aparecen sus detalles; termina con "Hecha para durar".
- Sección de mayoreo con formulario que arma el mensaje de cotización para WhatsApp.
- Cursor con huella de bota (solo en computadora), botón flotante de WhatsApp y menú animado en celular.
- Selector de paleta (A ámbar / B rojo ladrillo), pensado para quitarse al elegir una.
- Respeta `prefers-reduced-motion`. Si falla el JavaScript, el contenido se ve igual.

## Cómo adaptarla a otro cliente

Todo está en `index.html`.

1. **Colores:** al inicio del `<style>`, en `:root`. Cambiá `--accent`, `--bg`, `--glow` y `--cream`.
2. **WhatsApp:** buscá `wa.me/50558769896` y reemplazá el número (código de país + número, sin espacios ni guiones).
3. **Productos:** cada tarjeta es un `<article class="card">` dentro de `#grid`. Copiá una, cambiá la foto, el nombre, la categoría (`data-c`) y el texto del botón.
4. **Fotos:** van en `img/`. Recortadas sin fondo, en WebP, de unos 450–650 px de alto.
5. **Textos:** están en español con voseo (Nicaragua). Cambiá según el país del cliente.
6. **Selector de paleta:** cuando el cliente elija, borrá el bloque `<div class="palette">` y su CSS.

## Pendientes antes de publicar para el cliente

- Confirmar el número de WhatsApp.
- Reemplazar las fotos provisionales (capturas de video) por fotos de producto.
- Confirmar precios: solo la bota vaquera tiene precio real; las demás dicen "Precio por WhatsApp".
- Reseñas, dirección y horario están marcados como "por confirmar".

## Tipografías

Big Shoulders Display, Cormorant Garamond y Figtree, cargadas desde Google Fonts.
