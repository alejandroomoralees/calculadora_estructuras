# Calculadora de estructuras

Aplicación web para modelar y analizar estructuras planas. El proyecto parte de una calculadora de cerchas 2D y se ampliará para incorporar vigas y pórticos.

## Autoría

**Autor del proyecto: Alejandro Morales.** El código inicial fue creado por un compañero de clase y se ha incorporado a este repositorio con su autorización para atribuir el proyecto a Alejandro, modificarlo y ampliarlo.

## Uso actual

Abre [index.html](index.html) directamente en un navegador moderno. No necesita instalación ni dependencias externas.

La aplicación permite definir:

- Nodos con coordenadas X e Y en metros.
- Barras con módulo de elasticidad E en GPa y área en m².
- Apoyos articulados o deslizantes.
- Cargas nodales Fx y Fy en kN.

Calcula desplazamientos, reacciones y esfuerzos axiles. El modelo actual representa cerchas ideales 2D con análisis estático lineal; no incluye flexión ni pandeo.

## Desarrollo

El código actual está contenido en `index.html` para mantener intacta la calculadora recibida. La siguiente etapa será separar la interfaz, el modelo estructural, el solver y el dibujo para que los nuevos tipos de elemento puedan compartir la aplicación:

1. Mantener y documentar el solver de cerchas.
2. Diseñar grados de libertad nodales que incluyan giro.
3. Añadir elementos de viga y pórtico con rigidez axial y a flexión.
4. Incorporar casos de referencia para contrastar los resultados.
5. Añadir guardado e importación/exportación de modelos.

## Alcance

Esta herramienta es educativa y de apoyo al cálculo. Sus resultados deben revisarse con casos de referencia y con criterio profesional antes de usarse para decisiones de diseño estructural.
