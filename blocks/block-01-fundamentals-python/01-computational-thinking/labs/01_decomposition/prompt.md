# Ejercicio básico — Descomposición

## Escenario

Estás desarrollando una aplicación personal para organizar tareas.

La nueva funcionalidad solicitada es:

> **Permitir que un usuario cree una tarea con fecha límite y pueda consultar cuáles tareas vencen hoy.**

Una tarea contiene inicialmente:

- título;
- descripción opcional;
- fecha límite;
- estado.

Los estados posibles son:

- pendiente;
- completada.

No se ha definido todavía cómo se almacenarán las tareas ni qué tecnología se utilizará.

---

## Tu trabajo

Analiza el problema y entrega una propuesta con las siguientes secciones.

### 1. Objetivo

Explica en una o dos frases:

- qué necesidad intenta resolver la funcionalidad;
- qué resultado espera obtener el usuario.

### 2. Entradas

Identifica la información necesaria para:

- crear una tarea;
- consultar las tareas que vencen hoy.

### 3. Salidas

Indica qué debería producir cada operación.

### 4. Descomposición

Divide la funcionalidad en subproblemas razonables.

Por ejemplo, piensa en aspectos como:

```text
crear tarea
consultar tareas
determinar si una tarea vence hoy
...
```

No copies necesariamente esta estructura si encuentras una mejor.

### 5. Reglas básicas

Identifica reglas que deberían cumplirse.

Algunas preguntas para ayudarte:

- ¿puede una tarea no tener título?
- ¿puede tener una fecha anterior al día actual?
- ¿una tarea completada debería aparecer como "vence hoy"?
- ¿qué significa exactamente "hoy"?

### 6. Casos límite

Identifica al menos **5 casos límite o situaciones ambiguas**.

---

## Entregable sugerido

```text
Objetivo

Entradas

Salidas

Subproblemas

Reglas

Casos límite

Preguntas abiertas
```

---

## Criterios de evaluación

Tu respuesta es sólida si:

- [ ] explica la necesidad sin introducir tecnologías;
- [ ] diferencia claramente creación y consulta;
- [ ] identifica entradas y salidas;
- [ ] la descomposición tiene partes con responsabilidades comprensibles;
- [ ] contempla el estado de la tarea;
- [ ] identifica al menos una ambigüedad relacionada con fecha/hora;
- [ ] incluye casos límite reales;
- [ ] distingue reglas confirmadas de supuestos.