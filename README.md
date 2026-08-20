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

    Identifican recursos de manera única dentro de un sistema, son independientes del método HTTP, Deben ser claras y descriptivas, facilitando la identificación del recurso

7. ¿Por qué es recomendable usar nombres en plural para las URIs que representan colecciones de recursos?

Es recomendable usar nombres en plural para las URIs de colecciones porque sigue el principio de la consistencia semántica en arquitecturas REST

## Métodos HTTP
8. ¿Cuáles son los métodos HTTP principales utilizados en una API REST y cuál es la función de cada uno?

Los metodos principales en una API REST son: 
- GET: lee o consulta información de un recurso. No modifica los datos.
- POST: Crea un recurso nuevo en el servidor.
- PUT: Reemplaza por completo un recurso existente o lo crea si no existe.
- DELETE: Borra un recurso específico del servidor.

9. Describe la diferencia entre los métodos POST y PUT.

POST crea un nuevo recurso, mientras que PUT lo reemplaza un recurso existente

10. ¿Qué significa que un método HTTP sea idempotente? Da un ejemplo de un método idempotente.

Que un método HTTP sea idempotente significa que realizar la misma solicitud una o varias veces produce el mismo resultado en el servidor. Ejemplo: para actualizar un usuario. Si envías la misma solicitud varias veces, el usuario queda con los mismos datos.

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

Un objeto JSON está compuesto por pares clave-valor y se escribe entre llaves

15. ¿Qué tipos de datos pueden representarse en JSON?

En JSON se pueden representar strings, number, boolean, null, object y array

## Postman
16. ¿Qué es Postman y para qué se utiliza en el desarrollo de APIs?

Postman es una plataforma de software que funciona como un cliente interactivo para diseñar, probar, documentar y consumir APIs de forma visual

17. Menciona dos funcionalidades importantes de Postman que facilitan el trabajo con APIs.

Collections: Permiten agrupar y organizar peticiones HTTP relacionadas en carpetas estructuradas.
Environments: Permiten definir variables globales o específicas para diferentes contextos de desarrollo.

## Ejercicios Prácticos
18. Describe cómo implementarías una operación CRUD (Crear, Leer, Actualizar, Eliminar) en una API REST.

Para implementar un CRUD en una API REST, utilizaría métodos HTTP asociados a cada operación:
- Crear: POST /usuarios para registrar un nuevo usuario.
- Leer: GET /usuarios para obtener todos, o GET /usuarios/{id} para uno específico.
- Actualizar: PUT o PATCH /usuarios/{id} para modificar sus datos.
- Eliminar: DELETE /usuarios/{id} para borrar un usuario.


19. ¿Cómo usarías Postman para probar una nueva API que acabas de desarrollar?

Usaría Postman para comprobar que cada endpoint de la API funciona correctamente:
- Crear una colección con los endpoints de la API.
- Probar POST para crear datos y verificar la respuesta.
- Probar GET para consultar los datos creados.
- Probar PUT/PATCH para modificarlos.
- Probar DELETE para eliminarlos.
- Revisar los códigos HTTP, respuestas JSON, headers y mensajes de error.
- Probar también casos incorrectos, como datos faltantes o IDs inexistentes, para comprobar el manejo de errores.
Si la API requiere autenticación, configurar en Postman los tokens o credenciales correspondientes.


20. Propone un ejemplo de una API REST para gestionar un catálogo de productos y describe brevemente los endpoints necesarios.

Un ejemplo sería una API REST para gestionar un catálogo de productos.

Endpoints principales:

    POST /productos → Crear un producto.
    GET /productos → Obtener todos los productos.
    GET /productos/{id} → Obtener un producto específico.
    PUT /productos/{id} → Actualizar un producto.
    DELETE /productos/{id} → Eliminar un producto.
    GET /productos?categoria=electronica → Filtrar productos por categoría.

Cada producto podría tener datos como id, nombre, descripción, precio, categoría y stock. La API devolvería las respuestas en formato JSON y utilizaría códigos HTTP para indicar si las operaciones fueron exitosas o si ocurrió algún error.
