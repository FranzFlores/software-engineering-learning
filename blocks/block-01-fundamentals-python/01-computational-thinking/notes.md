# Notas — Tema 1: Pensamiento computacional y resolución de problemas

## Índice

- [1. Introducción](#1-introducción)
- [2. Definición](#2-definición)
- [3. ¿Por qué existe y qué problema resuelve?](#3-por-qué-existe-y-qué-problema-resuelve)

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

## 2. Definición

### Mi comprensión

### 2.1 Definición intuitiva
Desde el punto de vista intuitivo, el "Pensamiento computacional" se resume en transformar un problema grande o complejo en algo más simple que podamos manejar y resolver. No necesariamente se debe usar la computadora para ello.

### 2.2 Definición técnica
En lo personal, considero que básicamente tiene el mismo concepto que el punto anterior. Sin embargo, en este contexto ya entran temas específicos como la descomposición, abstracción, algoritmos,etc. 

### 2.3 Relación con resolución de problemas
Este punto es importante ya que explica, no solo "¿Qué?" hace el pensamiento computacional, sino el "¿Cómo?". Para ello se expone varias preguntas a considerar y que pueden ayudar a "aterrizar" mejor una idea. Considero clave tener siempre estas preguntas, sobre todo a la hora de trabajar con la IA, porque el tener una sección donde se aborden esas preguntas puede hacer que se llegue a resolver el problema correcto. 


### Feedback

Tu interpretación de los tres primeros puntos es correcta.

Hay un matiz que añadiría especialmente en **2.1**: el objetivo no es necesariamente hacer que el problema sea "simple", porque algunos problemas continúan siendo complejos incluso después de analizarlos.

La idea más precisa sería:

> **Transformar un problema complejo o ambiguo en una representación suficientemente clara y manejable como para poder razonar sobre él.**

Es una diferencia pequeña pero importante:

```text
Pensamiento computacional
        ≠
hacer que todo sea sencillo

Pensamiento computacional
        =
hacer que la complejidad sea manejable
```

En **2.2**, también entendiste correctamente la diferencia. No son dos definiciones contradictorias. La definición técnica simplemente hace explícitos los mecanismos que la definición intuitiva resume.

Una forma sencilla de recordarlo sería:

```text
Intuitiva:
"Ordenar el problema para poder resolverlo."

Técnica:
"Ordenarlo mediante descomposición,
abstracción, patrones, representación,
algoritmos, evaluación, etc."
```

Sobre **2.3**, tu asociación con IA es muy buena, pero añadiría otro matiz: esas preguntas no sirven únicamente para que la IA genere mejor código.

Sirven primero para que **nosotros mismos descubramos si entendemos el problema**.

Por ejemplo, si no podemos responder:

> ¿Qué resultado se considera correcto?

entonces probablemente todavía no estamos preparados para pedir una implementación, independientemente de que la escriba una persona o una IA.

Podemos verlo así:

```text
Preguntas estructuradas
        ↓
Obligan al desarrollador a razonar
        ↓
Hacen visibles huecos y supuestos
        ↓
Mejoran la especificación
        ↓
Después mejoran la interacción con la IA
```

Por tanto, la IA es una aplicación muy útil de esta disciplina, pero no es la razón por la que esas preguntas existen.

---

### Punto pendiente: 2.4 Relación con ingeniería de software

En tu resumen todavía faltaría esta pequeña parte de la sección.

La idea principal es que en ingeniería de software normalmente no resolvemos un problema una sola vez y lo abandonamos.

Construimos sistemas que después tendrán que soportar:

- nuevos requisitos;
- cambios del negocio;
- errores;
- nuevas integraciones;
- más usuarios;
- otras personas trabajando sobre el código;
- cambios tecnológicos.

Por eso comprender correctamente el problema y construir buenas abstracciones tiene consecuencias a largo plazo.

Podríamos resumirlo así:

```text
Programación:
¿Cómo hago que esto funcione?

Ingeniería de software:
¿Cómo hago que esto funcione correctamente
y siga siendo entendible y modificable
cuando el sistema cambie?
```

No significa que esa sea una definición formal de ambas disciplinas, sino un **modelo mental útil para este tema**.

---

### Idea final

El pensamiento computacional puede entenderse desde dos niveles:

```text
Nivel intuitivo

Tomar un problema difícil de manejar
y convertirlo en algo que podamos comprender
y razonar de forma estructurada.

            ↓

Nivel técnico

Utilizar herramientas mentales como:

- descomposición
- patrones
- abstracción
- representación
- algoritmos
- evaluación
```

Para resolver correctamente un problema no basta con encontrar una implementación.

Primero debemos poder explicar:

```text
¿Qué problema tengo?

¿Qué sé?

¿Qué estoy suponiendo?

¿Qué recibe la solución?

¿Qué debería producir?

¿Qué restricciones existen?

¿Qué podría salir mal?

¿Cómo sabré que funciona correctamente?
```

Estas preguntas son útiles por sí mismas y cobran todavía más importancia al trabajar con IA, porque permiten darle una especificación mejor estructurada y, sobre todo, **evaluar si la solución generada corresponde realmente al problema que queríamos resolver**.

La idea que quiero recordar de esta sección es:

> **El pensamiento computacional no elimina la complejidad; la organiza hasta hacerla suficientemente manejable como para poder diseñar y verificar una solución.**

## 3. ¿Por qué existe y qué problema resuelve?
En este punto aparece un concepto que en un inicio no lo tengo claro "comportamiento ejecutable". He consultado al respecto y de lo que entiendo es un conjunto de acciones, reglas o lógica que pueden ser entendidas por la computadora (En caso de que el concepto este erróneo, corrígelo). 

Además se presenta un diagrama bastante interesante. En este caso, en el punto "Modelo del problema", entiendo que es el proceso en el cual se analiza el problema y se lo hace mucho más manejable de llevar, justo lo que mencionabámos un poco en el punto anterior.

En cuanto al ejemplo del registrar el mismo gasto, me resulta bastante interesante. En este punto, tal vez agregaría que en el campo profesional, si podemos consultar o socializar con el cliente, a qué hace referencia determinado requerimiento ya que puede existir una brecha entre lo que entiende el cliente y el programador. 

Me gusto mucho la última sección del aporte que tiene este punto dentro del desarrollo, lo considero clave por las ventajas que se obtiene.


### Feedback

Tu interpretación general es correcta.

#### Sobre "comportamiento ejecutable"

Tu definición:

> "un conjunto de acciones, reglas o lógica que pueden ser entendidas por la computadora"

va bien encaminada.

Haría solamente un pequeño ajuste. En este contexto, **comportamiento ejecutable** se refiere al comportamiento concreto que finalmente tendrá el software y que puede ser llevado a ejecución.

Por ejemplo:

```text
Necesidad:

"Quiero saber cuánto he gastado este mes."
```

todavía no es directamente ejecutable.

Después de analizarla podríamos llegar a reglas como:

```text
1. Obtener los gastos del usuario.
2. Considerar únicamente los gastos del mes actual.
3. Excluir los gastos anulados.
4. Sumar sus importes.
5. Devolver el total.
```

Eso ya se encuentra mucho más cerca de un comportamiento que puede implementarse y ejecutarse.

Una forma sencilla de recordarlo sería:

```text
Necesidad
"Quiero controlar mis gastos."

        ↓

Comportamiento definido
"Cuando el usuario consulte el resumen mensual,
el sistema debe sumar los gastos válidos
correspondientes al período solicitado."

        ↓

Implementación
Código que realiza ese comportamiento.
```

Por tanto:

> **"Ejecutable" no significa solamente que la computadora entienda las palabras, sino que la necesidad ha sido transformada en reglas y operaciones suficientemente concretas como para poder implementarse.**

---

#### Sobre "Modelo del problema"

Tu interpretación del concepto es correcta.

El modelo del problema intenta responder:

> **¿Cómo representamos la realidad relevante de este problema sin entrar todavía en cómo vamos a programarla?**

Por ejemplo, en una aplicación de gastos podemos identificar:

```text
Usuario
Gasto
Categoría
Presupuesto
Período mensual
```

junto con reglas como:

```text
Un gasto pertenece a un usuario.

Un gasto posee un importe.

Un presupuesto corresponde a un período.

Un gasto cancelado no cuenta para ciertos cálculos.
```

Todavía no hemos decidido:

```text
clases Python
tablas SQL
endpoints
microservicios
```

Eso pertenece a etapas posteriores.

---

#### Sobre la comunicación con el cliente

Este aporte es especialmente importante y complementa muy bien la sección.

Una ambigüedad puede aparecer así:

```text
Cliente:
"No quiero gastos duplicados."

Desarrollador:
"Entonces dos gastos con el mismo importe
y la misma fecha son duplicados."
```

Pero quizá el cliente realmente quería decir:

```text
"No quiero que una doble pulsación del botón
registre dos veces la misma operación."
```

Son problemas diferentes.

Por eso, antes de implementar, puede ser necesario preguntar:

```text
¿Qué considera exactamente un duplicado?

¿Dos compras de $10 en el mismo lugar son duplicadas?

¿El problema ocurre cuando el usuario pulsa dos veces?

¿También puede ocurrir durante una importación bancaria?

¿Queremos bloquear o solamente advertir?
```

Aquí aparece una idea profesional importante:

> **El desarrollador no debería rellenar silenciosamente los huecos del requisito cuando esos huecos pueden cambiar el comportamiento del sistema.**

En algunos casos será necesario consultar al cliente; en otros, al Product Owner, analista, especialista del dominio o responsable funcional.

---

### Idea final

Entre una necesidad y el código existen varias transformaciones:

```text
Necesidad
"Quiero evitar gastos duplicados."

        ↓

Clarificación
"¿Qué significa duplicado?"

        ↓

Modelo del problema
Identificar:
- qué entidad está involucrada;
- qué datos importan;
- qué situaciones producen el problema;
- qué reglas existen.

        ↓

Diseño de solución
Definir cómo debería comportarse el sistema.

        ↓

Diseño técnico
Elegir mecanismos adecuados.

        ↓

Implementación
Convertir el diseño en software ejecutable.
```

Saltar directamente:

```text
Requisito → Código
```

puede provocar que una solución técnicamente correcta implemente una interpretación equivocada.

Por eso, cuando aparece una ambigüedad relevante:

```text
No asumir inmediatamente
        ↓
Identificar la duda
        ↓
Formular una pregunta concreta
        ↓
Validarla con quien conoce el dominio
        ↓
Actualizar el modelo del problema
```

La idea que quiero recordar de esta sección es:

> **Antes de decidir cómo resolver algo técnicamente, debo asegurarme de comprender qué comportamiento necesita realmente el negocio.**

Y una segunda idea que considero especialmente útil en el trabajo profesional:

> **Una buena pregunta realizada antes de implementar puede evitar mucho más retrabajo que una buena solución técnica construida sobre un requisito mal entendido.**
