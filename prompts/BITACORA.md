# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.

Herramienta de IA usada: ChatGPT

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|---|---|---|---|
| Zero-shot | 5 | Tabla con clasificacion | Si |
| One-shot | 5 | Texto con flechas | Si |
| Few-shot | 5 | Texto -> etiqueta | Si |

## Ejercicio 3: Chain of Thought

| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|---|---|---|---|
| Directo | 318.60 | No | Si |
| Paso a paso | S/ 318.60 | Si | Si |

Ver el razonamiento me permite comprobar cada calculo y detectar posibles errores.
Aunque la respuesta directa sea correcta, con los pasos puedo entender como se obtuvo el resultado.

## Ejercicio 4: Role prompting

| Version | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo | A quien le sirve mas |
|---|---|---|---|
| A. Sin rol | Sencillo | Si, codigo Python | Publico general |
| B. Rol docente | Sencillo | Si, ejemplo de una caja y codigo Python | Estudiantes principiantes |
| C. Rol senior | Tecnico | Si, codigo Java | Programadores con experiencia |

## Ejercicio 5: Descomposicion

Paso 1: La IA me dio los 5 requisitos principales del sistema de inventario.

Paso 2: La IA diseño las clases necesarias y sus atributos con tipos de datos.

Paso 3: La IA genero el codigo Java de la clase Producto con constructor, getters y setters.

Paso 4: La IA reviso el codigo y propuso 3 mejoras: validar precio, validar stock y agregar toString().

Comparacion: El pedido de una sola vez dio una respuesta general. Al dividirlo en pasos obtuve una solucion mas ordenada, detallada y coherente.


## Ejercicio 6: Prompt estructurado y autocritica

```text
<rol>Actua como analista de pruebas de software.</rol>
<contexto>Login web con correo y contrasena. La cuenta se bloquea despues de 3 intentos fallidos.</contexto>
<tarea>Piensa paso a paso que puede fallar y escribe 6 casos de prueba.</tarea>
<formato>Tabla con las columnas: ID, escenario, datos de entrada, resultado esperado.</formato>

Revisa tu tabla: faltan casos limite como campos vacios, correo sin @ o contrasena con espacios? Agrega los que falten e indica cuales agregaste.
```