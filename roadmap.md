# Roadmap de Aprendizaje

Este documento registra el progreso general del plan de estudio.

Por ahora se desarrolla únicamente el **Bloque 1 — Fundamentos de Programación y Python**.

El objetivo no es completar temas rápidamente, sino comprenderlos, documentarlos y practicarlos correctamente.

---

# Bloque 1 — Fundamentos de Programación y Python

## Objetivo

Reforzar los fundamentos universales de programación e ingeniería necesarios para comprender mejor cómo funcionan las aplicaciones modernas, utilizando Python como lenguaje principal de experimentación.

---

## 1. Pensamiento computacional y resolución de problemas

- [ ] Descomposición de problemas
- [ ] Reconocimiento de patrones
- [ ] Abstracción
- [ ] Diseño de soluciones paso a paso
- [ ] Pseudocódigo
- [ ] Separar problema e implementación

**Objetivo:** diseñar una solución antes de comenzar a escribir código.

Ruta:

```text
blocks/block-01-fundamentals-python/01-computational-thinking/
```

---

## 2. Funcionamiento básico de un programa

- [ ] Código fuente
- [ ] Compilación e interpretación
- [ ] Runtime
- [ ] Procesos
- [ ] Memoria
- [ ] Stack y Heap
- [ ] Variables y referencias
- [ ] Mutabilidad e inmutabilidad

**Objetivo:** comprender qué ocurre cuando se ejecuta un programa.

Ruta:

```text
blocks/block-01-fundamentals-python/02-how-programs-work/
```

---

## 3. Estructuras de datos

- [ ] Arrays / listas
- [ ] Pilas
- [ ] Colas
- [ ] Hash Maps / diccionarios
- [ ] Sets
- [ ] Listas enlazadas
- [ ] Árboles
- [ ] Grafos
- [ ] Elección de estructuras según el problema

**Objetivo:** organizar datos eficientemente y elegir estructuras con criterio.

Ruta:

```text
blocks/block-01-fundamentals-python/03-data-structures/
```

---

## 4. Algoritmos y complejidad

- [ ] Concepto de algoritmo
- [ ] Eficiencia
- [ ] Complejidad temporal
- [ ] Complejidad espacial
- [ ] Big O
- [ ] Búsqueda
- [ ] Ordenamiento
- [ ] Recorridos
- [ ] Trade-offs entre tiempo y memoria

**Objetivo:** razonar sobre el costo de una solución.

Ruta:

```text
blocks/block-01-fundamentals-python/04-algorithms-complexity/
```

---

## 5. Paradigmas de programación

- [ ] Programación imperativa
- [ ] Programación procedural
- [ ] Programación orientada a objetos
- [ ] Programación funcional
- [ ] Programación declarativa
- [ ] Cuándo usar cada paradigma

**Objetivo:** reconocer distintas formas de modelar problemas.

Ruta:

```text
blocks/block-01-fundamentals-python/05-programming-paradigms/
```

---

## 6. Programación Orientada a Objetos

- [ ] Clases y objetos
- [ ] Encapsulación
- [ ] Abstracción
- [ ] Herencia
- [ ] Composición
- [ ] Polimorfismo
- [ ] Interfaces y contratos
- [ ] Composición vs. herencia

**Objetivo:** comprender la POO como herramienta de diseño.

Ruta:

```text
blocks/block-01-fundamentals-python/06-oop/
```

---

## 7. Programación funcional básica

- [ ] Funciones como valores
- [ ] Funciones puras
- [ ] Efectos secundarios
- [ ] Inmutabilidad
- [ ] Funciones de orden superior
- [ ] `map`
- [ ] `filter`
- [ ] `reduce`
- [ ] Lambdas
- [ ] Composición de funciones

**Objetivo:** comprender principios funcionales útiles en distintos paradigmas.

Ruta:

```text
blocks/block-01-fundamentals-python/07-functional-programming/
```

---

## 8. Python — Fundamentos del lenguaje

- [ ] Filosofía general de Python
- [ ] Tipos de datos
- [ ] Colecciones
- [ ] Funciones
- [ ] Scope
- [ ] Módulos y paquetes
- [ ] Excepciones
- [ ] Comprensiones
- [ ] Iterables
- [ ] Iteradores
- [ ] Generadores
- [ ] Decoradores
- [ ] Context managers
- [ ] Dataclasses
- [ ] Type hints

**Objetivo:** comprender Python más allá de su sintaxis básica.

Ruta:

```text
blocks/block-01-fundamentals-python/08-python-fundamentals/
```

---

## 9. Entornos y dependencias en Python

- [ ] Instalación de Python
- [ ] `pip`
- [ ] Entornos virtuales
- [ ] `venv`
- [ ] Gestión de dependencias
- [ ] `pyproject.toml`
- [ ] Poetry
- [ ] Versionado de dependencias
- [ ] Dependencias directas y transitivas

**Objetivo:** crear entornos reproducibles y mantener dependencias correctamente.

Ruta:

```text
blocks/block-01-fundamentals-python/09-python-environments/
```

---

## 10. Modularidad y organización del código

