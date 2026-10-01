# Tarea: Mi prompt avanzado

## Tarea elegida

Encontrar y corregir errores de sintaxis en codigo Java.

## Version 1: prompt basico

```text
Revisa un codigo Java, encuentra sus errores y corrigelos.
```

La IA no pudo realizar la revision porque no le proporcione el codigo.

## Version 2

```text
<rol>Actua como desarrollador Java senior.</rol>

<contexto>Estoy aprendiendo programacion orientada a objetos en Java y necesito encontrar errores en un codigo.</contexto>

Revisa el siguiente codigo Java, identifica los errores y explica como corregirlos:

public class Producto {
    private String nombre;
    private double precio

    public Producto(String nombre, double precio) {
        this.nombre = nombre;
        this.precio = precio;
    }

    public void mostrarDatos() {
        System.out.println("Producto: " + nombre)
        System.out.println("Precio: " + precio);
    }
}
```

Tecnica agregada: Role prompting y contexto.

Por que: Para indicar a la IA desde que rol debe responder y explicar que estoy aprendiendo Java.

Mejora: La IA encontro los 2 errores, explico como corregirlos y mostro el codigo corregido.

## Version 3: prompt final

```text
<rol>Actua como desarrollador Java senior que ayuda a un estudiante que esta aprendiendo programacion orientada a objetos.</rol>

<contexto>El siguiente codigo Java de la clase Producto tiene errores de sintaxis y necesito corregirlo para que pueda compilar correctamente.</contexto>

<tarea>
Revisa el codigo siguiendo estos pasos:
1. Identifica todos los errores.
2. Explica de forma breve por que cada uno es un error.
3. Corrige cada error.
4. Muestra el codigo completo corregido.
5. Revisa nuevamente tu solucion y confirma si queda algun error de sintaxis.
</tarea>

<formato>
Primero muestra una tabla con las columnas: Error, Explicacion y Correccion.
Despues muestra el codigo Java completo corregido.
Finalmente escribe una conclusion corta sobre la revision final.
</formato>

<codigo>
public class Producto {
    private String nombre;
    private double precio

    public Producto(String nombre, double precio) {
        this.nombre = nombre;
        this.precio = precio;
    }

    public void mostrarDatos() {
        System.out.println("Producto: " + nombre)
        System.out.println("Precio: " + precio);
    }
}
</codigo>
```

Tecnicas agregadas: Role prompting, descomposicion, prompt estructurado y autocritica.

Por que: Para obtener una respuesta ordenada, facil de revisar y comprobar que la solucion final sea correcta.

Mejora: La IA identifico los errores, explico cada uno en una tabla, mostro el codigo completo corregido y reviso nuevamente la solucion.

## Tecnicas usadas en el prompt final

| Parte del prompt | Tecnica |
|---|---|
| Actua como desarrollador Java senior... | Role prompting |
| Etiquetas rol, contexto, tarea, formato y codigo | Prompt estructurado |
| Pasos del 1 al 5 | Descomposicion |
| Revisar nuevamente la solucion | Autocritica |

## Evaluacion del resultado

| Criterio | Cumple |
|---|---|
| Identifica todos los errores | Si |
| Explica los errores | Si |
| Muestra el codigo corregido | Si |
| Respeta el formato solicitado | Si |
| Realiza una revision final | Si |

## Por que elegi estas tecnicas

Elegi estas tecnicas porque necesitaba una respuesta clara y ordenada. El role prompting ayuda a definir como debe responder la IA, la descomposicion divide la tarea en pasos, el prompt estructurado organiza las instrucciones y la autocritica permite revisar la solucion final.