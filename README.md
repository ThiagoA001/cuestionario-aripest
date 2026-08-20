# Cuestionario sobre API REST

## Conceptos Básicos
1. ¿Qué es una API y cuál es su función principal?

API significa Interfaz de Programación de Aplicaciones y su principal funcion es permitir la comunicación entre diferentes sistemas de software.

2. Define brevemente el estilo arquitectónico REST.

REST es es una lógica de restricciones y recomendaciones bajo la cual se construye la API

3. ¿Qué significa que una API sea RESTful?

Una API que sea RESTFULL significa que cumple con todas las restricciones

## Recursos y URIs
4. ¿Qué es un recurso en el contexto de una API REST?

Un recurso es, en API REST, cualquier pieza de información o entidad que el servidor puede nombrar, almacenar y exponer

5. Explica la importancia de las URIs en una API REST.

Las URIS son importantes ya que son un identificador unico lo cual significa que cualquier recurso puede ser
accesible a través de un URL único.

6. Menciona tres características importantes de las URIs.



7. ¿Por qué es recomendable usar nombres en plural para las URIs que representan colecciones de recursos?



## Métodos HTTP
8. ¿Cuáles son los métodos HTTP principales utilizados en una API REST y cuál es la función de cada uno?

Los metodos principales en una API REST son: 
GET: lee o consulta información de un recurso. No modifica los datos.
POST: Crea un recurso nuevo en el servidor.
PUT: Reemplaza por completo un recurso existente o lo crea si no existe.
DELETE: Borra un recurso específico del servidor.

9. Describe la diferencia entre los métodos POST y PUT.

POST crea un nuevo recurso, mientras que PUT lo reemplaza un recurso existente

10. ¿Qué significa que un método HTTP sea idempotente? Da un ejemplo de un método idempotente.



## Códigos de Estado HTTP
11. ¿Qué indican los códigos de estado en las respuestas HTTP de una API REST?

Los codigos de estado indican si la petición tuvo éxito, si faltan datos, si hay un fallo en el servidor o si se requiere un paso adicional

12. Da un ejemplo de un código de estado para cada una de las siguientes categorías y explica su significado: 
    - 2xx (Éxito)
      200 La solicitud tuvo éxito
    - 4xx (Errores del cliente)
      404 El servidor no pudo encontrar el recurso solicitado
    - 5xx (Errores del servidor)
      500 El servidor encontró una condición inesperada que le impidió completar la solicitud.
## JSON
13. ¿Por qué es JSON el formato de datos más comúnmente utilizado en las APIs REST?

JSON es el formato estándar en las APIs REST principalmente por su simplicidad y eficiencia.

14. Explica brevemente la estructura de un objeto JSON.



15. ¿Qué tipos de datos pueden representarse en JSON?



## Postman
16. ¿Qué es Postman y para qué se utiliza en el desarrollo de APIs?
17. Menciona dos funcionalidades importantes de Postman que facilitan el trabajo con APIs.

## Ejercicios Prácticos
18. Describe cómo implementarías una operación CRUD (Crear, Leer, Actualizar, Eliminar) en una API REST.
19. ¿Cómo usarías Postman para probar una nueva API que acabas de desarrollar?
20. Propone un ejemplo de una API REST para gestionar un catálogo de productos y describe brevemente los endpoints necesarios.
