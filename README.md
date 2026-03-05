# Tarea-grupal-Juan-Manuel-y-Denis
 Los tres patrones de refactorizacion que puedo identificar en ese codigo son:

1. En el metodo generarReporte esta haciendo demasiadas cosas a la vez: imprime en consola, calcula el total, verifica tipos de datos y decide el formato de exportacion. Esto hace que el metodo sea largo. La solucion que veo que se debe implementar es dividir la logica en metodos pequeños y con nombres claros. Usando la herramienta de IDE Extract Method.
2. Hay una parte del codigo con un if y un else if que puede simplificarse utilizando el patron Strategy mediante polimorfismo.
El uso de List y la comprobación if (dato instanceof Integer) indican una debilidad en el sistema de tipos.

3.El código depende de verificaciones en tiempo de ejecución (instanceof) y casting (Integer) dato, lo cual es propenso a errores en tiempo de ejecución (ClassCastException). Una solucion seria utilizar Genericos de Java para asegurar la seguridad de tipos en tiempo de compilación.



