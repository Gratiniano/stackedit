

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

Un ejemplo de extracción e interpretación

** Datos no estructurados**

	 Hi,  
	  
	I would like to report a damage and ask you to compensate me.  
	  
	Yesterday, while playing with a friend, my 9-year-old son Rajad kicked a soccer ball against the chandelier in the living room, which then broke from its holder and fell onto the floor and shattered (it was made of glass).  
	  
	Luckily no one is injured, but the chandelier is damaged beyond repair.  
	  
	Attached is an invoice and some images of the destroyed chandelier.
	
	Deepak Jamal  
	contract no: HC12-223873923  
	123 Main Street  
	10008 New York City  
	(718) 123 45678


**Salida del modelo: datos estructurados en JSON**
	{  
		"name":  "Deepak",  
		"surname":  "Jamal",  
		"address":  "123 Main Street, 10008 New York City, NY",  
		"phone":"+1 718 123 45678",  
		"contract_no":  "HC12-223873923",  
		"claim_description":  "Yesterday [Dec-8, 2024], while playing with a friend, my 9-year-old son Rajad kicked a soccer ball against the chandelier in the living room, which then broke from its holder and fell onto the floor and shattered (it was made of glass).\nLuckily no one is injured, but the chandelier is damaged beyond repair.\n"  
	}

### 3. Llamar a servicios externos, haciendo que el contexto sea persistente

- Para poder generar una respuesta suele ser necesario acceder a datos corporativos o bases de datos externas.
- Para generar un contexto persistente, también debe poder escribirse en sistemas y bases de datos.

![](https://miro.medium.com/v2/resize:fit:1050/1*UjA1UCxseKtTDiZWDjmVWg.png)


### 4. Evaluación, RAG, razonamiento y confianza

El correcto desempeño de los trabajos administrativos consiste en interpretar los casos entrantes en base a las reglas a aplicar.
Para proporcionar estas reglas usaremos una **base de datos vectorial** mediante RAG.

Es conveniente reflejar el razonamiento.
- para fundamentar la respuesta al cliente.
- para ayudar a los ajustes de ingeniería.
- para comprobaciones

#### Confianza

- Si el modelo estima su confianza, se puede establecer un umbral por debajo del cual los casos necesitarán un soporte humano.
- Un umbral de confianza alto garantiza errores mínimos pero mayor procesamiento manual.
- Un umbral de confianza bajo permite que más casos se procesen automáticamente pero con un mayor riesgo de errores.

![](https://miro.medium.com/v2/resize:fit:1500/1*-kJEBbVKpueHaNxEmvlLXw.png)






 
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA1NzI5MTI0MSwtMTIyMDQzODcyNCw5MD
gxMTQ4OTddfQ==
-->