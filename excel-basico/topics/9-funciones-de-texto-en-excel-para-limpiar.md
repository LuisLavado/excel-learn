# Funciones de texto en Excel para limpiar y organizar datos

Dominar las funciones de texto en Excel es esencial para quienes trabajan con grandes volúmenes de datos. Estas herramientas ayudan a organizar la información cuando no llega en el formato necesario, facilitando tareas que de otra forma serían complicadas. Aprender a usar funciones como _**CONCAT, EXTRAER, ESPACIOS y LIMPIAR**_ puede transformar cómo gestionas tus bases y reportes.

## ¿Cómo unir textos y agregar información personalizada en Excel?
Las funciones para unir textos ahorran tiempo y simplifican el manejo de datos dispersos.

- **CONCAT** sirve para combinar diferentes celdas, incluso permitiéndote agregar espacios o palabras adicionales entre los datos.
- Al escribir **CONCAT**, Excel recomienda esta función sobre concatenar, ya que la segunda está en desuso.
- Para añadir un espacio, se escribe entre comillas: `", "`.
- Puedes agregar cualquier texto fijo, como códigos o etiquetas, usando comillas para que se reconozca como texto.
- El símbolo ampersand (`&`) es otro método ágil para unir datos, actuando como un "pegamento" flexible entre celdas o palabras.
Ambas opciones entregan el mismo resultado; la elección depende de cuál te resulte más clara o rápida según el contexto.

## ¿Cómo extraer segmentos específicos usando izquierda, extraer y derecha?
A veces necesitas solamente una parte del dato, como códigos, fechas o tipos de movimiento.

- La función IZQUIERDA toma un número específico de caracteres desde el extremo izquierdo del texto.
    - Por ejemplo, puedes traer los primeros tres caracteres para identificar la clase de operación: gasto o ingreso.
- EXTRAER permite seleccionar una parte ubicada en medio del texto.
    - Necesitas indicar la posición de inicio y la cantidad de caracteres a extraer.
    - Ejemplo: desde el quinto carácter, toma los siguientes tres.
- DERECHA obtiene un bloque de caracteres desde el final de la celda.
    - Útil para sacar fechas o códigos que siempre están al final.
Estas funciones agilizan el filtrado y análisis de información sin tener que modificar el archivo original.

## ¿Cómo limpiar espacios o caracteres invisibles para tener datos limpios?
Una base de datos limpia es clave para evitar errores y facilitar el análisis.

- ESPACIOS elimina los espacios extras al inicio, en medio (más de uno) y al final del texto, dejando solo un espacio entre palabras.
- LIMPIAR borra caracteres no imprimibles, como saltos de línea ocultos o símbolos extraños.
- Puedes anidar ambas funciones para limpiar al máximo: primero aplicas ESPACIOS, luego envuelves dentro de LIMPIAR.
    - Presta atención a los paréntesis de colores en Excel; debes cerrarlos todos, terminando con el color negro para asegurar el cierre correcto de la fórmula.
Estos pasos convierten cualquier columna en una fuente lista para copiar y usar en otros documentos.

## ¿Cómo convertir fórmulas a valores planos para usarlos en cualquier hoja?
Al finalizar, es probable que quieras convertir el resultado de tus fórmulas en valores estáticos.

- Simplemente copias la columna con Control C.
- Luego, eliges "Pegar como valores" desde el menú, asegurando que la información quede fija al moverla entre hojas.

Así, tendrás la flexibilidad de trabajar con los datos ya limpios y listos para agregar a informes o dashboards.