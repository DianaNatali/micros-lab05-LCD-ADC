# Lab05 - LCD + ADC

Índice:

1. [Integrantes](#integrantes)
2. [Documentación](#documentación)
3. [Diagramas](#diagramas)
4. [Preguntas](#preguntas)
5. []

## 1. Integrantes

## 2. Documentación

## 3. Diagramas

## 4. Preguntas


### Preguntas sobre inicialización y configuración del ADC

1. Explicar el propósito de una función dedicada a inicializar el módulo ADC en el **PIC**. Describir qué se configura en cada uno de los registros principales utilizados en este proceso.

2. ¿Qué parámetros se deben ajustar para definir el canal analógico, la referencia de voltaje y el reloj de conversión en el ADC del **PIC**?

3. Explicar por qué es importante habilitar el módulo ADC antes de intentar realizar cualquier conversión.

### Preguntas sobre la lectura del ADC

1. Detallar el proceso completo que sigue el microcontrolador desde que se inicia la conversión hasta que se obtiene el valor final, incluyendo qué sucede a nivel de bits y registros.

2. ¿Cuál es la función de la bandera ```GO/DONE``` en el proceso de conversión y qué representa su valor en $1$ o en $0$?

3. Describir cómo se combinan los registros de resultado del ADC para formar un único valor de $1$ bits.

### Preguntas sobre la LCD

1. Explicar detalladamente cómo se divide un byte en dos partes y cómo se envían primero los $4$ bits más significativos y luego los menos significativos.
Incluir en la explicación:

    * El uso de operadores de desplazamiento (```>>```) y enmascaramiento (```&```).

    * El orden en que deben enviarse los datos y por qué este orden es importante.

2. La LCD requiere una secuencia específica de comandos durante su inicialización.
Describir paso a paso la secuencia de inicialización usada en el código para configurar la LCD en modo de $4$ bits, explicando el propósito de cada comando enviado.


### Preguntas de aplicación y resolución de problemas

1. ¿Por qué en la conversión de la lectura del ADC a voltaje, se debe dividir en $1023$?

2. Explicar cómo se utiliza una función para formatear un valor de voltaje y mostrarlo en la LCD con dos cifras decimales. Describir el rol de cada elemento que interviene en el proceso.

3. Explicar la diferencia entre mostrar texto fijo y texto formateado en la LCD, e indicar por qué en el caso del voltaje se requiere formatear el texto antes de enviarlo a la pantalla.

4. Suponer que ahora se necesita implementar una función que permita desplazar el texto hacia la izquierda automáticamente cada $300$ ms, pero sin usar retardos bloqueantes (```__delay_ms```), ¿qué periféricos del **PIC** debe configurar para realizar esto?


## Referencias


