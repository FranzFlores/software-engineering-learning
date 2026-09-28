## Feedback — Ejercicio 1: Descomposición

Tu resolución va por buen camino y cumple varias partes importantes del ejercicio: separaste creación y consulta, identificaste entradas y salidas, descompusiste en subproblemas y ya empezaste a pensar en reglas y casos límite.

### 1. Objetivo

La idea general es correcta, pero aquí todavía estás describiendo bastante la funcionalidad y menos la **necesidad**.

Tu frase:

> permitir guardar tareas con una fecha límite y consultar tareas que vencen el día actual

explica bien **qué hace** la funcionalidad, pero podrías subir un nivel y expresar mejor **para qué existe**.

Por ejemplo, conceptualmente la necesidad sería algo como:

```text
Ayudar al usuario a organizar sus pendientes
y detectar qué tareas requieren atención hoy.
```

Luego sí puedes indicar que el resultado esperado es:

```text
- registrar una tarea correctamente;
- consultar las tareas pendientes que vencen hoy.
```

También tendría cuidado con asumir:

> mensaje de confirmación

Puede ser perfectamente razonable, pero no forma parte explícita del requerimiento original. Lo marcaría como una decisión de experiencia de usuario o supuesto, no como necesidad confirmada.

---

### 2. Entradas

La separación que hiciste entre:

```text
Crear tarea
Consultar tareas
```

está muy bien.

#### Crear tarea

Identificaste correctamente:

- usuario;
- título;
- descripción;
- fecha límite.

También es razonable pensar que:

```text
estado = pendiente
```

sea el valor inicial.

Pero hiciste bien en escribirlo como una **nota**, porque el enunciado no confirma explícitamente esa regla.

La convertiría formalmente en:

```text
Supuesto:
Toda tarea nueva inicia con estado "pendiente".
```

#### Consultar tareas que vencen hoy

Aquí aparece un punto muy interesante.

Tu razonamiento sobre no enviar necesariamente la fecha actual es correcto desde implementación, pero para este ejercicio conviene subir un nivel de abstracción.

La entrada conceptual podría ser simplemente:

```text
usuario
```

y el proceso necesita además:

```text
fecha/hora actual según una referencia temporal definida
```

No necesariamente esa fecha tiene que ser enviada por el usuario.

La pregunta realmente importante no es:

> ¿uso una función del lenguaje para obtener la fecha?

sino:

> **¿Quién determina qué significa "hoy"?**

Por ejemplo:

```text
Servidor: 2026-09-28 00:30 UTC
Usuario en Ecuador: 2026-09-27 19:30
```

Para el usuario todavía podría ser 27 de septiembre.

Ese es uno de los casos conceptuales importantes que buscaba el ejercicio.

---

### 3. Salidas

Aquí haría una distinción importante entre:

```text
salida de la operación
```

y:

```text
efecto interno
```

Cuando dices:

> Guardado en el mecanismo para el almacenamiento de datos

eso no es exactamente una salida.

Es un **efecto** del proceso.

Podríamos separarlo así:

```text
Crear tarea

Efecto:
- la tarea queda registrada.

Salida:
- tarea creada;
- o confirmación de creación;
- o error.
```

Y para consultar:

```text
Salida:
- colección de tareas pendientes que vencen hoy.
```

Este detalle será bastante importante más adelante cuando trabajes APIs.

---

### 4. Descomposición

Esta es probablemente la parte más sólida de tu respuesta.

La estructura:

```text
Crear tarea
├── Validar información
├── Definir dueño
├── Persistir
└── Confirmar

Consultar tareas
├── Obtener tareas del usuario
└── Filtrar fecha + estado
```

es comprensible y mantiene responsabilidades claras.

Haría dos ajustes.

#### "Definir dueño"

La idea es correcta, pero lo nombraría algo como:

```text
Asociar tarea al usuario
```

porque "definir dueño" puede sonar a una operación distinta del dominio.

#### Consulta

Podrías descomponer un poco mejor:

