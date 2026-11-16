# Tarea: Mi prompt avanzado

Herramienta de IA usada: **Gemini**

## Tarea elegida

Explicar un error de compilación

## Version 1: prompt basico

```text
Explica uno de los errores más comunes al compilar
```

## Version 2

```text
<rol> Actúa como un ingeniero de software senior. </rol>
<contexto> Explica uno de los errores más comunes al compilar. </contexto>
<tarea> Respecto al error común, dime los factores por lo cual sucede y los lenguajes de programación donde más ocurre este tipo de error. </tarea>
```

> Usé la técnica del Role Promptng y del Prompt Estructurado porque permite escribir una instrucción más organizada y precisa obteniendo respuestas menos ambiguas y de mayor calidad.

## Version 3: prompt final

•	Un prompt final que combine al menos tres técnicas de la sesión: few-shot, chain of thought, role prompting, descomposición, prompt estructurado o autocrítica.

•	Un rol específico (no "experto") y un formato de respuesta definido.

```text
Paso 1: Actúa como un ingeniero de software senior. Explica uno de los errores más comunes al compilar.
Paso 2: Con el error común, explica los factores por el cual sucede el error.
Paso 3: Haz una tabla que muestre los lenguajes de programación donde más frecuentan este tipo de error.
Paso 4: Revisa tu tabla y verifica que no falte ningún lenguaje de programación e indica cuales agregaste.
```

> Sé agregó la técnica de la Descomposición porque permite ordenar las instrucciones paso a paso, con estas subtareas se obtuvo una mayor precisión y detalle en cada respuesta hecha por la IA, además se agrego una Autocrítica para que la IA revise su propia repuesta, enucentre errores y entregue una versión mejorada.

## Técnicas usadas en el prompt final

•	Una tabla que indique qué parte del prompt final corresponde a cada técnica.

| Partes del Prompt Final | Técnicas Usadas |
|-------------------------|---------------|
| Actúa como un ingeniero de software senior. Explica uno de los errores más comunes al compilar. | Role Prompting, Descomposición, Prompt Estructurado |
| Con el error común, explica los factores por el cual sucede el error. | Descomposición, Prompt Estructurado |
| Haz una tabla que muestre los lenguajes de programación donde más frecuentan este tipo de error. | Descomposición, Prompt Estructurado |
| Revisa tu tabla y verifica que no falte ningún lenguaje de programación e indica cuales agregaste. | Descomposición, Autocrítica |

## Evaluación del resultado

•	Una tabla de evaluación del resultado con al menos cuatro criterios (Sí / No).

| Revisión | ¿Cumple?|
|---------|--------------------------------|
| ¿Incluye soluciones para evitar el error? | Si |
| ¿La tabla incluye una explicación para cada lenguaje de programación? | Si |
| ¿Indica qué otros lenguajes de programación se agregaron en la autocrítica? | Si |
| ¿Hay algún lenguaje de programación que se haya repetido? | No |

## Por que elegí estas técnicas

- Role Prompting, la escogí para que la IA adopte una personalidad más profesional y se oriente para el nivel de detalle en las respuestas.
- Prompt Estructurado, porque al usarlo se obtiene una respuesta adaptada a lo que necesitamos
- Autocrítica, para obtener respuestas menos superficiales y que la IA nos genere datos falsos.
- Descomposición, porque así la IA no tiene que pensar todo de golpe lo cual puede generar respuestas erróneas.