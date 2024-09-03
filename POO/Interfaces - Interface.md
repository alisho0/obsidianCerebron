
Hablamos de interfaces a algún tipo de "[[Clases]]" donde funciona como una plantilla para las clases. 
Aquí solo se pueden definir los métodos y si o si la clase que los implemente debe darles un Override.

Las únicas que no van a ser obligatorias son la *default* porque no es obligatoria aunque se la puede reescribir y después la *static* que pertenece a la inferfaz, no a la clase que la implementa. O sea digamos, que la puedes llamar aunque no lo implementes creo.
Ojito que se pueden implementar varias interfaces, pero hay que tener en cuenta que al hacer esto debemos implementar a cada uno de sus métodos.


Características:

- Evitar poner variables aunque se puede. (Tiene sentido porque las clases pueden ir variando en sus variables).
- Las variables y métodos son PUBLICOS.
- No se especifica la implementación de un método, solo lo creas digamos.


DATO: En Java 8 se agrega el *default* para evitar que al agregar métodos nuevos a la interfaz se genere un error de compilación por la falta de implementación del nuevo método. En Java 8 se agrega este tipo de método que tiene su implementación dentro de la interfaz misma, evitando que se generen errores y pudiendo agregar métodos tranqui.

