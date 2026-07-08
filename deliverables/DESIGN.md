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

* ¿Cuántas columnas utiliza la página se muestra en un monitor de escritorio?
* ¿Qué ocurre cuando el ancho de pantalla es menor a 900px?
* ¿Qué ocurre cuando el ancho de pantalla es menor a 600px?