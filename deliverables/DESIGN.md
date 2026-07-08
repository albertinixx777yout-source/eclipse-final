# Evaluación de Diseño Responsivo y Rejillas CSS

---

Analice las siguientes reglas CSS

```css

.personajes-grid {
    grid-template-columns: repeat(3, 1fr);
}

.reparto-grid {
    grid-template-columns: repeat(4, 1fr);
}

.opiniones-grid {
    grid-template-columns: repeat(3, 1fr);
}

@media (max-width: 900px) {

    .personajes-grid,
    .reparto-grid,
    .opiniones-grid {
        grid-template-columns: 1fr 1fr;
    }

    .hero-content h1 {
        font-size: 3.5rem;
    }

    .navbar {
        flex-direction: column;
        gap: 15px;
    }
}

@media (max-width: 600px) {

    .personajes-grid,
    .reparto-grid,
    .opiniones-grid {
        grid-template-columns: 1fr;
    }

    .navbar ul {
        flex-direction: column;
        text-align: center;
    }

    .hero-content h1 {
        font-size: 2.5rem;
    }

    .section {
        padding: 50px 5%;
    }
}
```

Identifique:

## Respuestas

### 1. ¿Cuántas columnas utiliza la página cuando se muestra en un monitor de escritorio?

En un monitor de escritorio, las rejillas utilizan:

- **personajes-grid:** 3 columnas.
- **reparto-grid:** 4 columnas.
- **opiniones-grid:** 3 columnas.

Esto permite aprovechar el espacio disponible en pantallas grandes y mostrar más contenido de forma organizada.

---

### 2. ¿Qué ocurre cuando el ancho de pantalla es menor a 900px?

Cuando la pantalla tiene un ancho menor a **900px**, todas las rejillas (`personajes-grid`, `reparto-grid` y `opiniones-grid`) pasan a tener **2 columnas**, facilitando la visualización en tablets y pantallas medianas.

Además:

- El título principal (`hero-content h1`) disminuye su tamaño de fuente a **3.5rem**.
- La barra de navegación (`navbar`) cambia su dirección a **columna** (`flex-direction: column`) y agrega un espacio de **15px** entre sus elementos.

---

### 3. ¿Qué ocurre cuando el ancho de pantalla es menor a 600px?

Cuando la pantalla tiene un ancho menor a **600px**, todas las rejillas pasan a tener **una sola columna**, adaptándose a dispositivos móviles.

También ocurren los siguientes cambios:

- El menú de navegación (`navbar ul`) se organiza en **columna** y centra su contenido.
- El tamaño del título principal (`hero-content h1`) disminuye a **2.5rem**.
- Las secciones (`section`) reducen su espaciado interno (`padding`) a **50px 5%**, optimizando el espacio disponible en pantallas pequeñas.
