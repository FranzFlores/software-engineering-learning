# Software Engineering Learning

Repositorio personal de aprendizaje para reforzar fundamentos de ingeniería de software, profundizar en desarrollo backend y arquitectura, y construir una base de conocimiento reutilizable a largo plazo.

La idea principal es separar claramente:

- teoría
- laboratorios y ejercicios pequeños
- particularidades de lenguajes
- frameworks
- patrones de diseño
- aplicación práctica en proyectos reales

El objetivo no es acumular apuntes, sino construir una referencia que permita entender los conceptos, practicarlos y volver a consultarlos en el futuro.

---

## Estructura general

```text
software-engineering-learning/
│
├── README.md
├── roadmap.md
│
├── blocks/
│   └── block-01-fundamentals-python/
│       ├── README.md
│       ├── 01-computational-thinking/
│       ├── 02-how-programs-work/
│       ├── 03-data-structures/
│       ├── 04-algorithms-complexity/
│       ├── 05-programming-paradigms/
│       ├── 06-oop/
│       ├── 07-functional-programming/
│       ├── 08-python-fundamentals/
│       ├── 09-python-environments/
│       ├── 10-modularity/
│       ├── 11-errors-debugging/
│       ├── 12-concurrency-parallelism/
│       ├── 13-async-programming/
│       ├── 14-operating-systems/
│       ├── 15-networking/
│       └── 16-python-quality/
│
├── languages/
│   ├── python/
│   ├── typescript/
│   └── dart/
│
├── frameworks/
│   ├── fastapi/
│   ├── nestjs/
│   ├── angular/
│   └── flutter/
│
├── design-patterns/
│
└── templates/
    ├── topic-template.md
    ├── lab-template.md
    └── study-prompt.md
```

---

## Cómo se organiza el conocimiento

### `blocks/`

Contiene el plan de estudio ordenado por bloques.

Aquí van los conceptos que deben estudiarse en una secuencia concreta.

Regla general:

> Si el concepto es independiente del lenguaje, pertenece al bloque correspondiente.

Ejemplos:

- estructuras de datos
- complejidad algorítmica
- concurrencia
- redes
- arquitectura
- sistemas distribuidos

---

### `languages/`

Contiene características y mecanismos propios de cada lenguaje.

Ejemplos:

```text
languages/python/asyncio/
languages/python/decorators/

languages/typescript/type-system/
languages/typescript/promises/

languages/dart/isolates/
languages/dart/null-safety/
```

Regla general:

> Si el tema explica cómo un lenguaje concreto implementa un concepto, pertenece a `languages/`.

---

### `frameworks/`

Contiene conocimiento específico de frameworks y tecnologías.

Ejemplos:

```text
frameworks/fastapi/
frameworks/nestjs/
frameworks/angular/
frameworks/flutter/
```

---

### `design-patterns/`

Contiene patrones de diseño independientes del lenguaje.

Cada patrón puede incluir:

```text
strategy/
├── theory.md
└── labs/
    ├── python/
    └── typescript/
```

---

### `templates/`

Contiene plantillas reutilizables para mantener consistencia en todo el repositorio.

Ejemplos:

- estructura para documentos teóricos
- estructura para laboratorios
- prompt de estudio reutilizable

---

## Estructura recomendada por tema

Los temas pueden seguir una estructura similar a:

```text
topic/
├── theory.md
├── references.md
└── labs/
    ├── python/
    ├── typescript/
    └── dart/
```

No todos los temas necesitan todos los lenguajes.

La prioridad inicial será Python.

---

## Filosofía de aprendizaje

El proceso recomendado para cada tema es:

```text
Entender
   ↓
Documentar
   ↓
Experimentar
   ↓
Validar
   ↓
Aplicar cuando tenga sentido
```

La teoría debe responder preguntas como:

- ¿Qué es?
- ¿Por qué existe?
- ¿Qué problema resuelve?
- ¿Cómo funciona?
- ¿Cuándo utilizarlo?
- ¿Cuándo no utilizarlo?
- ¿Qué errores son frecuentes?
- ¿Cómo aparece en proyectos reales?

---

## Teoría y práctica

La teoría se documentará principalmente en archivos Markdown.

Los ejercicios deberán ser pequeños y aislados.

Ejemplo:

```text
13-async-programming/
├── theory.md
├── references.md
└── labs/
    └── python/
        ├── 01-blocking-vs-async.py
        ├── 02-coroutines.py
        └── 03-concurrent-tasks.py
```

Los laboratorios no deben convertirse innecesariamente en aplicaciones completas.

Su objetivo es demostrar y entender un concepto concreto.

---

## Proyecto transversal

Además de este repositorio de aprendizaje, se desarrollará un proyecto de gestión de gastos personales dividido en repositorios independientes:

```text
expense-tracker-backend
expense-tracker-web
expense-tracker-mobile
```

Este repositorio sirve para aprender.

El proyecto de gastos sirve para aplicar lo aprendido cuando tenga sentido.

Regla:

> Learning repo = entender y experimentar.  
> Expense Tracker = integrar y tomar decisiones reales.

---

## Estrategia de Git

Durante el Bloque 1 se probará un flujo basado en:

```text
main
└── versión estable

develop
└── integración del bloque

feature/*
└── trabajo de cada tema
```

Ejemplos:

```text
feature/data-structures
feature/python-asyncio
feature/networking-basics
```

Flujo recomendado:

```text
feature/*
   ↓
develop
   ↓
main
```

`main` se actualizará cuando el bloque alcance un estado estable.

---

## Bloque actual

El primer bloque está dedicado a:

> **Fundamentos de Programación y Python**

Consulta el detalle en:

```text
blocks/block-01-fundamentals-python/README.md
```

y el progreso general en:

```text
roadmap.md
```

---

## Objetivo a largo plazo

Construir una base de conocimiento personal que permita:

- reforzar fundamentos
- aprender nuevas tecnologías con mayor facilidad
- comprender mejor sistemas reales
- revisar código con mayor criterio
- trabajar de forma efectiva con herramientas de IA
- reutilizar conceptos entre diferentes lenguajes y frameworks
