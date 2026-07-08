# Planificación de Estilos CSS

---

## Mapeo de intrucciones técnicas, elementos html y reglas css

Mapee cada instrucción técnica con el elemento HTML afectado y la regla CSS (el selector CSS y las propiedades CSS) que debe implementarse

| Versión | Fecha | Instrucción del CHANGELOG.md | Elemento HTML en `index.html` | Selector CSS | Propiedad CSS principal |
|----------|--------|------------------------------|-------------------------------|--------------|--------------------------|
| [1.0.0] | 2026-03-04 | Reinicia todos los elementos del documento. | Todos los elementos HTML | `*` | `box-sizing`, `margin`, `padding` |
| [1.1.0] | 2026-03-11 | Modifica el selector por clase `.logo` y cambia el color del texto a dorado. | Elemento con clase `logo` | `.logo` | `color` |
| [1.2.0] | 2026-03-18 | Modifica el selector `.navbar` usando flexbox y alineación horizontal. | Barra de navegación `<nav class="navbar">` | `.navbar` | `display`, `justify-content`, `align-items` |
| [1.3.0] | 2026-03-25 | Modifica los enlaces `.navbar a` eliminando subrayado y usando negrita. | Enlaces dentro de `.navbar` | `.navbar a` | `text-decoration`, `font-weight` |
| [1.4.0] | 2026-04-01 | Agrega efecto hover en `.navbar a:hover` cambiando color a dorado. | Enlaces del menú de navegación | `.navbar a:hover` | `color` |
| [1.5.0] | 2026-04-08 | Modifica la clase `.btn` agregando fondo dorado, padding y bordes redondeados. | Botones con clase `btn` | `.btn` | `background`, `padding`, `border-radius` |
| [1.6.0] | 2026-04-15 | Define espaciado general para `.section` usando padding. | Secciones con clase `section` | `.section` | `padding` |

# Estructura y Organización del Archivo CSS

En esta sección se describirá cómo estará organizado el archivo `styles.css` para mantener claridad, orden y facilidad de mantenimiento del código con, al menos, una regla CSS como ejemplo.

## Organización sugerida

```css
/* Reset y estilos globales */
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

/* Navegación */
.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

/* Contenido de portada */
.hero{
    padding:40px;
}

/* Multimedia */
.video-container{
    width:100%;
}

/* Botones */
.btn{
    background:#e2b450;
    border-radius:8px;
}

/* Tarjetas */
.card{
    padding:20px;
}

/* Pie del sitio */
.footer{
    text-align:center;
}
```
## Estrategia de Nomenclatura CSS

La siguiente tabla define la convención de nombres que se utilizará para las clases y componentes CSS del proyecto, con el propósito de mantener consistencia, claridad y facilidad de mantenimiento del código.

| Regla General | Descripción | Ejemplo Correcto | Ejemplo Incorrecto |
|----------------|-------------|------------------|--------------------|
| **Utilizar kebab-case** | Separar palabras con guiones medios y usar letras minúsculas. | `.video-container` | `.videoContainer` |
| **Mantener consistencia en el idioma** | Utilizar un solo idioma para todas las clases CSS del proyecto. | `.video-container` | `.contenedor-video` |
| **Utilizar nombres descriptivos** | Las clases deben indicar claramente la función o propósito visual del componente. | `.hero-content` | `.caja1` |
| **Evitar nombres ambiguos** | No utilizar nombres genéricos o poco claros. | `.navigation-menu` | `.item` |
| **Mantener nombres reutilizables** | Crear clases que puedan reutilizarse en distintos componentes. | `.section-title` | `.titulo1` |
| **Evitar abreviaciones innecesarias** | Usar nombres completos y comprensibles. | `.video-container` | `.vid-cont` |
