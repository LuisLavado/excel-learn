# Funciones de fecha y tiempo para gestión de proyectos

Trabajar con fechas en hojas de cálculo puede simplificar el control y análisis de proyectos. Dominar funciones que permiten calcular diferencias, identificar días específicos y personalizar periodos es clave para gestionar correctamente las entregas y tiempos.

## ¿Cómo usar funciones de fecha en hojas de cálculo para proyectos?
Utilizar la función HOY te muestra la fecha actual con solo escribir `=HOY()`. Esto facilita comparar plazos, ya que puedes restar la fecha de entrega de un proyecto con la fecha actual para saber cuántos días faltan o han pasado.

La función AHORA (`=AHORA()`) agrega además la hora, útil cuando necesitas precisión temporal y seguimiento detallado de actividades.

## ¿Qué funciones ayudan a extraer información específica de las fechas?
- DÍA: Permite obtener únicamente el día numérico de una fecha usando `=DÍA(fecha)`. Así sabes el día exacto de entrega.
- DÍA SEM: Con =`DIASEM(fecha, tipo)`, identificas qué día de la semana corresponde a una fecha. El "tipo" define si tu semana inicia en lunes, domingo, o cualquier otro día; por ejemplo, usar 2 para que el lunes sea 1 y el domingo 7.
- TEXTO: Utilizando `=TEXTO(valor, formato)`, puedes mostrar la fecha como texto legible. Ejemplo: `=TEXTO(fecha, "dddd")` te regresa "domingo" si corresponde, y con `"mmm"` o `"mmmm"` cambias el formato del mes, obteniendo "jun" o "junio" respectivamente.
- MES: Con `=MES(fecha)` obtienes el número del mes, y con TEXTO ese valor puede ser visualizado como nombre de mes.
- AÑO: `=AÑO(fecha)` te da únicamente el año de una fecha, útil para análisis anuales o filtrado de datos.

## ¿Cómo calcular diferencias y contar sólo días laborables?
- DÍAS: Usa `=DÍAS(fecha_final, fecha_inicial)` para obtener el número de días naturales entre dos fechas. Si inviertes las fechas, el resultado será negativo, así que importa el orden según lo que desees analizar.
- DIAS.LAB.INT: Esta fórmula `=DIAS.LAB.INT(fecha_inicial, fecha_final, [fin_de_semana], [días_no_laborables])` calcula la diferencia entre dos fechas considerando solo días laborables. Puedes personalizar qué días son fin de semana y añadir un rango de días festivos o de descanso, que deben fijarse para que no se desplacen al copiar la fórmula.
- El parámetro de fin de semana es flexible: 1 es sábado y domingo, 2 es domingo y lunes, y hay más opciones según tus necesidades.
- Los días no laborables pueden colocarse como un rango fijo; usa F4 para fijarlos cuando los selecciones.
- Los corchetes en los argumentos indican opciones opcionales. Si no necesitas estas opciones, puedes omitirlas y la fórmula igual funcionará.

## ¿Qué recomendaciones permiten optimizar el análisis de fechas?
- Fija las celdas que representan la fecha de hoy o los días de descanso para mantener cálculos correctos al copiar la fórmula.
- Usa formatos de texto para mostrar resultados más claros y personalizados al usuario final.
- Calcula la diferencia entre la fecha actual y la entrega para saber rápido el avance de tus proyectos.