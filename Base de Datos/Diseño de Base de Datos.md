
A la hora de diseñar una base de datos, es algo que tiene su complejidad al seguir una serie de pasos para que sea un trabajo correcto, ya que el propósito del diseño es producir modelos físicos y lógicos para el sistema de la BD.

Aquí se pueden ver las fases del diseño de una base de datos:
![[fasesDiseñoBD.png]]

En este caso veremos el modelo [[Entidades|Entidad]] Relación para el diseño de la base de datos, ya que tiene una notación gráfica, semántica clara, es fácil de entender e independiente de cualquier SGBD.

---
### Las entidades
Con ellas vamos a encontrar dos tipos, físicas y conceptuales, las cuales deben seguir ciertas reglas:
- Nombre en singular.
- Un conjunto de entidades o tipo entidad es un conjunto de entidades que comparten las mismas propiedades.

### Las relaciones
Aquí vemos la relación entre las [[Entidades|entidades]], donde la relación se representa con un rombo *(se recomienda usar verbos en el rombo)*.
Hay veces que se da lugar a que las relaciones tengan atributos, llamándose como *entidad asociativa* la cual contiene atributos que son peculiares de la relación.
También se pueden dar casos de grado en una relación, es decir, el número de entidades participantes en una relación.

#### Restricciones en las relaciones
Se limitan las combinaciones de entidades que pueden participar, donde obviamente esto depende de la situación a la cual se esté modelando. A la hora de modelar se considera lo siguiente: 
- Cardinalidad: Entidades que pueden participar en la relación (1:1, 1:N, N:M)
![[Cardinalidad.png]]
- Participación: Específica cuando la existencia de una entidad X depende de la existencia de otra entidad Y. Donde podemos encontrar dos tipos, parcial o total.![[Participacion.png]]
---
### Cuestiones de Diseño
A considerar los siguientes puntos a la hora de diseñar:
- Los atributos pertenecen a las entidades o a las relaciones.
- Las relaciones y las entidades deben tener nombres únicos.
- Los atributos deben tener nombres únicos dentro de una entidad o relación, no necesariamente dentro del esquema.
- Las relaciones deben darse entre al menos dos conjuntos de entidades.
- El nombre de un rol, debe ser único y distinto tanto de la entidad como de la relación.