- [ ] Módulos
- [ ] Paquetes
- [ ] Imports
- [ ] Dependencias entre módulos
- [ ] Separación de responsabilidades
- [ ] Organización básica de proyectos
- [ ] Reutilización
- [ ] Acoplamiento
- [ ] Cohesión

**Objetivo:** organizar software para que pueda crecer de manera mantenible.

Ruta:

```text
blocks/block-01-fundamentals-python/10-modularity/
```

---

## 11. Errores, excepciones y debugging

- [ ] Tipos de errores
- [ ] Excepciones
- [ ] `try / except / else / finally`
- [ ] Excepciones personalizadas
- [ ] Stack trace
- [ ] Debugger
- [ ] Logging básico
- [ ] Estrategias de diagnóstico

**Objetivo:** diagnosticar problemas de forma sistemática.

Ruta:

```text
blocks/block-01-fundamentals-python/11-errors-debugging/
```

---

## 12. Concurrencia y paralelismo

- [ ] Procesos
- [ ] Threads
- [ ] Concurrencia
- [ ] Paralelismo
- [ ] I/O Bound
- [ ] CPU Bound
- [ ] Race conditions
- [ ] Locks
- [ ] Sincronización
- [ ] Thread safety
- [ ] Multiprocessing

**Objetivo:** comprender cómo se coordinan múltiples tareas.

Ruta:

```text
blocks/block-01-fundamentals-python/12-concurrency-parallelism/
```

---

## 13. Programación asíncrona

- [ ] Síncrono vs. asíncrono
- [ ] Blocking vs. non-blocking
- [ ] Event Loop
- [ ] Coroutines
- [ ] `async`
- [ ] `await`
- [ ] Tasks
- [ ] `asyncio`
- [ ] `gather`
- [ ] Timeouts
- [ ] Cancelación
- [ ] Semáforos
- [ ] Errores comunes con async

**Objetivo:** comprender las bases que posteriormente aparecen en FastAPI y SQLAlchemy async.

Ruta:

```text
blocks/block-01-fundamentals-python/13-async-programming/
```

---

## 14. Fundamentos de sistemas operativos

- [ ] Procesos y threads
- [ ] Memoria
- [ ] Sistema de archivos
- [ ] Variables de entorno
- [ ] Entrada y salida
- [ ] Señales
- [ ] Puertos
- [ ] Permisos
- [ ] Terminal y shell
- [ ] Fundamentos de Linux

**Objetivo:** comprender el entorno donde realmente se ejecutan las aplicaciones.

Ruta:

```text
blocks/block-01-fundamentals-python/14-operating-systems/
```

---

## 15. Fundamentos de redes

- [ ] Cliente y servidor
- [ ] IP
- [ ] DNS
- [ ] Puertos
- [ ] TCP
- [ ] UDP
- [ ] HTTP
- [ ] HTTPS
- [ ] Request / Response
- [ ] Latencia
- [ ] Sockets
- [ ] Conexiones persistentes
- [ ] Fundamentos de TLS

**Objetivo:** establecer la base para APIs, WebSockets, gRPC y sistemas distribuidos.

Ruta:

```text
blocks/block-01-fundamentals-python/15-networking/
```

---

## 16. Calidad básica en Python

- [ ] PEP 8
- [ ] Ruff
- [ ] Formateo
- [ ] Type checking
- [ ] MyPy
- [ ] Pytest
- [ ] Fixtures
- [ ] Tests parametrizados
- [ ] Organización de tests

**Objetivo:** incorporar herramientas de calidad desde el inicio.

Ruta:

```text
blocks/block-01-fundamentals-python/16-python-quality/
```

---

# Herramientas principales del Bloque 1

- Python
- Git
- GitHub
- Markdown
- `venv`
- Poetry
- Ruff
- MyPy
- Pytest
- IDE con debugger

---

# Estrategia de trabajo

Para cada tema:

```text
feature/<tema>
   ↓
teoría
   ↓
laboratorios
   ↓
revisión
   ↓
merge a develop
```

Cuando el Bloque 1 esté completo y estable:

```text
develop
   ↓
main
```

---

# Criterio para considerar un tema completado

Un tema puede marcarse como terminado cuando:

- [ ] Existe documentación teórica.
- [ ] Las referencias principales están documentadas.
- [ ] Se completaron los ejercicios prácticos seleccionados.
- [ ] Se comprende cuándo utilizar el concepto.
- [ ] Se comprende cuándo no utilizarlo.
- [ ] Se puede explicar con palabras propias.
- [ ] Se puede reconocer su uso o mal uso durante una revisión de código.

---

# Resultado esperado del Bloque 1

Al completar el bloque debería ser posible:

- comprender cómo se ejecuta un programa
- razonar sobre estructuras de datos y complejidad
- distinguir distintos paradigmas
- utilizar Python con mayor profundidad
- comprender procesos, threads y asincronía
- entender fundamentos de sistemas operativos
- entender fundamentos de redes
- escribir código con testing, typing y herramientas básicas de calidad

Una vez completado este bloque se podrá avanzar hacia:

> **Bloque 2 — Ingeniería de Software**
