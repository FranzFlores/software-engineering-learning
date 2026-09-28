# Objetivo
Necesidad a resolver: La tarea consisten en permitir guardar tareas con una fecha límite y consultar tareas que vencen el día actual.

Resultado que espera el usuario: 
- Mensaje de confirmación indicando que su tarea se guardo correctmante.
- Listado de tareas donde el campo `fecha límite` coincide con la fecha actual. 

# Entradas
## Crear una tarea
Los datos de entradas para esta tareas son:
- Id usuario -> obligatorio
- título -> obligatorio
- descripción -> opcional
- fecha límite -> obligatorio

Nota: Considero que al crearse una nueva tarea, por defecto, el campo `estado` toma el valor de `pendiente`.

## Consultar tareas que vencen hoy
El dato de entrada que considero que se debe enviar es:
- Id usuario -> obligatorio. Para que el sistema pueda identificar el listado de las notas que pertenecen al usuario que consulta
- fecha actual -> opcional. Para que compare con el campo de `fecha límite`. Sin embargo, dentro del proceso es posible obtener la fecha actual, es por eso que considero como opcional este campo. En la práctica no lo pediría ya que usaría las funciones de los diferentes lenguajes para saber la fecha actual.

# Salidas 
## Crear una tarea
Guardado en el mecanismo para el almacenamiento de datos (puede ser una BD, archivo, etc) y mostrar un mensaje de confirmación de la acción al usuario

## Consultar tareas que vencen hoy
Listado de tareas que pertenecen al usuario y que su campo `fecha límite` coincida con la fecha actual.

# Descomposición
Los subproblemas que identifico son:

- Crear una nueva tarea
    - Validar información (campos obligatorios u opcionales)
    - Definir el "dueño" de la tarea
    - Persistir información
    - Mostrar confirmación de la acción
- Consultar tareas 
    - Obtener las tareas asociadas al usuario
    - Obtener las tareas que coincida su fecha límite con la fecha actual y su estado sea "pendiente"

# Reglas básicas
## Crear una tarea
- Una tarea siempre debe tener un título, título y un usuario asociado

## Consultar tareas que vencen hoy
- La consulta debe contar con el identificativo del usuario para poder obtener los datos 
- Las consultas deben tener filtros
    - estado: Solo con estado `pendiente`
    - fecha: Solo aquellas que su `fecha límite` sea igual a la fecha actual

## Casos límite
- Al crear una tarea, si no se tiene el identificativo del usuario, no se debe permitir la acción y mostrar un error.
- Al crear una tarea, si no se tiene los campos obligatorios no se debe permitir la acción y mostrar un error.
- Al obtener el listado de tareas se debe tener el identificativo del usuario.
