# Multi AI Agent Systems with crewAI

## Introduction

Ejemplo: Sistema multiagente para conseguir y preparar entrevistas de trabajo IT.

### ¿Qué es la Automatizacion mediante agentes?

- La automatización determinista mediante código tiene a complicarse conforme se añaden condiciones.

#### Diferencias entre el desarrollo tradicional y el desarrollo AI

| | Desarrollo Tradicional | Desarrollo AI |
|:--|:--|:--|
| Entradas| Conocimiento claro de los inputs a priori | **Entradas difusas**: las desconocemos a priori|
| Transformaciones | Cálculos matemáticos, flujos deterministas y controlados | **Transformaciones difusas**: no sabemos exactamente que hará el LLM |
| Salidas | Conocimiento claro de la salida esperada | **Salidas difusas**: el resultado obtenido puede adoptar múltiples formatos |
| Notas | El comportamiento puede ser replicado | Al ser un modelo **probabilistico** cada vez puede ser diferente|

### Ejemplos de aplicaciones

#### Recopilación y análisis de datos

En la **aproximación tradicional** se aplican una serie de reglas a posibles clientes que han conectado con una empresa a través de su formulario de contacto para realizarles ofertas.

En la **aproximación mediante agentes IA** se puede tener un grupo de agentes que **investiguen** (research) sobre los potenciales clientes, los comparen con los clientes actuales (comparasion), los puntuen (scoring) y determinen qué temas les pueden interesar (talking points)

![alt text](image.png)
