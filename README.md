# Tecnologico de Costa Rica

Estudiante: Jose Andres Solano Vargas
Curso: Introduccion al desarrollo de sowftware

---

## 📑 Estructura Semántica

Lista de etiquetas clave utilizadas y su propósito:

- `<header>` – Encabezado principal del sitio, incluye el logo y navegación.
- `<nav>` – Menú de navegación entre secciones.
- `<main>` – Contenido principal de la página.
- `<section>` – Agrupación de contenido relacionado.
- `<article>` – Contenido independiente o destacado.
- `<footer>` – Información de contacto y pie de página.

---

## 🌐 URL pública (Netlify)

dancing-trifle-fa13da.netlify.app

---

## ✅ Validación W3C

**Captura:**  
![Captura de Validación W3C](assets/W3Cindex1.png)

**Resumen del html principal:**  
En su totalidad la estructura del index prinicpal es correcta, solo el caso de un mismo warning por falta de etiquetas heading(h2-h6). Ademas de un Error por el uso de border el cual aparentemente esta obsoleto.

**Captura:**  
![Captura de Validación W3C](assets/Screenshot%202025-08-14%20212851.png)

**Resumen del html registro:**  
El registro no presento ningun warning ni error por lo que se optuvo un 100% de calificacion.

---

## 📊 Lighthouse

**Puntuaciones obtenidas:**

![Captura Lighthouse](assets/Screenshot%202025-08-14%20214323.png)

**Plan de mejoras:**

- Se debera arreglar los warning aunque estos no reflejen un problema significativo en el lightning.
- Se cambio el

---

## ♿ Accesibilidad Aplicada

Acciones implementadas para mejorar la accesibilidad del sitio:

- **`tabindex`** → _[Explica dónde y por qué lo usaste]_
- **`aria-*`** → _[Describe qué atributos aria utilizaste y en qué elementos]_
- **`alt`** en imágenes → _[Ejemplo de uso y justificación]_
- **Enlaces descriptivos** → _[Ejemplos de textos de enlace claros y accesibles]_

**Captura de ejemplo de accesibilidad:**  
![Captura Accesibilidad](assets/img/accesibilidad.png)

---

## 🎨 Resumen de selectores y propiedades aplicados

### Selectores de tipo

`header`, `nav`, `section`, `footer`, `main`, `aside`, `img`, `table` → usados en la estructura principal de las páginas.

### Selectores de clase

- `.nombre-sitio` → en el título principal.
- `.btn-nav` → en enlaces de navegación.
- `.registro` → sección del formulario de registro.
- `.nav-principal`, `.contenedor`, `.hero` → estructura general.
- `.producto`, `.texto-producto`, `.precio`, `.btn-compras` → en los productos.
- `.site-footer`, `.grid-footer`, `.footer-menu`, `.copyright` → en el footer.

### Selectores de ID

- `#agenda` → sección con la tabla de promociones.
- `#sobre-nosotros` → sección de descripción de la empresa.

### Selectores de atributo

- `a[target="_blank"]` → en enlaces externos (ej. Instagram, TEC, WhatsApp).
- `img[alt]` → aplicado en todas las imágenes de productos y categorías para accesibilidad.
- `button[aria-label]` → en el botón de enviar en el formulario de registro.

### Combinadores

- `.footer-menu a + a` → para espaciar enlaces dentro del footer.
- `.producto p` → para dar estilo al texto dentro de cada tarjeta de producto.

### Pseudo-clases de estado

- `a:hover` → aplicado en enlaces de navegación y productos.
- `.btn-compras:hover` → efecto en los botones de agregar al carrito.
- `.btn-nav:focus-visible` → accesibilidad en la navegación por teclado.

### Pseudo-clases estructurales

- `ul li:first-child` → aplicado en patrocinadores para estilo del primer ítem.
- `tr:nth-child(even)` → alternancia de filas en la tabla de agenda de promociones.

### Especificidad

- `!important` aplicado en ajustes de overrides.css.
- `style="..."` inline en algunos elementos de prueba (ejemplo: ajustes rápidos en headings).

### Box model

- `.producto`, `.registro`, `.footer-menu a` → aplican `margin`, `padding`, `border`, `border-radius`.
- `#registro button` → usa `padding` para hacerlo más alto y ancho.

### Overflow

- `.registro` → `overflow-x: hidden` para controlar desbordamiento horizontal.
- `.texto-producto p` → pensado para textos largos dentro de las tarjetas.

### Flexbox

- `.nav-principal` → organiza enlaces en fila con `display: flex; justify-content: space-between;`.
- `.footer-menu` → organiza verticalmente enlaces con `flex-direction: column;`.

### Grid

- `.grid-footer` → organiza columnas del footer.
- `.listado-categorias` y `.listado-productos` → organizan tarjetas de categorías y productos en rejilla.

### Position relative/absolute

- `.registro` → `position: relative;` como contenedor.
- `#registro::after` → ejemplo de `position: absolute;` para mostrar un texto decorativo.
- `.hero .etiqueta` (en CSS extra) → para destacar texto sobre la imagen principal.