```text
Consultar tareas que vencen hoy
├── Identificar usuario
├── Determinar qué fecha corresponde a "hoy"
├── Obtener tareas del usuario
├── Considerar solo pendientes
└── Seleccionar las que vencen hoy
```

Aquí aparece una lección importante:

> La descomposición no solo separa acciones; también ayuda a hacer visibles decisiones que antes estaban implícitas.

---

### 5. Reglas básicas

Aquí encontré un pequeño error de redacción:

```text
Una tarea siempre debe tener un título, título y un usuario asociado
```

probablemente querías escribir:

```text
título, fecha límite y usuario asociado
```

porque esos son los campos que marcaste previamente como obligatorios.

También cambiaría:

> Las consultas deben tener filtros.

Eso describe más una posible forma de implementación.

Una regla de negocio más neutral sería:

```text
Solo deben incluirse tareas:
- pertenecientes al usuario;
- con estado pendiente;
- cuya fecha límite corresponda a hoy.
```

Así expresas el comportamiento sin asumir que internamente existe una operación de "filtro".

---

### 6. Casos límite

Aquí es donde más falta desarrollar la respuesta.

El ejercicio pedía **al menos 5 casos límite o situaciones ambiguas**, y actualmente tienes tres, además bastante relacionados con validación de datos obligatorios.

Los que escribiste son válidos, pero deberías buscar situaciones menos obvias.

Por ejemplo, sin resolverlas todavía, podrías preguntarte:

```text
- ¿Puede crearse una tarea cuya fecha límite ya pasó?
- ¿Qué ocurre con una tarea completada que vence hoy?
- ¿Qué significa "hoy" según la zona horaria del usuario?
- ¿Qué ocurre si el usuario no tiene tareas que vencen hoy?
- ¿Puede existir una tarea con fecha límite exactamente al cambiar de día?
- ¿Qué ocurre si la tarea se completa durante la consulta?
- ¿Puede modificarse la fecha límite después de crearla?
```

No necesitas utilizar exactamente esas preguntas, pero ese es el nivel de análisis que conviene practicar.

---

### 7. Preguntas abiertas

Esta sección faltó explícitamente en tu resolución.

Y en este ejercicio es importante porque existen varias cosas que el enunciado deliberadamente no define.

Por ejemplo:

```text
- ¿Toda tarea nueva inicia en estado pendiente?
- ¿Se permite una fecha límite pasada?
- ¿Qué zona horaria determina "hoy"?
- ¿Las tareas completadas se excluyen siempre?
- ¿Una fecha límite contiene solo fecha o también hora?
```

Esto conecta directamente con lo estudiado antes:

> **No rellenar silenciosamente los requisitos que todavía no están definidos.**

---

## Evaluación según los criterios del ejercicio

```text
[x] Explica la necesidad sin introducir una tecnología concreta.
[x] Diferencia creación y consulta.
[x] Identifica entradas y salidas.
[x] La descomposición tiene responsabilidades comprensibles.
[x] Contempla el estado de la tarea.
[~] La ambigüedad de fecha/hora aparece parcialmente.
[ ] Faltan más casos límite.
[~] Distingue algunos supuestos, pero todavía falta hacerlo sistemáticamente.
```

### Estado general

Yo lo consideraría una **buena primera versión**, pero todavía no la daría por finalizada.

El principal objetivo para una segunda iteración sería mejorar tres cosas:

```text
1. Separar necesidad, salida y efecto interno.

2. Añadir preguntas abiertas en lugar de asumir
   comportamientos no definidos.

3. Profundizar en casos límite, especialmente
   alrededor de fecha, estado y "hoy".
```

### Idea principal a conservar

Lo más valioso de este ejercicio no es descubrir que necesitas:

```text
validar → guardar → consultar
```

sino empezar a detectar que expresiones aparentemente simples como:

> **"tareas que vencen hoy"**

esconden decisiones importantes:

```text
¿Qué es hoy?
¿Para quién?
¿En qué zona horaria?
¿Qué estados cuentan?
¿Qué ocurre en los límites del día?
```

Ese es precisamente el tipo de preguntas que una buena descomposición debería ayudarte a descubrir.