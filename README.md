# Api del Clima CieloScopio


![UML CieloScopio](https://github.com/jihuder/cieloscopio-api-java/blob/main/imagenes/UML-CieloScopio-api.jpg?raw=true)


Se comienza con la clase Principal en donde se ejecuta el aplicativo. Pasamos a la capa CONTROLLER en donde hay una clase Búsqueda, la cual  es el controlador que llama los métodos de las otras dos clases de Clima y Ubicación, los cuales se llaman en  determinada línea de tiempo. Se hace una capa MODELOS en donde ubicamos las clases Clima y Ubicación, cuyo objetivo es asociar los datos que necesitaremos de la API para darle una estructura. Esto es debido a que la API nos envía muchos datos, de los cuales utilizaremos algunos. También haremos la manipulación de esos datos, pidiendo y recibiendo la comunicación de la API, cumpliendo la lógica de negocio del requerimiento puntual dentro de esta capa, aparte, se crea una interfaz debido a que estas dos clases que la firman tiene el mismo método cuyo propósito es el mismo y devuelven el mismo tipo de dato. No se HACE una capa DTO porque no vamos a enviar información entre capas, ya que no tenemos Frontend y tampoco vamos a enviar la información por HTTP. Tampoco se hace una capa de ENTIDAD porque no vamos a utilizar una base de datos en nuestro sistema o registrarlo dentro. 

Tenemos que aclarar que la capa de MODELOS no  nos sirve para la capa de ENTIDAD, porque tienen propósitos diferentes. La capa MODELOS nos sirve para agrupar los datos y hacer la lógica de negocio de una entidad, mientras que la capa de ENTIDAD nos sirve para registrar esa entidad en base de datos. Aunque las dos pueden tener la misma estructura, sus propósitos son totalmente diferentes y van a tener cambios a medida que se vaya desarrollando el aplicativo.


