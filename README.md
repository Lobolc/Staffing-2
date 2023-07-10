# Staffing-2

Este es un planificador de turnos, que toma los datos de unos archivos de Excel y devuelve un CSV con los turnos semanales de cada trabajador.

Descripción del problema

Supongamos que tenemos un centro de monitoreo que debe funcionar las 24 horas del día, y que tenemos una cantidad mínima de trabajadores necesarios, en nuestro caso son 52 monitoristas y 4 jefes de turno, para hacerlo funcionar en dos turnos, turno de día y turno de noche. Tenemos que crear un programa de turnos que esté sujeto a ciertas restricciones.

En este caso, las restricciones añadidas son:

$\bullet$ Tenemos cada monitorista y su disponibilidad semanal (todos están siempre disponibles) en un fichero Excel, junto con su "score de productividad" (de 1 a 100).

$\bullet$ Los días de trabajo están separados en dos turnos de 12 horas (lunes 07:00 - lunes 19:00, lunes 19:00 - martes 07:00, martes 07:00 - martes 19:00, martes 19:00 - miércoles 07:00, miércoles 07:00 - miércoles 19:00, miércoles 19:00 - jueves 07:00, jueves 07:00 - jueves 19:00, jueves 19:00 - viernes 07:00, viernes 07:00 - viernes 19:00, viernes 19:00 - sábado 08:00, sábado 08:00 - sábado 20:00, sábado 20:00 - domingo 08:00, domingo 08:00 - domingo 20:00, domingo 20:00 - lunes 07:00).
