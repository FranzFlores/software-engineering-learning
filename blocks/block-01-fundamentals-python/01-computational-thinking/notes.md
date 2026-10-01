# Notas — Tema 1: Pensamiento computacional y resolución de problemas

## Índice

- [1. Introducción](#1-introducción)
- [2. Definición](#2-definición)
- [3. ¿Por qué existe y qué problema resuelve?](#3-por-qué-existe-y-qué-problema-resuelve)
- [4. Modelo mental general](#4-modelo-mental-general)
- [5. Descomposición de problemas](#5-descomposición-de-problemas)
- [6. Reconocimiento de patrones](#6-reconocimiento-de-patrones)

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

### Mi comprensión

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

## 4. Modelo mental general

### Mi comprensión
El modelo en general, me ha gustado mucho. Algo importante a tener en cuenta es que, como dice en el texto: "No es un proceso rígidamente lineal", lo que me indica que no es un proceso donde se deba seguir todos los pasos sino acoplarlo al problema que se trata de resolver.

### 4.1 Necesidad / problema
Es la descripción de la situación que se desea cambiar o mejorar, es el punto principalal entender dentro del proceso.

### 4.2 Clarificación y restricciones
Es esta fase, por llamarle de alguna manera, se "transforma" la necesidad identificada previamente en condiciones específicas que permitan ir atterizando el problema.

### 4.3 Descomposición
Se aplica el famoso "Divide y vencerás" donde se separa las condiciones previamente identificadas en partes más fáciles de analizar

### 4.4 Patrones
Consiste en el proceso de buscar elementos y situaciones que se parezcan. En lo personal (no se si estoy en lo correcto) que en este paso se puede empezar a identificar elementos que en código puede ser reutilizables y genéricos

### 4.5 Abstracción
En lo que entiendo, consiste en enfocarse en los elementos más relevante de un sistema y "ocultar" los detalles específicos del mismo.

### 4.6 Diseño de solución
En este paso es básicamente empezar a encontrar la solución. Puede ser marcando los pasos del flujo ideal de funcionamiento, de ahí que no sea necesario escoger una tecnología aún.

### 4.7 Validación
En este caso, si se empieza a analizar los flujos principales, alternos y posibles errores. Un término nuevo para mí en este contexto fue "concurrencia" que lo entiendo como la capacidad de que el sistema realice varias acciones al mismo tiempo.

### 4.8 Representación
Es la forma en la cual se mostrará la solución. Personalmente lo entiendo como el entregable del proceso. Al ser una etapa previa a la implementación, por experiencia, siempre me gusta usar diagramas UML como diagramas de clases o diagramas de caso de uso, los considero prácticos para el cliente.

### 4.9 Selección tecnológica
Básicamente es elegir la tecnología a usar para la implemetación de la solución. 

### 4.10 Implementación y retroalimentación
Al momento de implementar es muy probable que se noten nuevos flujos que no estuvieron previstos y toque realizar el proceso nuevamente. Personalmente, considero que varias iteraciones puede hacer una solución más robusta aunque claro se agrega más complejidad


## Feedback

Tu comprensión general del modelo es **muy buena**. Hay, sin embargo, varios matices importantes que vale la pena fijar porque serán útiles posteriormente en arquitectura y diseño.

---

### Sobre que el proceso no sea lineal

Tu interpretación es correcta, pero haría una pequeña precisión.

Cuando el documento dice:

> "No es un proceso rígidamente lineal"

no significa exactamente:

> "Podemos omitir cualquier paso."

Significa principalmente que **el razonamiento puede avanzar y retroceder entre ellos**.

Por ejemplo:

```text
Diseño una solución
        ↓
Descubro que no sé qué ocurre si el gasto está duplicado
        ↓
Regreso a requisitos
        ↓
Consulto el comportamiento esperado
        ↓
Actualizo el modelo
        ↓
Continúo diseñando
```

Además, en problemas pequeños algunos pasos pueden realizarse mentalmente y casi simultáneamente.

Por eso una formulación que considero más precisa sería:

> **No todos los pasos necesitan convertirse en una actividad formal, pero las preguntas que representan siguen siendo útiles.**

---

### Sobre 4.3 Descomposición

La asociación con **"divide y vencerás"** es útil como modelo mental.

Pero conviene no confundirlo con el paradigma algorítmico del mismo nombre (*divide and conquer*).

Aquí estamos hablando de una idea más general:

```text
Problema grande
        ↓
Subproblemas comprensibles
```

mientras que *Divide and Conquer* en algoritmos tiene un significado más específico que veremos posteriormente.

---

### Sobre 4.4 Patrones y reutilización de código

Aquí tu intuición es correcta, pero existe una distinción importante.

Sí, reconocer patrones puede posteriormente permitir descubrir:

- lógica reutilizable;
- componentes comunes;
- funciones compartidas;
- abstracciones;
- patrones de diseño.

Pero **no deberíamos convertir inmediatamente una semejanza en código genérico**.

Por ejemplo:

```text
Gasto:
importe
fecha
moneda

Ingreso:
importe
fecha
moneda
```

podemos decir:

> "Existe un patrón en los datos."

Pero todavía no necesariamente:

> "Necesitamos una clase genérica `FinancialTransaction`."

Primero debemos comprobar si la semejanza es suficientemente profunda.

Por eso:

```text
Reconocer un patrón
        ↓
Investigar la semejanza
        ↓
Entender diferencias
        ↓
Solo después considerar reutilización
```

Una idea importante para recordar:

> **La reutilización puede ser consecuencia del reconocimiento de patrones, pero no es obligatoriamente su objetivo inmediato.**

---

### Sobre 4.5 Abstracción

Tu explicación:

> "enfocarse en los elementos más relevantes y ocultar los detalles específicos"

es bastante buena.

Solo cambiaría ligeramente la palabra **"ocultar"**, porque puede hacer que abstraction e *information hiding* parezcan exactamente lo mismo.

Preferiría:

> **Abstraer consiste en representar únicamente los detalles relevantes para el nivel de razonamiento actual y dejar fuera temporalmente aquellos que no necesitamos.**

Por ejemplo:

```text
Estamos analizando:

"Realizar un pago."
```

Podemos trabajar con:

```text
importe
medio de pago
resultado
```

sin necesitar todavía:

```text
HTTP
TLS
JSON
SDK del proveedor
timeouts
```

Los detalles no necesariamente están "escondidos" técnicamente.

Simplemente **no forman parte del modelo actual**.

---

### Sobre 4.7 Concurrencia

Aquí sí conviene hacer una corrección importante.

Tu definición:

> "la capacidad de que el sistema realice varias acciones al mismo tiempo"

se aproxima, pero **concurrencia no significa necesariamente simultaneidad**.

Una forma más precisa sería:

> **Concurrencia ocurre cuando varias operaciones pueden estar en progreso durante períodos que se solapan y el sistema debe coordinar correctamente sus interacciones.**

Por ejemplo:

```text
Solicitud A:
leer total = 100
                      Solicitud B:
                      leer total = 100

Solicitud A:
sumar 20 → 120

                      Solicitud B:
                      sumar 30 → 130
```

Si ambas trabajan sobre el mismo dato podríamos terminar con:

```text
130
```

cuando el resultado esperado era:

```text
150
```

Las operaciones no necesitan ejecutarse exactamente en el mismo nanosegundo.

Lo importante es que **sus períodos de ejecución se solapan y pueden interferir entre sí**.

Una distinción que estudiaremos más adelante será:

```text
Concurrencia
Varias tareas progresan durante períodos solapados.

Paralelismo
Varias tareas se ejecutan literalmente al mismo tiempo.
```

Por ahora basta con quedarte con esa diferencia conceptual.

---

### Sobre 4.8 Representación

Aquí también haría un pequeño ajuste.

La representación **puede ser un entregable**, pero no necesariamente lo es.

Su objetivo principal es:

> **externalizar el diseño para poder comprenderlo, discutirlo y validarlo.**

Por ejemplo, un pseudocódigo que escribes durante cinco minutos para verificar una lógica quizá nunca llegue al cliente ni al repositorio.

Sigue siendo una representación útil.

Respecto a UML, tu experiencia tiene sentido, pero elegiría el diagrama según la pregunta que queremos responder.

Por ejemplo:

```text
Caso de uso
→ ¿Qué puede hacer cada actor?

Secuencia
→ ¿Quién interactúa con quién y en qué orden?

Estados
→ ¿Qué estados puede tener una entidad?

Clases
→ ¿Qué estructura conceptual o de diseño existe?

Flowchart
→ ¿Qué decisiones sigue un proceso?
```

Una pequeña observación importante:

Un **diagrama de clases** normalmente se encuentra más cerca del diseño técnico que de la representación inicial del problema.

Para conversar con un cliente, dependiendo del contexto, pueden resultar más accesibles:

- casos de uso;
- diagramas de actividad;
- flujos;
- wireframes;
- diagramas simples del proceso.

No significa que un diagrama de clases sea incorrecto, sino que debería utilizarse cuando ayude a responder la pregunta actual.

---

### Sobre 4.10 Iteraciones y robustez

Tu idea:

> "varias iteraciones pueden hacer una solución más robusta"

tiene sentido, pero añadiría un matiz importante.

Las iteraciones aportan valor cuando incorporan **nueva información o validación**.

No necesariamente:

```text
más iteraciones
=
mejor solución
```

Podríamos iterar muchas veces y simplemente añadir complejidad.

Una secuencia saludable sería:

```text
Implementar
    ↓
Obtener nueva información
    ↓
Evaluar
    ↓
Corregir el modelo
    ↓
Simplificar o mejorar
```

De hecho, una buena iteración también puede descubrir que debemos **eliminar complejidad**, no agregarla.

Así que preferiría pensar:

> **Las iteraciones permiten ajustar progresivamente una solución conforme obtenemos nueva información.**

---

## Idea final

Este modelo mental no es una receta rígida, sino una guía para evitar saltar demasiado pronto desde:

```text
"Tengo una necesidad"
```

hasta:

```text
"Voy a escribir código."
```

El recorrido puede entenderse así:

```text
¿Qué necesito resolver?
        ↓
¿Qué significa realmente?
        ↓
¿En qué partes puedo dividirlo?
        ↓
¿Qué elementos se repiten?
        ↓
¿Qué información importa?
        ↓
¿Cómo debería comportarse la solución?
        ↓
¿Qué podría salir mal?
        ↓
¿Cómo puedo representar y validar la idea?
        ↓
¿Qué tecnología satisface esas necesidades?
        ↓
Implementar
        ↓
Aprender de la implementación
        ↓
Ajustar cuando sea necesario
```

Tres ideas que quiero conservar especialmente de esta sección son:

> **Reconocer patrones puede conducir a reutilización, pero una semejanza no justifica automáticamente crear una abstracción genérica.**

> **Concurrencia no significa necesariamente ejecutar dos acciones exactamente al mismo tiempo; significa que varias operaciones pueden solaparse y necesitar coordinación.**

> **El modelo mental no busca obligarme a documentar cada paso, sino evitar que omita preguntas importantes antes de tomar decisiones técnicas.**

## 5. Descomposición de problemas

### Mi comprensión
### 5.1 Qué significa descomponer
En este apartado, entiendo que descomponer un problema involucra tomar un problema grande y "dividirlo" en problemas más pequeños que permitan manejarlo de mejor manera. Este proceso se realiza antes de implementar código ya que puede involucrar tomar decisiones de arquitectura como el uso de microservicios

### 5.2 Cómo identificar subproblemas
En cuanto a las preguntas que se ofrecen, me gusta mucho poder identificar subproblemas mediante definir responsabilidades, datos, resultados, etc. 

### 5.3 Cómo determinar límites
Me agradó mucho poder contar con los elementos que conforman un buen límite. Del listado la única que no me queda del todo claro es "dependencias explícitas". De lo que comprendo, significa que se conoce adecuadamente los elementos que necesita un componente para poder funcionar correctamente. Por ejemplo, para poder "Registrar un gasto", debo tener acceso a una BD para almacenar la información.

### 5.4 Dependencias entre subproblemas
Me parece que este concepto guarda cierta relación con el punto anterior. En este caso, si bien cada problema se analiza de manera independiente, no se debe eliminar las relaciones que tiene. Se me ocurre como ejemplo de que un inicio de sesión se puede analizar como proceso pero guarda relación con usuarios, cuentas, roles, etc.

### 5.5 Descomposición demasiado grande
Algo que me llamó la atención en este punto es que si "resulta difícil de nombrar a un problema" probablemente es por que su alcance aún es muy amplio. Se me ocurre como ejemplo decir "la autenticación de usuarios", donde puede existe diferentes procesos como si se debe o no permitir que los usuarios se registren, el inicio de sesión, el guardado de contraseñas seguras, etc.

### 5.6 Descomposición demasiado pequeña
El ejemplo me gustó mucho, más parece un pseudocódigo de un proceso que un subproblema. 

## Feedback

Tu comprensión general de la sección es correcta. Hay algunos matices importantes que conviene ajustar.

### Sobre 5.1 — Descomponer antes de implementar

Es correcto que la descomposición ocurre antes del código y que puede terminar influyendo en decisiones arquitectónicas.

Sin embargo, evitaría asociar directamente:

```text
Descomposición
    ↓
Microservicios
```

La descomposición primero descubre **responsabilidades y límites conceptuales**.

Por ejemplo:

```text
Sistema de gastos
├── Registro de movimientos
├── Presupuestos
├── Reportes
└── Notificaciones
```

Eso no significa que cada parte deba convertirse en un microservicio.

Posteriormente podríamos implementar todo como:

- un monolito;
- un monolito modular;
- varios servicios;
- otra arquitectura.

Una idea importante sería:

> **La descomposición descubre cómo está estructurado el problema; la arquitectura decide posteriormente cómo representar técnicamente esos límites.**

---

### Sobre 5.2 — Identificación de subproblemas

Las preguntas sobre responsabilidades, datos y resultados son especialmente útiles porque evitan dividir simplemente por intuición.

Una pregunta que añadiría mentalmente es:

> **¿Puedo explicar este subproblema de manera relativamente independiente?**

Por ejemplo:

```text
Calcular resumen mensual
```

puede explicarse indicando:

- qué información necesita;
- qué reglas aplica;
- qué resultado produce;

sin necesidad de explicar todo el sistema de gastos.

Eso es una buena señal de que existe un subproblema razonable.

---

### Sobre 5.3 — Dependencias explícitas

Tu interpretación está bien encaminada:

> una dependencia es algo que un subproblema necesita para poder cumplir su responsabilidad.

Pero haría una corrección importante en el ejemplo.

Decir:

```text
Registrar gasto necesita una base de datos
```

ya introduce una decisión tecnológica.

En este nivel sería mejor decir:

```text
Registrar gasto necesita algún mecanismo
para conservar el gasto.
```

Posteriormente podremos decidir si ese mecanismo será:

```text
PostgreSQL
archivo local
API externa
almacenamiento en memoria
etc.
```

También existen dependencias que no son infraestructura.

Por ejemplo:

```text
Registrar gasto
│
├── necesita conocer al usuario
├── necesita validar la categoría
├── necesita las reglas del gasto
└── necesita conservar el resultado
```

Que sean **explícitas** significa básicamente que podemos decir claramente:

> "Para realizar X necesito Y."

en lugar de que esa relación quede oculta o aparezca inesperadamente durante la implementación.

---

### Sobre 5.4 — Dependencias entre subproblemas

Tu ejemplo de autenticación va en la dirección correcta.

Aquí conviene distinguir entre:

```text
Conceptos relacionados
```

y:

```text
Dependencias entre procesos
```

Por ejemplo:

```text
Inicio de sesión
```

está relacionado conceptualmente con:

- usuario;
- cuenta;
- roles.

Pero podríamos identificar dependencias más concretas como:

```text
Validar credenciales
        ↓
necesita obtener la cuenta

Crear sesión
        ↓
depende de que las credenciales sean válidas

Determinar permisos
        ↓
depende de roles o políticas asociadas
```

Esto permite descubrir no solamente **qué cosas están relacionadas**, sino también:

- qué necesita cada proceso;
- qué debe ocurrir antes;
- qué información pasa de uno a otro;
- qué sucede si una dependencia falla.

---

### Sobre 5.5 — Descomposición demasiado grande

La observación sobre la dificultad para nombrar algo es una heurística útil.

Tu ejemplo de:

```text
Autenticación de usuarios
```

también muestra algo interesante: el nombre no siempre será malo por ser amplio.

Podría ser perfectamente válido como **área o problema de alto nivel**.

Lo que ocurre es que probablemente todavía necesitemos descomponerlo para trabajar sobre él:

```text
Autenticación
├── Registro
├── Inicio de sesión
├── Recuperación de acceso
├── Gestión de credenciales
└── Cierre / renovación de sesión
```

Además, aquí hay una pequeña precisión:

```text
Roles
```

normalmente se relaciona más con **autorización** que con autenticación.

Una distinción útil para recordar:

```text
Autenticación
"¿Quién eres?"

Autorización
"¿Qué puedes hacer?"
```

Aunque ambos procesos suelen estar relacionados dentro de un sistema.

---

### Sobre 5.6 — Descomposición demasiado pequeña

Tu observación es exactamente el problema que intenta mostrar el ejemplo.

Cuando llegamos a algo como:

```text
leer variable
convertir valor
llamar función
incrementar contador
```

ya no estamos necesariamente descomponiendo el **problema**, sino describiendo pasos de una posible implementación.

Una buena comparación sería:

```text
Descomposición del problema:

Registrar gasto
├── validar
├── clasificar
├── conservar
└── reflejar en resumen
```

frente a:

```text
Detalle de implementación:

leer amount
convertir a Decimal
llamar save()
sumar variable
```

La primera ayuda a razonar sobre responsabilidades.

La segunda puede ser útil más adelante como pseudocódigo o implementación, pero tiene un nivel de detalle demasiado bajo para esta etapa.

---

### Idea que conviene conservar

El principal criterio que extraería de toda esta sección sería:

> **Una buena descomposición no intenta producir la mayor cantidad posible de partes, sino encontrar partes suficientemente independientes y comprensibles como para poder razonar sobre ellas sin perder las relaciones que existen entre sí.**

Y una segunda idea especialmente importante para las próximas secciones:

```text
Descomponer el problema
        ≠
diseñar inmediatamente módulos técnicos
```

Primero descubrimos **responsabilidades y límites del problema**.

Después podremos decidir cómo esos límites se traducen —o no— en funciones, clases, módulos, servicios o componentes arquitectónicos.

## 6. Reconocimiento de patrones
### Mi comprensión

### Qué significa
La definición bridada, hace que se remarqué que al tratar de encontrar semejanzas importantes entre ciertas situaciones, se trata de reutilizar "razonamiento" en lugar de código.

### Patrones de datos
El ejemplo brindado es bastante interesante. En lo personal, basado en el ejemplo propuesto, pienso que tal vez se puede "optimizar" todo en una sola clase llamada "Movimiento" donde se tiene todos los campos propuestos y se tiene uno adicional llamado "tipo" donde se identificaría si es "Gasto" o "Ingreso". Con todo, tengo claro de que esto NO necesariamente significa que van a compatir una cosa o tabla.

### Patrones en comportamiento
El ejemplo no lo he entidido bien. De lo que comprendo, es que pueden existir varias acciones como crear o editar un gasto, que probablemente afecten a una misma operación como el presupuesto o resumen mensual.

### Patrones de requisitos
En este caso, del ejemplo provisto, comprendo que a partir de los requisitos con intervalo común, se puede obtener un requisito más general.

### Reutilizar soluciones conocidas
En este caso, lo que entiendo es que, a partir de procesos o soluciones previamente usados se pueden aplicar los mismos para problemas con similar estructura.

### Reconocer patrón ≠ aplicar patrón de diseño
Correcto, aunque me gustaría que uses un ejemplo sencillo relacionado al tema de la aplicación para llevar el control financiero.

## Feedback

Tu comprensión general de la sección es correcta. La idea principal que ya estás captando es esta:

> **Reconocer patrones no significa buscar inmediatamente código que pueda reutilizarse, sino detectar semejanzas que permitan reutilizar razonamiento.**

A partir de ahí sí pueden aparecer oportunidades de reutilización técnica, pero eso ocurre después.

---

### Sobre qué significa reconocer patrones

Tu interpretación es correcta.

Cuando encontramos dos situaciones parecidas, podemos preguntarnos:

```text
¿Qué tienen realmente en común?

¿Qué razonamiento utilizado en una de ellas
puedo aplicar también en la otra?
```

Por ejemplo, si ya resolvimos:

```text
Consultar gastos por mes
```

y luego aparece:

```text
Consultar ingresos por mes
```

podemos reconocer que ambos problemas comparten una estructura:

```text
movimientos
+
intervalo temporal
+
usuario
```

Esto nos permite reutilizar parte del **modelo mental** antes de pensar siquiera en reutilizar código.

---

### Sobre patrones en datos

Aquí aparece un punto muy importante en tu propuesta de crear una clase `Movimiento`.

Tu razonamiento es perfectamente válido como **hipótesis de diseño**:

```text
Movimiento
- fecha
- importe
- moneda
- tipo
```

donde:

```text
tipo = gasto | ingreso
```

Pero precisamente esta sección intenta enseñarnos a no saltar todavía a esa conclusión.

Lo que podemos afirmar con seguridad es:

```text
Gasto e ingreso comparten ciertos datos.
```

Eso es un **patrón detectado**.

Después podemos evaluar diferentes representaciones:

```text
Opción A

Movimiento
- fecha
- importe
- moneda
- tipo
```

o:

```text
Opción B

Gasto
- fecha
- importe
- moneda

Ingreso
- fecha
- importe
- moneda
```

o incluso otras alternativas.

La pregunta relevante sería:

> **¿Las semejanzas entre gasto e ingreso son suficientemente importantes como para tratarlos como el mismo concepto?**

Imagina que después aparecen reglas como:

```text
Gasto:
- afecta presupuesto;
- puede tener comercio;
- puede tener categoría de consumo.

Ingreso:
- puede tener fuente;
- puede ser salario;
- puede tener reglas fiscales diferentes.
```

Entonces quizá:

```text
Movimiento
```

siga siendo una buena abstracción para algunas operaciones, pero no necesariamente para todo el sistema.

La idea importante sería:

```text
Detectar semejanza
        ↓
Reconocer patrón
        ↓
Analizar también diferencias
        ↓
Evaluar abstracción
        ↓
Recién después diseñar clases/tablas
```

Por eso tu propuesta no está mal. Simplemente está **un paso más adelante** de lo que necesitamos concluir en esta sección.

---

### Sobre patrones en comportamiento

Tu interpretación es correcta.

El ejemplo intenta mostrar que distintas acciones pueden producir una **misma consecuencia conceptual**.

Por ejemplo:

```text
Registrar gasto
Editar gasto
Cancelar gasto
```

son acciones diferentes.

Pero las tres pueden provocar:

```text
El resumen mensual debe reflejar el nuevo estado.
```

También podrían afectar:

```text
Presupuesto mensual
Estadísticas
Gráficas
Alertas
```

Entonces detectamos un patrón de comportamiento:

> **Cuando cambia un gasto, cierta información derivada puede necesitar actualizarse.**

Podemos representarlo así:

```text
Crear gasto ────────┐
                    │
Editar gasto ───────┼──→ Cambia información financiera derivada
                    │
Cancelar gasto ─────┘
```

Todavía no estamos diciendo:

```text
"Debemos usar eventos."
```

ni:

```text
"Debemos crear un Observer."
```

Solo estamos reconociendo una regularidad.

Este tipo de patrón resulta muy útil porque más adelante puede ayudarnos a descubrir responsabilidades del sistema.

---

### Sobre patrones en requisitos

Tu comprensión es correcta.

Si tenemos:

```text
Filtrar gastos por mes.
Filtrar ingresos por mes.
Filtrar transferencias por mes.
```

podemos detectar una necesidad más general:

```text
Consultar movimientos financieros por período.
```

Sin embargo, hay que tener cuidado con una cosa.

El requisito general:

```text
Consultar movimientos por período
```

no necesariamente **reemplaza** los requisitos anteriores.

Puede servir para descubrir una capacidad común, pero cada tipo de movimiento todavía podría tener reglas particulares.

Podemos verlo como:

```text
Requisitos específicos
        ↓
Detectar semejanza
        ↓
Capacidad común
```

y no necesariamente como:

```text
Requisitos específicos
        ↓
Eliminar diferencias
```

---

### Sobre reutilizar soluciones conocidas

Tu interpretación también es correcta.

Si encontramos un problema cuya estructura ya conocemos, podemos recuperar razonamiento previo.

Por ejemplo:

En una parte de la aplicación tenemos:

```text
Presupuesto

activo
agotado
cerrado
```

y descubrimos que las transiciones entre estados están estrictamente controladas.

Más adelante aparece:

```text
Meta de ahorro

activa
completada
cancelada
```

Podemos reconocer:

> Ambos problemas involucran entidades que atraviesan estados definidos y cuyas transiciones tienen reglas.

Esto puede hacer que recordemos el concepto de:

```text
máquina de estados
```

Pero todavía debemos comprobar si realmente aporta valor en el nuevo problema.

Por tanto:

> **Reutilizar soluciones conocidas significa reutilizar experiencia y razonamiento, no copiar automáticamente la implementación anterior.**

---

### Sobre reconocer patrón ≠ aplicar patrón de diseño

Tomemos un ejemplo sencillo del sistema financiero.

Supongamos que tenemos tres formas de calcular una comisión:

```text
Transferencia bancaria:
1%

Tarjeta:
2%

Transferencia internacional:
3%
```

Observamos un patrón:

```text
Existe una operación:

calcular comisión

pero el cálculo cambia
según el tipo de operación.
```

Podríamos pensar inmediatamente:

```text
Strategy Pattern
```

y crear:

```text
CommissionStrategy
├── BankCommissionStrategy
├── CardCommissionStrategy
└── InternationalCommissionStrategy
```

Pero antes deberíamos preguntarnos:

```text
¿Realmente existen muchos algoritmos?

¿Van a cambiar frecuentemente?

¿Necesitamos agregarlos dinámicamente?

¿Hay comportamiento complejo?

¿O simplemente son tres reglas pequeñas?
```

Quizá para nuestro sistema actual sea suficiente:

```text
SI tipo = bank:
    comisión = amount * 0.01

SI tipo = card:
    comisión = amount * 0.02

SI tipo = international:
    comisión = amount * 0.03
```

o alguna representación sencilla equivalente.

Entonces:

```text
Patrón reconocido:
"El cálculo cambia según el tipo."

        ↓

Posible solución:
Strategy

        ≠

Obligación:
usar Strategy
```

Si posteriormente aparecen:

```text
20 tipos de comisión
reglas complejas
proveedores diferentes
cambios frecuentes
configuración dinámica
```

entonces Strategy podría empezar a aportar mucho más valor.

La lección es:

> **Un patrón de diseño debe resolver una complejidad existente, no crear complejidad porque reconocimos una semejanza.**

---

## Idea final

El reconocimiento de patrones puede verse así:

```text
Observar varios casos
        ↓
Detectar semejanzas
        ↓
Preguntar qué tienen realmente en común
        ↓
Reutilizar razonamiento
        ↓
Analizar también sus diferencias
        ↓
Evaluar si conviene abstraer o reutilizar una solución
```

En el proyecto de gastos podría aparecer en distintos niveles:

```text
Datos:
Gasto e ingreso comparten fecha, importe y moneda.

Comportamiento:
Crear, editar y cancelar gastos afectan resúmenes.

Requisitos:
Gastos, ingresos y transferencias necesitan consultas por período.

Soluciones:
Varias entidades pueden requerir controlar transiciones de estados.
```

Pero reconocer esas semejanzas **no obliga** a crear inmediatamente:

```text
clases genéricas
tablas compartidas
microservicios
patrones GoF
arquitecturas complejas
```

La idea que quiero recordar de esta sección es:

> **Primero reconozco la semejanza. Después compruebo si es suficientemente importante y estable. Solo entonces decido si merece convertirse en una abstracción o solución reutilizable.**

