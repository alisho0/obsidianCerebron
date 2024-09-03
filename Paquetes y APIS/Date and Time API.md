
Una API interesante que tiene Java es el paquete java.time. Esta se divide en varias clases:
- LocalDate
- LocalTime
- LocalDateTime
- ZoneDateTime (Misma función que la anterior, pero con valores de acuerdo a la zona horaria)
- ZoneId: Para definir la zona horaria.
- Duration: Representa el tiempo en nanosegundos
- Period: Se utiliza para expresar el tiempo en unidades como el año. 
- Instant: Se utiliza para representar la instancia de una hora (marca de tiempo), y es mejor usarlo en las API de registro y las tareas del sistema. ***(CHEQUEARLO A FUTURO)***
- DateTimeFormatter: Te puede servir para establecer como se deben mostrar algunas fechas. Puede darse el formato de forma manual o automática según la configuración regional en el caso de usar la clase [[Locale Class|Locale]].

**Dato**: En Java 8 se introducen nuevas APIs para Date and Time para abordar mejor las deficiencias de los antiguos _java.util.Date_ y _java.util.Calendar_.

Algunos métodos que se pueden ver son: 
+ .now te muestra lo actual, sea de Date, Time o DateTime.
+ .of donde indicas una fecha, hora o ambas.
+ .plusX te sirve para incrementar ya sea año, mes, hora, segundo, etc.
+ .isBefore/.isAfter sirve para comparar una fecha con la otra. Retorna un booleano.
+ .getX y no hace falta que lo explique
+ .between (Period) te marca la distancia que hay entre un año/mes/dia y otro.
+ .withZoneSameInstant (ZonedDateTime) encuentra cuál era la fecha y la hora en determinado lugar.


*Dato*: Al usar .format y cambiar a otro patrón, hay que guardarlo en un String.
