# Calculadora de estructuras

Aplicación web para análisis de estructuras planas. El menú principal ofrece tres módulos: **Cerchas**, **Vigas** y **Pórticos**.

## Autoría

**Autor del proyecto: Alejandro Morales.** El código inicial de cerchas fue creado por un compañero de clase y se incorporó con su autorización para atribuir el proyecto a Alejandro, modificarlo y ampliarlo.

## Abrir la aplicación

Abre [index.html](index.html) en un navegador moderno. No requiere instalación ni dependencias externas.

- **Cerchas:** [cerchas.html](cerchas.html), la calculadora existente de método matricial 2D.
- **Vigas:** [vigas.html](vigas.html), módulo inicial inspirado en el flujo de DSNWinbeam.
- **Pórticos:** [porticos.html](porticos.html), sección vacía reservada para una futura versión.

## Módulo de vigas

Introduce longitud, módulo E, inercia, apoyos y cargas. Permite cargas puntuales, momentos y cargas distribuidas uniformes o lineales. Informa reacciones, equilibrio, cortante, momento flector, giro y flecha.

El solver usa elementos de viga Euler–Bernoulli y rigidez directa, con subdivisiones de cálculo y nodos adicionales en posiciones de cargas y apoyos. Es una primera versión funcional; todavía no replica todas las opciones de DSNWinbeam ni se ha validado para diseño profesional. La referencia consultada describe el método de rigidez directa y los resultados de equilibrio y diagramas del programa: [FAQ de DSNWinbeam](https://dsnwinbeam.weebly.com/faq.html).

## Hoja de ruta

1. Contrastar los resultados del módulo de vigas con casos analíticos y referencias independientes.
2. Separar interfaz, modelo, solver y gráficos en módulos.
3. Incorporar más opciones de apoyos, tipos de sección y edición de cargas.
4. Añadir guardado e importación/exportación de modelos.
5. Implementar el análisis de pórticos 2D compartiendo el solver y la visualización.

## Alcance

La calculadora actual es educativa y de apoyo al cálculo. Sus resultados deben contrastarse con casos de referencia y criterio profesional antes de usarse para decisiones de diseño estructural.
