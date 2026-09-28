# Attempt final — Ejercicio básico de descomposición

## Objetivo

### Necesidad a resolver

Ayudar al usuario a organizar sus tareas pendientes y detectar cuáles requieren atención durante el día actual.

### Resultado esperado

El usuario debe poder:

- registrar una nueva tarea con fecha límite;
- consultar las tareas pendientes que vencen hoy.

---

## Entradas

### Crear una tarea

Información necesaria:

- usuario;
- título;
- descripción opcional;
- fecha límite.

### Supuesto

Toda tarea nueva inicia con estado:

```text
pendiente
```

Este comportamiento debe confirmarse como regla del dominio.

### Consultar tareas que vencen hoy

Entrada principal:

- usuario que realiza la consulta.

Contexto necesario:

- fecha/hora actual;
- zona horaria utilizada para determinar qué significa "hoy".

La fecha actual no necesariamente debe recibirse como parámetro de entrada.

---

## Salidas

### Crear una tarea

#### Resultado exitoso

```text
Tarea creada.
```

La tarea queda registrada y asociada al usuario.

#### Resultado fallido

```text
Error indicando por qué la tarea no pudo crearse.
```

Por ejemplo:

- datos obligatorios faltantes;
- usuario no válido;
- fecha no permitida.

### Consultar tareas que vencen hoy

#### Resultado exitoso

```text
Colección de tareas pertenecientes al usuario
que están pendientes y vencen hoy.
```

La colección puede estar vacía si ninguna tarea cumple las condiciones.

#### Resultado fallido

```text
Error si no es posible identificar o validar
al usuario que realiza la consulta.
```

---

## Descomposición

### Crear una tarea

```text
Crear tarea
├── Validar información obligatoria
├── Validar reglas relacionadas con la fecha límite
├── Asociar la tarea al usuario
├── Definir estado inicial
└── Registrar la tarea
```

### Consultar tareas que vencen hoy

```text
Consultar tareas que vencen hoy
├── Identificar al usuario
├── Determinar qué fecha corresponde a "hoy"
├── Obtener las tareas pertenecientes al usuario
└── Seleccionar aquellas que:
    ├── estén pendientes
    └── venzan hoy
```

---

## Reglas básicas

### Crear una tarea

Una tarea debe:

- tener título;
- tener fecha límite;
- estar asociada a un usuario.

### Supuesto pendiente de confirmación

```text
Toda tarea nueva inicia en estado "pendiente".
```

### Consultar tareas que vencen hoy

Solo deben incluirse tareas que:

- pertenezcan al usuario que realiza la consulta;
- tengan estado `pendiente`;
- tengan una fecha límite correspondiente al día actual según la zona horaria definida.

---

## Casos límite y situaciones ambiguas

### 1. Usuario no identificado

Si no es posible determinar qué usuario realiza la operación, no debe permitirse crear ni consultar tareas asociadas a él.

### 2. Datos obligatorios faltantes

Si falta título, fecha límite o usuario, la tarea no debe crearse.

### 3. Fecha límite pasada

Debe definirse si el sistema:

- impide crear una tarea con fecha pasada;
- permite crearla;
- o solicita confirmación.

Actualmente es una regla pendiente.

### 4. Tarea completada que vence hoy

Debe confirmarse si una tarea completada debe excluirse del listado.

Según el comportamiento esperado del ejercicio, se asume que solo se muestran tareas pendientes.

### 5. Usuario sin tareas que vencen hoy

La consulta debe poder devolver correctamente una colección vacía.

Esto no debería considerarse un error.

### 6. Diferencias de zona horaria

Debe existir una regla para determinar qué zona horaria define el día actual.

### 7. Fecha límite con hora

Debe definirse si `fecha límite` representa:

```text
2026-09-28
```

o:

```text
2026-09-28 18:00
```

Esto puede modificar cómo se determina cuándo una tarea vence.

---

## Preguntas abiertas

1. ¿Toda tarea nueva inicia obligatoriamente con estado `pendiente`?
2. ¿Se permite crear una tarea cuya fecha límite ya pasó?
3. ¿Qué zona horaria se utiliza para determinar el día actual?
4. ¿La fecha límite contiene únicamente fecha o también hora?
5. ¿Las tareas completadas deben excluirse siempre de la consulta "vence hoy"?
6. ¿Puede modificarse posteriormente la fecha límite?
7. ¿Cómo se identifica conceptualmente al usuario que realiza la operación?

---

## Modelo mental final del ejercicio

La funcionalidad inicialmente parece sencilla:

```text
Crear tarea
Consultar tareas que vencen hoy
```

Pero al descomponerla aparecen decisiones importantes:

```text
Usuario
   ↓
Crear tarea
   ├── validar datos
   ├── validar fecha
   ├── asociar usuario
   ├── establecer estado
   └── registrar

Usuario
   ↓
Consultar tareas de hoy
   ├── determinar "hoy"
   ├── identificar tareas propias
   ├── considerar estado
   └── considerar fecha límite
```

La principal conclusión del ejercicio es que una buena descomposición no consiste únicamente en dividir una funcionalidad en pasos.

También debe ayudar a descubrir:

- responsabilidades;
- dependencias;
- reglas;
- supuestos;
- ambigüedades;
- casos límite.

En este punto todavía no es necesario decidir:

- lenguaje;
- framework;
- base de datos;
- estructura de tablas;
- endpoints;
- clases.

Primero se busca comprender correctamente el problema.
