# Fundamentos HTML — Proyecto de ejemplo

Resumen
-------
Proyecto de ejemplo con páginas HTML y una hoja de estilos simple. Ideal para prácticas básicas de HTML y CSS.

Estructura
---------
- [carpeta1/home.html](carpeta1/home.html) — Página de ejemplo con títulos, listas, imágenes y enlaces.
- [carpeta1/home3.html](carpeta1/home3.html) — Página simple con texto estático.
- [carpeta1/home4.html](carpeta1/home4.html) — Página que carga la hoja de estilos `main.css`.
- [carpeta1/blog.html](carpeta1/blog.html) — Ejemplo de uso de `header`, `article`, `section` y `footer`.
- [carpeta1/main.css](carpeta1/main.css) — Hoja de estilos del proyecto.

Descripción de archivos
-----------------------
- [carpeta1/home.html](carpeta1/home.html)
  - Contiene ejemplos de encabezados h1–h6, párrafos, listas ordenadas y desordenadas, imágenes y enlaces.
- [carpeta1/home3.html](carpeta1/home3.html)
  - Página mínima con texto.
- [carpeta1/home4.html](carpeta1/home4.html)
  - Página que importa la hoja de estilos: `<link rel="stylesheet" href="main.css">`.
  - Usa las clases CSS [`.texto-article`](carpeta1/main.css) y [`.texto-plano`](carpeta1/main.css).
- [carpeta1/blog.html](carpeta1/blog.html)
  - Ejemplo de estructura semántica (`header`, `article`, `section`, `footer`).
- [carpeta1/main.css](carpeta1/main.css)
  - Define estilos por etiqueta y por clase. Contiene actualmente un error de sintaxis (falta una llave de cierre y la regla de `.texto-plano` está mal formada).

Problemas conocidos y recomendaciones
------------------------------------
1. Errores en CSS:
   - En [carpeta1/main.css](carpeta1/main.css) falta la llave de cierre `}` para la clase `.texto-article` y la regla `.texto-plano` está incompleta. Solución recomendada: cerrar la regla y declarar `.texto-plano` correctamente.
   - Referencia rápida a los selectores en el CSS: [`.texto-article`](carpeta1/main.css), [`.texto-plano`](carpeta1/main.css).

2. Rutas de imágenes inconsistentes:
   - En algunos HTML se usa `carpeta1/imagen1.jpg` y en otros `imagen1.jpg`. Estandarizar rutas según la ubicación real de las imágenes o mover imágenes a una carpeta `assets/` o `images/`.

3. Accesibilidad y semántica:
   - Añadir atributos `alt` significativos a las imágenes (ya hay `alt`, mejorar su contenido).
   - Verificar jerarquía de encabezados para mantener orden lógico (h1 → h2 → h3...).

Cómo ver el proyecto
--------------------
- Abrir cualquiera de los archivos HTML en un navegador:
  - [carpeta1/home4.html](carpeta1/home4.html) (usa `main.css`)
  - [carpeta1/home.html](carpeta1/home.html)
  - [carpeta1/blog.html](carpeta1/blog.html)
  - [carpeta1/home3.html](carpeta1/home3.html)

Sugerencia de arreglo rápido para el CSS
----------------------------------------
- Revisa y corrige [carpeta1/main.css](carpeta1/main.css). Ejemplo de corrección mínima:
```css
/* ejemplo de corrección: abrir y cerrar correctamente las reglas */
.texto-article {
    font-size: 30px;
    color: purple;
}

.texto-plano {
    color: black; /* ejemplo: definir color o estilos */
}