# Notas — Tema 1: Pensamiento computacional y resolución de problemas

## Índice

- [1. Introducción](#1-introducción)

## 1. Introducción

### Mi comprensión

El pensamiento computacional básicamente es poder aplicar conceptos que se usan dentro de la informática como el descomponer problemas grandes en pequeños o sintizar lo relevante para poder resolver un problema mediante un sistema informático. 

Por ejemplo, si un amigo se dedica a vender productos por internet y desea tener un mejor control de su mercadería, le podría sugerir que use hojas de Excel. Sin embargo, si desea algo más preciso como obtener gráficas de lo que ha vendido, información de sus clientes, declaraciones de impuestos, etc si podría proponerle hacer un sistema informático acoplado a cada una de sus necesidades.

Además, algo que me llamó la atención de esta primera sección es que este "pensamiento computacional" NO debe resumirse en simplemente programar SINO resolver el problema.

Luego de ello, se da una serie de pasos que consisten en desglosar el problema en relación a datos, restricciones, casos de uso, etc. En esta sección además se da como mensaje el riesgo que existe si no se analiza correctamente el problema. La IA puede hacer una implementación correcta pero de un problema equivocado.

### Feedback

La comprensión general es correcta.

El principal matiz que debía ajustar era esta idea:

> “Resolver un problema mediante un sistema informático.”

El pensamiento computacional ocurre antes de decidir qué tecnología o incluso si necesitamos desarrollar software.

Una formulación más precisa sería:

> Estructurar y comprender un problema de manera que podamos diseñar una solución sistemática, que posteriormente podría implementarse mediante software.

En el ejemplo del vendedor, **Excel ya es una posible solución**, no el problema.

Antes convendría analizar:

```text
Problema:
"No tengo buen control de mi mercadería."

↓

¿Qué significa "control"?

- conocer stock;
- registrar entradas y salidas;
- analizar ventas;
- conocer clientes;
- generar información contable;
- etc.

↓

Descomponer las necesidades.

↓

Evaluar posibles soluciones.

- proceso manual;
- Excel;
- software existente;
- sistema personalizado.
```

También conviene diferenciar algunos conceptos:

- **Descomposición:** dividir un problema en partes manejables.
- **Abstracción:** conservar lo relevante e ignorar detalles innecesarios para el nivel actual.
- **Reconocimiento de patrones:** identificar semejanzas o comportamientos repetidos.
- **Diseño de solución:** definir cómo deberían funcionar conjuntamente las partes del problema.

La idea relacionada con IA es especialmente importante:

```text
Código técnicamente correcto
            ≠
Problema correctamente resuelto
```

La IA puede implementar muy bien una especificación incorrecta o incompleta.

### Idea final

El pensamiento computacional no comienza preguntando:

> “¿Cómo programo esto?”

Comienza preguntando:

> “¿Qué problema estamos intentando resolver realmente?”

A partir de ahí:

```text
Comprender
    ↓
Descomponer
    ↓
Identificar patrones
    ↓
Abstraer
    ↓
Definir reglas y restricciones
    ↓
Diseñar una solución
    ↓
Evaluar implementación
```

La tecnología aparece después de comprender suficientemente el problema.

Una idea que quiero recordar especialmente de esta sección es:

> **Antes de preocuparme por si puedo programar una solución, debo asegurarme de que estoy resolviendo el problema correcto.**