# Feedback — Attempt 2: Descomposición de problemas

## Evaluación general

La segunda versión mejora claramente respecto al primer intento.

Los cambios más importantes fueron:

- separaste mejor **efecto** y **salida**;
- incorporaste preguntas abiertas;
- hiciste más explícita la descomposición;
- mejoraste la formulación de las reglas de consulta;
- agregaste más casos límite.

Aun así, quedan algunos puntos que conviene ajustar antes de dar el ejercicio por cerrado.

---

## 1. Objetivo

La frase:

> "La tarea ayudará al usuario a organizar las tareas pendientes que tenga y darles más prioridad."

va en la dirección correcta, pero "darles más prioridad" introduce una idea que no está realmente definida en el enunciado.

La funcionalidad no establece mecanismos de priorización. Solo permite:

- registrar tareas con fecha límite;
- consultar cuáles vencen hoy.

Una formulación más precisa sería:

> Ayudar al usuario a organizar sus tareas pendientes y detectar cuáles requieren atención durante el día actual.

---

## 2. Entradas

### Crear tarea

Está bien identificar:

- usuario;
- título;
- descripción;
- fecha límite.

También está bien mantener:

> Toda tarea nueva inicia con estado `pendiente`.

como **supuesto**, porque el enunciado no lo confirma explícitamente.

### Consultar tareas que vencen hoy

Aquí todavía haría un ajuste.

Actualmente incluyes:

> fecha actual -> opcional

Pero conceptualmente, la fecha actual no tiene por qué ser una entrada proporcionada a la operación.

Conviene diferenciar:

```text
Entrada:
- usuario

Contexto necesario:
- fecha/hora actual
- zona horaria aplicable
```

La operación necesita conocer "hoy", pero eso no significa que deba recibirlo como parámetro.

---

## 3. Salidas

La separación entre efecto y salida mejoró bastante.

Sin embargo, en creación:

```text
Salida:
- tarea creada
- confirmación de creación
- error
```

mezcla dos niveles distintos.

Una forma más clara sería:

```text
Resultado exitoso:
- tarea creada

Resultado fallido:
- error
```

La confirmación visual pertenece más a presentación/UX que al resultado conceptual de la operación.

---

## 4. Descomposición

La descomposición está bien encaminada.

### Crear tarea

Podría quedar:

```text
Crear tarea
├── Validar información
├── Asociar tarea al usuario
├── Definir estado inicial
└── Registrar tarea
```

"Mostrar confirmación" podría quedar fuera si el ejercicio se concentra en dominio/aplicación, porque pertenece más a presentación.

### Consultar tareas

Aquí mejoraste bastante al hacer explícitos usuario, fecha y estado.

Lo reformularía como:

```text
Consultar tareas que vencen hoy
├── Identificar usuario
├── Determinar qué significa "hoy"
├── Obtener tareas del usuario
└── Seleccionar las que:
    ├── estén pendientes
    └── venzan hoy
```

Esto evita pensar demasiado pronto en filtros técnicos separados.

---

## 5. Reglas básicas

Las reglas están bien formuladas.

Solo distinguiría mejor entre reglas confirmadas y supuestos:

```text
Reglas:
- título obligatorio;
- fecha límite obligatoria;
- usuario asociado.

Supuesto:
- toda tarea nueva inicia en estado pendiente.
```

---

## 6. Casos límite

La sección mejoró, pero algunos elementos son más bien errores de validación normales que verdaderos casos límite.

Por ejemplo:

```text
- falta usuario;
- falta campo obligatorio.
```

son importantes, pero son casos básicos de validación.

Para profundizar más, conviene incluir situaciones como:

```text
- una tarea vence hoy pero ya fue completada;
- el usuario cambia de zona horaria;
- la fecha límite coincide con el cambio de día;
- la consulta devuelve cero tareas;
- una tarea fue creada para hoy justo después de haber consultado;
- la fecha límite contiene hora y no solo fecha.
```

No necesitas resolver todas esas situaciones ahora; lo importante es hacerlas visibles.

---

## 7. Preguntas abiertas

Esta sección es una mejora importante respecto al primer intento.

Tus preguntas son pertinentes, especialmente:

- estado inicial;
- zona horaria;
- fecha vs. fecha y hora.

La última:

> "¿Existe alguna manera de obtener el id del usuario para poder realizar las consultas?"

la reformularía como:

> ¿Cómo se identifica al usuario que realiza la operación?

Así mantiene el análisis en un nivel más conceptual.

También añadiría:

```text
- ¿Se permite crear una tarea con fecha límite pasada?
- ¿Las tareas completadas que vencen hoy deben aparecer?
- ¿Puede modificarse posteriormente la fecha límite?
```

---

## Evaluación final

### Criterios cumplidos

- [x] Explica la necesidad sin depender de tecnología.
- [x] Distingue creación y consulta.
- [x] Identifica entradas y salidas.
- [x] Descompone en responsabilidades comprensibles.
- [x] Considera el estado de la tarea.
- [x] Identifica la zona horaria como ambigüedad.
- [x] Incluye varios casos límite.
- [x] Diferencia mejor supuestos de reglas confirmadas.

### Aspectos a afinar

- [ ] Evitar introducir "prioridad" si no forma parte del requisito.
- [ ] Distinguir entrada de contexto del sistema.
- [ ] No tratar la confirmación visual como una salida conceptual distinta.
- [ ] Diferenciar validaciones normales de casos límite.
- [ ] Mantener las preguntas abiertas en un nivel conceptual antes de pensar en implementación.

---

## Conclusión

Daría este **Attempt 2 como suficientemente bueno para cerrar el ejercicio**, teniendo presentes los ajustes anteriores.

La mejora más importante respecto al primer intento es que ahora ya no estás pensando solamente en:

```text
crear
guardar
consultar
```

sino también en:

```text
qué significa "hoy"
qué información es entrada
qué información es contexto
qué es regla
qué es supuesto
qué casos no están definidos
```

Ese cambio de nivel de razonamiento es precisamente el objetivo del ejercicio.
