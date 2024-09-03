A causa de algunas situaciones reales que eran complicadas de representar con el modelo E-R básico, se incorporaron dos nuevos elementos, produciendo lo que se conoce como **Modelo Entidad - Relación Extendido (MERE)**.
Este modelo incluye lo ya visto en el modelo E-R y conceptos de herencia (superclase, subclase, etc).

#### Superentidad
Se refiere básicamente a la superclase o padre, la cual contiene los mismos atributos que tendrán sus entidades hijas (no necesariamente todos).
#### Subentidad
Es la entidad hija (subclase) que contiene los atributos del padre y sus propios atributos únicos.

### Generalización
Se refiere a la relación extendida que hay entre el conjunto de nivel más alto (padre) y uno o más conjuntos de nivel más bajo (hijos). 
Dicha generalización permite que los hijos hereden los atributos del padre, donde **normalmente el padre tiene un atributo clave distinto de sus hijos**.
Todo esto permite la eliminación de redundancia de atributos al agrupar atributos similares.
### Especialización
Es el proceso por el que se definen las subentidades de una superentidad. Este proceso te permite:
- Definir subconjuntos
- Asociar atributos específicos, adicionales en cada sub-entidad.
- Establecer relaciones específicas

==***OJO: La especialización se da en un proceso de diseño descendente mientras que la generalización en un proceso de diseño ascendente.***==

Pregunta: ¿La especialización y generalización son un concepto o es un tipo de funcionabilidad?
Mi respuesta: Especialización es un proceso, yo mismo lo puse y  generalización no sé, es un tipo de ventaja?
¿Por qué la generalización es un proceso ascendente?.


### Restricciones de disyunción
Especifica que las entidades hijas deben ser disjuntas y se especifica dentro del triángulo con la letra "d". De caso contrario no se especifica o se pone la letra "o".

- **Disjunta**: Una entidad no puede pertenecer a más de un conjunto de entidades de nivel más bajo.
- **Solapada**: La misma entidad puede pertenecer a más de un conjunto de entidades de nivel más bajo.
