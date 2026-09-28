# Objetivo
Necesidad a resolver: La tarea ayudará al usuario a organizar las tareas pendientes que tenga y darles más prioridad.

Resultado que espera el usuario: 
- Registrar una tarea correctamente.
- Obtener el listado de tareas pendientes que caducan hoy.

# Entradas
## Crear una tarea
Los datos de entradas para esta tareas son:
- Id usuario -> obligatorio
- título -> obligatorio
- descripción -> opcional
- fecha límite -> obligatorio

Supuesto:
Toda tarea nueva inicia con estado "pendiente".

## Consultar tareas que vencen hoy
El dato de entrada para esta tarea es:
- Id usuario -> obligatorio. Para que el sistema pueda identificar el listado de las notas que pertenecen al usuario que consulta
- fecha actual -> opcional. Para que compare con el campo de `fecha límite`. Sin embargo, dentro del proceso es posible obtener la fecha actual para el usuario, es por eso que considero como opcional este campo.

# Salidas 
## Crear una tarea
```text
Efecto:
    - la tarea queda registrada

Salida (3 valores posibles):
    - tarea creada
    - confirmación de creación
    - error
```

## Consultar tareas que vencen hoy
```text
Salida:
- colección de tareas pendientes que vencen hoy.
```

# Descomposición
Los subproblemas que identifico son:

- Crear una nueva tarea
    - Validar información (campos obligatorios u opcionales)
    - Asociar tarea al usuario
    - Persistir información
    - Mostrar confirmación de la acción

- Consultar tareas
    - Identificar usuario
    - Determinar la fecha actual
    - Obtener las tareas asociadas al usuario
    - Obtener las tareas que coincida su fecha límite con la fecha actual
    - Obtener las tareas cuyo estado sea "pendiente"

# Reglas básicas
## Crear una tarea
- Una tarea siempre debe tener título, fecha límite y usuario asociado

## Consultar tareas que vencen hoy
La consulta debe mostrar solamente las tareas:
    - pertenecientes al usuario.
    - con estado pendiente. 
    - cuya fecha límite corresponda a la fecha actual.

## Casos límite
- Al crear una tarea, si no se tiene el identificativo del usuario, no se debe permitir la acción y mostrar un error.
- Al crear una tarea, si el campo `fecha límite` es menor a la fecha actual, no se debe permitir la acción y mostrar un error.
- Al crear una tarea, si no se tiene los campos obligatorios no se debe permitir la acción y mostrar un error.
- Al obtener el listado de tareas se debe tener el identificativo del usuario.
- En caso de que el usuario no tenga tareas que cumplas con las condiciones previstas, se indica al usuario que no cuenta con tareas pendientes.

# Preguntas abiertas
- ¿Toda tarea nueva inicia en estado pendiente?
- ¿En qué zona horaria se trabajará las fechas?
- ¿Las fechas límite contienen fecha y hora?
- ¿Existe alguna manera de obtener el id del usuario para poder realizar las consultas?