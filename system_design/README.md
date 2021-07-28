## System Design 

- Links:
    + [cheatsheet](https://gist.github.com/vasanthk/485d1c25737e8e72759f)
  

- ### ¿Qué es REST?
  * No es un protocolo ni un estándar, sino más bien un conjunto de límites de arquitectura. Los desarrolladores de las API pueden implementarlo de distintas maneras.
  * Cuando se envía una solicitud del cliente a través de una API de RESTful, esta transfiere una representación del estado del recurso requerido a quien lo haya solicitado o al extremo. La información, o representación, se entrega por medio de HTTP en uno de estos formatos: JSON (JavaScript Object Notation), HTML, XLT, Python, PHP o texto sin formato. JSON es el lenguaje de programación más popular, ya que tanto las máquinas como las personas lo pueden comprender y no depende de ningún lenguaje, a pesar de que su nombre indique lo contrario.

- ### ¿Qué es una API de REST?
  * Es una API que se ajusta a los limites de la arquitectura REST y permite interaccion con otros servicios web RESTful
  * Una API es un conjunto de definiciones y protocolos que se utiliza para desarrollar e integrar el software de las aplicaciones.Suele considerarse como el contrato entre el proveedor de información y el usuario, donde se establece el contenido que se necesita del consumidor (la llamada) y el que requiere el productor (la respuesta).Por ejemplo, el diseño de una API para un servicio meteorológico podría solicitar que el usuario escribiera un código postal y que el productor diera una respuesta en dos partes: la primera sería la temperatura máxima y la segunda, la mínima.
  * Para que una API se considere de RESTful, debe cumplir los siguientes criterios:

    - Arquitectura cliente-servidor compuesta de clientes, servidores y recursos, con la gestión de solicitudes a través de HTTP.
    - Comunicación entre el cliente y el servidor sin estado, lo cual implica que la información del cliente no se almacena entre las solicitudes de GET y que cada una de ellas es independiente y está desconectada del resto.
    - Datos que pueden almacenarse en caché y optimizan las interacciones entre el cliente y el servidor.
    - Una interfaz uniforme entre los elementos, para que la información se transfiera de forma estandarizada. Para ello deben cumplirse las siguientes condiciones:
      * Los recursos solicitados deben ser identificables e independientes de las representaciones enviadas al cliente.
      * El cliente debe poder manipular los recursos a través de la representación que recibe, ya que esta contiene suficiente información para permitirlo.
      * Los mensajes autodescriptivos que se envíen al cliente deben contener la información necesaria para describir cómo debe procesarla.
      * Debe contener hipertexto o hipermedios, lo cual significa que cuando el cliente acceda a algún recurso, debe poder utilizar hipervínculos para buscar las demás acciones que se encuentren disponibles en ese momento.
    - Un sistema en capas que organiza en jerarquías invisibles para el cliente cada uno de los servidores (los encargados de la seguridad, del equilibrio de carga, etc.) que participan en la recuperación de la información solicitada.0
    - Código disponible según se solicite (opcional), es decir, la capacidad de enviar códigos ejecutables del servidor al cliente cuando se requiera, lo cual amplía las funciones del cliente. 
