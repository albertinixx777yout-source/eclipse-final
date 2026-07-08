# Planificación de Estilos CSS

---

## Mapeo de intrucciones técnicas, elementos html y reglas css

Mapee cada instrucción técnica con el elemento HTML afectado y la regla CSS (el selector CSS y las propiedades CSS) que debe implementarse

| Versión |   Fecha    |       Instrucción del CHANGELOG.md         | Elemento HTML en `index.html` |         Selector CSS          |     Propiedad CSS principal       |
|---------|------------|--------------------------------------------|-------------------------------|:-----------------------------:|:---------------------------------:|
| [1.0.0] | 2026-03-04 | Reinicia todos los elementos del documento.|   Todos los elementos HTML    |             `*`               | `box-sizing`, `margin`, `padding` |
|         |            |                                            |                               |                               |                                   |
|         |            |                                            |                               |                               |                                   |
|         |            |                                            |                               |                               |                                   |

# Estructura y Organización del Archivo CSS

En esta sección se describirá cómo estará organizado el archivo `styles.css` para mantener claridad, orden y facilidad de mantenimiento del código con, al menos, una regla CSS como ejemplo.

## Organización sugerida

```css
/* Reset y estilos globales */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

/* Navegación */

/* Contenido de portada */

/* Multimedia */

/* Botones */

/* Tarjetas */

/* Pie del sitio */

```
## Estrategia de Nomenclatura CSS

La siguiente tabla define la convención de nombres que se utilizará para las clases y componentes CSS del proyecto, con el propósito de mantener consistencia, claridad y facilidad de mantenimiento del código.

|       Regla General     |                    Descripción                                |  Ejemplo Correcto | Ejemplo Incorrecto |
| :---------------------- | :------------------------------------------------------------ | :---------------: | :----------------: |
| **Utilizar kebab-case** | Separar palabras con guiones medios y usar letras minúsculas. | `.video-container` | `.videoContainer` |
| **Mantener consistencia en el idioma** | Utilizar un solo idioma para todas las clases CSS del proyecto. |  |  |
| **Utilizar nombres descriptivos** | Las clases deben indicar claramente la función o propósito visual del componente. |  |  |
| **Evitar nombres ambiguos** | No utilizar nombres genéricos o poco claros. |  |  |
| **Mantener nombres reutilizables** | Crear clases que puedan reutilizarse en distintos componentes. | | |
| **Evitar abreviaciones innecesarias** | Usar nombres completos y comprensibles. | | |
