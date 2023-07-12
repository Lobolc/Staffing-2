# Staffing-2

Este es un planificador de turnos, que toma los datos de unos archivos de Excel y devuelve un CSV con los turnos semanales de cada trabajador.

Descripción del problema

Supongamos que tenemos un centro de monitoreo que debe funcionar las 24 horas del día, y que tenemos una cantidad mínima de trabajadores necesarios, en nuestro caso son 48 monitoristas, 4 jefes de turno y 1 persona de altas, para hacerlo funcionar en dos turnos, turno de día y turno de noche. Tenemos que crear un programa de turnos que esté sujeto a ciertas restricciones.

En este caso, las restricciones añadidas son:

$\bullet$ Tenemos cada monitorista y su disponibilidad semanal (todos están siempre disponibles) en un fichero Excel, junto con su "score de productividad" (de 1 a 100) y su nivel de experiencia (0 = Experiencia baja, 1 = Experiencia media y 2 = Experiencia alta).

$\bullet$ El ciclo semanal constará de 6 días, es decir, se asumirá que una semana consta de 6 días.

$\bullet$ Los días de trabajo están separados en dos turnos de 12 horas (lunes 07:00 - lunes 19:00, lunes 19:00 - martes 07:00, martes 07:00 - martes 19:00, martes 19:00 - miércoles 07:00, miércoles 07:00 - miércoles 19:00, miércoles 19:00 - jueves 07:00, jueves 07:00 - jueves 19:00, jueves 19:00 - viernes 07:00, viernes 07:00 - viernes 19:00, viernes 19:00 - sábado 08:00, sábado 08:00 - sábado 20:00, sábado 20:00 - domingo 08:00, domingo 08:00 - domingo 20:00, domingo 20:00 - lunes 07:00).

$\bullet$ Cada monitorista deberá trabajar como máximo 12 horas por día.

$\bullet$ El horario considerado como de día es el correspondiente a 07:00 - 19:00 ó 08:00 - 20:00.

$\bullet$ El horario considerado como de noche es el correspondiente a 19:00 - 07:00, 19:00 - 08:00,  20:00 - 08:00 ó 20:00 - 07:00.

$\bullet$ La distribución de monitoristas está dada de la siguiente manera: 18 monitoristas y un jefe de turno en el día, y 16 monitoristas y un jefe de turno en la noche.

$\bullet$ En caso de que un jefe de turno llegase a faltar, éste será sustituído por un supervisor.

$\bullet$ A cada monitorista se le asignará de manera aleatoria una operación, dicha operación no deberá ser asignada al mismo monitorista de manera consecutiva.

$\bullet$ A los monitoristas más nuevos se les asignarán operaciones mas pequeñas.

$\bullet$ En caso de existir faltantes en los monitoristas, se construirá una redistribución de las operaciones. Es decir, uno o más monitoristas se les asignará mas operaciones.

$\bullet$ Los monitoristas (y los jefes de turno) tendrán dos turnos en el día, dos turnos en la noche y un descanso de 2 días a la "semana" (ciclo semanal).






