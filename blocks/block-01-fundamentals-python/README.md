# Bloque 1 — Fundamentos de Programación y Python

## Objetivo del bloque

Reforzar los fundamentos que permiten comprender cómo funciona el software más allá de un framework o lenguaje concreto, utilizando **Python** como lenguaje principal para experimentar y practicar.

La meta no es volver a aprender programación desde cero, sino conectar conceptos fundamentales con situaciones reales de desarrollo.

---

## 1. Pensamiento computacional y resolución de problemas

- Descomposición de problemas.
- Reconocimiento de patrones.
- Abstracción.
- Diseño de soluciones paso a paso.
- Pseudocódigo y diagramas simples.
- Separar el problema de su implementación.

**Objetivo:** aprender a diseñar una solución antes de comenzar a escribir código.

---

## 2. Funcionamiento básico de un programa

- Código fuente.
- Compilación e interpretación.
- Runtime.
- Procesos.
- Memoria.
- Stack y Heap.
- Variables, referencias y objetos.
- Mutabilidad e inmutabilidad.

**Objetivo:** entender qué ocurre cuando un programa se ejecuta y cómo utiliza la memoria.

---

## 3. Estructuras de datos

- Arrays / listas.
- Pilas.
- Colas.
- Hash Maps / diccionarios.
- Sets.
- Listas enlazadas.
- Árboles.
- Grafos.
- Elección de estructuras según el problema.

**Objetivo:** comprender cómo organizar datos eficientemente y por qué una estructura puede ser mejor que otra.

---

## 4. Algoritmos y complejidad

- Concepto de algoritmo.
- Eficiencia.
- Complejidad temporal.
- Complejidad espacial.
- Big O.
- Búsqueda.
- Ordenamiento.
- Recorridos básicos.
- Trade-offs entre tiempo y memoria.

**Objetivo:** poder razonar sobre el costo de una solución sin necesidad de optimizar prematuramente.

---

## 5. Paradigmas de programación

- Programación imperativa.
- Programación procedural.
- Programación orientada a objetos.
- Programación funcional.
- Programación declarativa.
- Cuándo resulta útil cada enfoque.

**Objetivo:** reconocer diferentes formas de modelar y resolver problemas.

---

## 6. Programación Orientada a Objetos

- Clases y objetos.
- Encapsulación.
- Abstracción.
- Herencia.
- Composición.
- Polimorfismo.
- Interfaces y contratos.
- Composición vs. herencia.

**Objetivo:** comprender la POO como herramienta de diseño y no únicamente como sintaxis.

---

## 7. Programación funcional básica

- Funciones como valores.
- Funciones puras.
- Efectos secundarios.
- Inmutabilidad.
- Funciones de orden superior.
- `map`, `filter` y `reduce`.
- Lambdas.
- Composición de funciones.

**Objetivo:** conocer principios funcionales útiles incluso dentro de aplicaciones orientadas a objetos.

---

## 8. Python — Fundamentos del lenguaje

- Sintaxis y filosofía general de Python.
- Tipos de datos.
- Colecciones.
- Funciones.
- Scope.
- Módulos y paquetes.
- Excepciones.
- Comprensiones.
- Iteradores e iterables.
- Generadores.
- Decoradores.
- Context managers.
- `dataclasses`.
- Type hints.

**Objetivo:** pasar de “saber usar Python” a comprender sus principales mecanismos.

---

## 9. Entornos y dependencias en Python

- Instalación de Python.
- `pip`.
- Entornos virtuales.
- `venv`.
- Gestión de dependencias.
- `pyproject.toml`.
- Poetry.
- Versionado de dependencias.
- Dependencias directas y transitivas.

**Objetivo:** entender cómo aislar, reproducir y mantener correctamente un proyecto Python.

---

## 10. Modularidad y organización del código

- Módulos.
- Paquetes.
- Imports.
- Dependencias entre módulos.
- Separación de responsabilidades.
- Organización básica de proyectos.
- Código reutilizable.
- Acoplamiento y cohesión.

