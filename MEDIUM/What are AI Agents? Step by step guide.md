

# ¿Que son los agentes AI? Guía paso a paso.

## Características de los agentes AI
- Pueden procesar un problema complejo (ej. reclamo seguro) de principio a fin.
	- comprender texto, imagenes o archivos.
	- recuperar información de la bbdd.
	- comparar el caso con los términos y condiciones del seguro.
	- hacer preguntas y esperar respuestas sin perder contexto (aún en periodos largos de tiempo).
- Funcionan de forma autónoma.

*Diferencias entre IA Generativa Tradicional y de Agentes*
![](https://miro.medium.com/v2/resize:fit:1050/1*7rWViLLiWpoHivd15UHZTQ.png)

## Anatomía de un Agente de IA
Se usa el ejemplo del agente para el rpcoeso de seguros.

### 1. Clasificación y envío de un trabajo a las líneas de procesamiento.

La clasificación asigna el texto a una categoría predefinida.

 - El flujo de trabajo comienza cuando se recibe el mensaje de un cliente.
 - El agente analiza el contenido y determina qué quiere el cliente.
 - En base a la clasificación inicia una línea de procesamiento
 ![](https://miro.medium.com/v2/resize:fit:1500/1*CvV2Yu0Nk43LN7GUDO8JPQ.png)
 
 ### 2. Extracción de datos
 
 La extracción implica la lectura e interpretación de los datos del texto.
 
Convertir los datos no estructurados en datos estructurados ayuda a que el proceso sea sistemático, seguro y protegido. P.ej. normalizando el formato de los datos.

![](https://miro.medium.com/v2/resize:fit:1050/1*Q8o6a2-Fe1FbqIOS7I3EaQ.png)

Un ejemplo de extracción e intetrpretación

|Datos no estructurados|  |
|--|--|
| Hi,

I would like to report a damage and ask you to compensate me.  
Yesterday, while playing with a friend, my 9-year-old son Rajad kicked a soccer ball against the chandelier in the living room, which then broke from its holder and fell onto the floor and shattered (it was made of glass). |  |

| datos no estructurados |
|:--|
|Hi, 
I would like to report a damage and ask you to compensate me.    
Yesterday, while playing with a friend, my 9-year-old son Rajad kicked a soccer ball against the chandelier in the living room, which then broke from its holder and fell onto the floor and shattered (it was made of glass).  
  
Luckily no one is injured, but the chandelier is damaged beyond repair.  
  
Attached is an invoice and some images of the destroyed chandelier.  
  
Deepak Jamal  
contract no: HC12-223873923  
123 Main Street  
10008 New York City  
(718) 123 45678 |
||







 
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMzNzEzODQwMV19
-->