**Objetivo:** aprender a estructurar software que pueda crecer sin convertirse rápidamente en código difícil de mantener.

---

## 11. Errores, excepciones y debugging

- Tipos de errores.
- Excepciones.
- `try / except / else / finally`.
- Excepciones propias.
- Stack trace.
- Debugger.
- Logging básico.
- Estrategias de diagnóstico.

**Objetivo:** aprender a investigar problemas en lugar de depender únicamente de prueba y error.

---

## 12. Concurrencia y paralelismo

- Procesos.
- Threads.
- Concurrencia.
- Paralelismo.
- I/O Bound.
- CPU Bound.
- Race conditions.
- Locks y sincronización.
- Thread safety.
- Multiprocessing.

**Objetivo:** entender cómo un programa puede ejecutar o coordinar múltiples tareas.

---

## 13. Programación asíncrona

- Síncrono vs. asíncrono.
- Blocking vs. non-blocking.
- Event Loop.
- Coroutines.
- `async`.
- `await`.
- Tasks.
- `asyncio`.
- `gather`.
- Timeouts.
- Cancelación.
- Semáforos.
- Errores comunes con código async.

**Objetivo:** comprender la base de la programación asíncrona utilizada posteriormente por FastAPI, SQLAlchemy async y otros componentes del backend.

---

## 14. Fundamentos de sistemas operativos para desarrolladores

- Procesos y threads.
- Memoria.
- Sistema de archivos.
- Variables de entorno.
- Entrada y salida.
- Señales.
- Puertos.
- Permisos.
- Terminal y shell.
- Conceptos básicos de Linux.

**Objetivo:** entender mejor el entorno donde realmente se ejecutan las aplicaciones.

---

## 15. Fundamentos de redes

- Cliente y servidor.
- IP.
- DNS.
- Puertos.
- TCP y UDP.
- HTTP y HTTPS.
- Request / Response.
- Latencia.
- Sockets.
- Conexiones persistentes.
- Conceptos básicos de TLS.

**Objetivo:** construir la base necesaria para estudiar posteriormente APIs, HTTP, WebSockets, gRPC y sistemas distribuidos.

---

## 16. Calidad básica en Python

- PEP 8.
- Ruff.
- Formateo.
- Type checking.
- MyPy.
- Tests con Pytest.
- Fixtures.
- Tests parametrizados.
- Organización de tests.

**Objetivo:** incorporar calidad automática desde los primeros ejercicios.

---

# Herramientas principales del bloque

| Herramienta | Uso |
|---|---|
| Python | Lenguaje principal de práctica |
| Git | Control de versiones |
| GitHub | Repositorio y seguimiento |
| VS Code / IDE | Desarrollo y debugging |
| `venv` / Poetry | Entornos y dependencias |
| Ruff | Linting y calidad |
| MyPy | Comprobación de tipos |
| Pytest | Testing |
| Markdown | Documentación teórica |

---

# Forma de trabajo

Cada tema podrá tener dos componentes:

```text
tema/
├── theory.md
└── labs/
```

- **`theory.md`** → conceptos, explicación, ejemplos y referencias.
- **`labs/`** → ejercicios pequeños diseñados para comprobar el concepto de forma aislada.

Cuando un tema tenga sentido dentro del proyecto principal de gastos, se aplicará posteriormente allí.

---

# Resultado esperado

Al finalizar este bloque deberías poder:

- Explicar cómo se ejecuta un programa y cómo utiliza memoria.
- Elegir estructuras de datos con criterio.
- Razonar sobre complejidad básica.
- Comprender varios paradigmas de programación.
- Utilizar Python con mayor profundidad.
- Diferenciar procesos, threads, concurrencia y paralelismo.
- Comprender cómo funciona `asyncio`.
- Entender los fundamentos de sistemas operativos y redes.
- Escribir pequeños programas con testing, typing y herramientas de calidad.
- Tener la base necesaria para pasar al bloque de **Ingeniería de Software**.
