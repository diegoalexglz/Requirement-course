# INTRODUCCIÓN

## ¿Qué es la ingeniería de requerimientos?

*'Es el arte de quitar, no de poner'*

## ¿Qué es un requerimiento?

**Es**:

- Definición de lo que un software debe hacer.
- Especificación de las restricciones en su operación e implementación (limitaciones de hardware, de presupuesto, de tecnología).

**Identifica:**

- Las necesidades de las usuarios.
- Las funciones que debe tener el producto para satisfacerlas.

Describe **atributos de calidad**, como:

- Desempeño
- Seguridad
- Confiabilidad
- Disponibilidad

Contiene **información del usuario**, como:

- Quiénes son
- Intereses
- Prioridades

E información del **ambiente de operación**.

## Actividades de un requerimiento

> Elicitación.

Recolección de información por parte de los usuarios.

> Análisis

Tareas orientadas al entendimiento de las necesidades de los usuarios.

> Especificación

Tareas para establecer de forma clara, concisa y completa las funciones pque deben estar presentes para la solución de las necesidades.

> Validación

Tareas para aprobar o descartar las propuestas de solución. 

## 'El cliente no sabe lo que quiere'

Un proceso de requerimientos debe **empezar por conocer la situación actual del usuario (stakeholders)**, es decir, preguntando:

*¿cómo te encuentras hoy? ¿cuáles son tus objetivos? ¿qué te gustaría estar haciendo y todavía no puedes?*

en vez de:

*¿qué es lo que quieres?*

No se debe pensar primero en la tecnología, **se debe entender el problema** y **proteger al usuario de sí mismo**, para que no pida cosas que no necesita y podamos explicarle qué impacto tiene cada una de las solicitudes y cambios que hace.

# STAKEHOLDERS

Son los interesados o que tienen un impacto cuando se hace el sistema. Representan la voz de las necesidades a solucionar con el sistema.

- Patrocinadores
- Usuarios directos
- Usuarios indirectos (otras pequeñas empresas que se puedan beneficiar, por ejemplo, los dueños de restaurantes con las apps de mapas)
- Definidores de reglas (pueden ser externos, como instituciones de gobierno, e incluso pueden no usar el sistema, pero definen las reglas de negocio a las que se debe ajustar)

# NIVELES

> N1 - De negocios

Son la razón de ser del producto. Contiene los objetivos globales y la dirección que debe tomar el proyecto.

Responden a: **¿Qué se debe hacer?**

> N2 - De usuario

Actividades y objetivos de trabajo que persiguen los usuarios y que deben incluirse en el software.

Responden a: **¿Para quién es el software?**

> N3 - De software

Describen lo que el software debe de hacer, las funciones que se deben incluir y otros **atributos de calidad**, que se conocen como ***Requerimientos No Funcionales*.**

Responden a: **¿Cómo debe hacerse?**

NOTA: Todos los **Requerimientos No Funcionales son obligatorios**.

# TIPOS

> Deseables

Estéticos. Nice to have, si tenemos tiempo.

> Importantes

Valiosos, pero pueden esperar. Se negocian por otros que son más prioritarios.

> No implementables

Poco valor y alto costo. Suelen ser para pocos usuarios y la mayoría quedan fuera de los objetivos del producto, a excepción de 1 o 2.

> Obligatorios

Sin ellos, el producto no tiene razón de ser, se vuelve inútil.

**Ejemplo:**

D	->	Editar en línea

I	  ->	Edición múltiple de registros

N	->	Animación con sonido cuando se guarda un registro

O	->	Guardar y editar información de los clientes


## ¿Cómo identificar los tipos de requerimiento

En los 3 niveles se encuentran los 4 tipos de requerimientos, por lo que para identificar y priorizar los requerimientos siempre se deben tener en mente los requerimientos de **Nivel 1** (de negocio); los que ayudan a conseguir **los objetivos de negocio son los obligatorios**.

Así, el orden para lograr esto es:

1. Identificar los Stakeholders
2. Levanta los requerimientos
3. Identificar el nivel de los requerimientos
4. Priorizar los requerimientos

# RECOLECCIÓN (ELICITACIÓN)

Las brechas en el lenguaje técnico deben reducirse. No se debe hacer preguntas al usuario cómo ¿cuál sistema? ¿qué harramientas? ¿web, móvil o de escritorio? ¿responsivo?, etc...

El usuario hablará desde su vocabulario, desde su contexto y las cosas que conocen y hacen.

## Técnicas de recolección

- **Entrevistas** con los usuarios (individuales o en grupos pequeños).
  - Resuelve preguntas iniciales.
  - El facilitador escucha activamente, solo se interviene para aclarar algo.
- **Talleres**
  - Se discuten ideas, no personas.
  - El facilitador conduce y lee el lenguaje corporal para mantener la motivación y ganas de participar de los demás.
- **Focus groups**
  - Es una reunión con un subconjunto de los usuarios, llamado 'champions'.
  - Explora actitudes, preferencias y necesidades.
  - Sirve para validar qué se parece a soluciones ya existentes.
  - El facilitador debe ser neutral.
  - La reunión debe ser grabada.
- **Observación**
  - Registra las herramientas, áreas y objetos del área de trabajo del usuario.
  - No hay interacción con los usuarios.
  - Se observa a los usuarios mientras hacen sus actividades.
  - El facilitador no debe interrumpir.
- **Encuestas**
  - Debe tener preguntas cerradas y respuestas mutuamente excluyentes.
  - Usa escalas numéricas o escalas de opinión (excelente, regular, malo).
- **Análisis de documentos**
  - Se revisan manuales, procesos y bibliotecas de problemas.
  - Puede revelar cosas que la gente no dice.
- **Evaluación heurística**
  - Evalúa un producto existente similar al que se quiere desarrollar (puede ser el producto actual del usuario o uno parecido del mercado).
  - Evalúa qué tan bien funciona y sus oportunidades de mejora.

# ANÁLISIS

*'Tenemos mucha documentación de requerimientos, pero todavía no sabemos por dónde empezar.'*

## Contexto

Una app de software no está aislada. El contexto **es útil para definir los Requerimientos No Funcionales**.

Hay otros factores como hardware, redes y otras apps.

Para definir el contexto, se deben buscar:

- **Otras apps** y software que se esté usando (mencionadas por el usuario o en documentos)
  - instancias
  - versiones
  
- **Ubicaciones remotas**: dónde se encuentran geográficamente los usuarios y otros sistemas que interactúan
  - infraesructura de comunicaciones
  - acceso a la red
  
- **Hardware**: qué hardware y dispositivos se usarán para correr el software
  - versiones
  - capacidad
  - cantidad
  - ¿actualizable?



✓	Adaptar el sistema al usuario.

X	Adaptar el usuario al sistema.

## Dominio de información

> Cliente

Dispositivo o programa que se comunica con un servidor para consultar información o ejecutar funciones de hardware.

Del cliente nos interesa saber:

- Origen
- Dirección IP
- Capacidad
- Permisos

Así, se podrán definir las:

Entidades de información en el software + Relaciones en el dominio

> Dominio

Su análisis nos describe cómo el usuario entiende la información, es un diccionario de datos (pero no una base de datos), de qué significa para un usuario un concepto que usa con frecuencia.

Esto permite saber en qué procesos se origina y transforma la información.

## Procesamiento de información

Se debe definir cómo y dónde cambia (se procesa) la información, ya que puede estar en diferentes partes del sistema y en diferentes momentos.

Por ejemplo, si nuestra app utiliza a un tercero para autenticar al usuario, como Facebook login, tanto la app como Facebook tienen datos del usuario, pero con distintos usos, en distintos lugares y momentos.

## Comportamiento

Es cómo reacciona el sistema ante ciertos estímulos o estados.

Es importante crear escenarios para:

- Funcionamiento correcto
- Errores
- Excepciones
- Alta demanda
- Ancho de banda limitado

Por ejemplo, el permitir o impedir guardar un cambio, o el cancelar una transacción si el servidor tarda en completar una petición.

Recursos que se pueden usar son:

- Diagramas de flujo
- Diagramas de actividad UML
- Diagramas de secuencia
- Diagramas de clases
- Diagramas de contexto

# ESPECIFICACIÓN

'- ¿Qué tengo que hacer después de guardar la info? - Invéntate algo y luego lo cambiamos'

Es imposible memorizar toda la info de los requerimientos. A lo largo del proyecto surgirán dudas, que a su vez generarán suposiciones y diferencias en el entendimiento entre los miembros del equipo, que a su vez, causarán retrabajos, retrasos e insatisfacción de los stakeholders.

La especificación también permite entender cómo se hizo el proyecto y las implicaciones que tendría hacerle cambios.

Para la especificación se recomienda el uso de una herramienta que facilite la búsqueda de información, la edición, la colaboración y que gestione automáticamente los cambios de versiones, como lo es una **WIKI**.

Una buena especificación responde a las preguntas a continuación.

## ¿Qué se va a resolver y por qué es importante?

Para tenerlo presente, se debe hacer un **resumen ejecutivo** con:

- Estado actual y problemática
- Estado deseado, expresado en objetivos smart
- Visión del software
- Funciones principales
- Riesgos del proyecto

Acá NO se debe usar lenguaje técnico.

## ¿A quién impactamos?

Se debe especificar quiénes son los patrocinadores, los usuarios directos, indirectos, y definidores de reglas.

## ¿Qué quieren hacer los usuarios?

Se deben especificar las actividades y objetivos que quieren completar con nuestro software, pero el enfoque está en actividades completas del usuario, no funciones específicas del software.

Por ejemplo, un publicista quiere diseñar correos electrónicos para enviar promociones a sus clientes. En este caso, el objetivo es enviar promociones y la actividad es diseñar el correo.

Una herramienta para espcificar los requerimientos de usuario son las **User Stories**, que son la **unidad más pequeña de trabajo en un framework ágil**, y que se define como una explicación de una función de software escrita desde la perspectiva del usuario, que desea una nueva característica.

## ¿Qué debe hacer el software?

Se debe especificar qué hace cada elemento del software, sin el cómo.

Por ejemplo, con el ejemplo del publicista, las funciones pueden ser: alinear texto, elegir fuente, agregar imagen, crear destinatarios, enviar correo.

Es importante especificar el comportamiento de las funciones durante **uso normal, error y excepción**.

Una herramienta útil son las **maquetas** o **mock ups**, que son prototipos que muestran cómo sería el producto.

## ¿Cuál y cómo es el ambiente operativo?

Se debe especificar:

- las características de los dispositivos en los que se ejecutará el software.
- las característicasde las redes de comunicación entre los dispositivos.
- cuántos usuarios hay y dónde se localizan.
- días y horas de mayor uso.
- ecosistema de software con el que convive el producto (programas, versiones, sistemas operativos).

## ¿Cuáles son las interfaces de hardware y software?

Se debe especificar:

- cuáles son las apps con las que se comunicará el sistema
- las características de las interfaces (API) que se usarán para comunicarse con las otras apps
- problemas conocidos con el uso de las interfaces

## ¿Cuáles son las restricciones tecnológicas?

Se debe sepecificar:

- dependencias con componentes de terceros
- restricción de recursos (memoria, procesamiento, ancho de banda)
- resolución de las pantallas
- sistemas que no pueden ser actualizados

## ¿Cómo se evaluarán los requisitos no funcionales?

Se debe especificar:

- parámetros objetivos y medibles

que permitan saber si el programa es seguro, usable, rápido, libre de fallos y de alto desempeño.

Idealmente, incluye **escenarios de prueba (testing)**.

## ¿A cuáles estándares nos debemos apegar?

Se debe especificar:

- estándares definidos interna o externamente sobre cómo debe ser una interfaz, un proceso o una documentación en el sistema.

## ¿Qué no sabemos todavía?

Se debe especificar:

- suposiciones y temas por resolver.

# VALIDACIÓN

Entender mal los requerimientos lleva a poner un mal producto en las manos del cliente, por lo que se deben validar antes de que sea tarde.

## Características de un requerimiento excelente

- **correcto**: provee una función acorde a una necesidad del stakeholder.
- **factible**: es posible implementarlo dentro de las capacidades y limitaciones del proyecto.
- **necesario**: ofrece el valor esperado, diferenciándolo de otros productos de software del mercado.
- **no ambiguo**: debe ser comprensible e interpretado de la misma manera por dos o más personas.
- **verificable**: se pueden definir formas de probarlo (testers).
- **consistente**: debe ser atómico, es decir, no tiene que entrar en conflicto con otros requerimientos.
- **completo**: se especficó con el detalle suficiente para saber qué se debe desarrollar.

## Validación de req. de negocio

Al inicio, se pueden validar con una **prueba de concepto** (también conocida como prototipo no funcional, maqueta o mock up), que pueden ser dibujos en papel, una presentación interactiva de diapositivas o un **andamio con ruby on rails**.

Luego, se comienza el desarrollo con un **MVP (Minimum Viable Product)**, para construir una **primera versión del producto** con la que se validará la idea del negocio.

## Validación de req. del usuario

Se recomienda colaborar con el usuario para validar el aspecto, interacciones y flujos de información del producto.

## Validación de req. no funcionales

Se validan con prototipos que se despliegan en un ambiente similar al de producción, para checar aspectos como carga, seguridad e interoperabilidad.

# REQS EN FUNCIÓN DE LA METODOLOGÍA

La estrategia para la especificación de los requerimientos depende de la metodología a usar:

- **Cascada**: involucra una documentación extensa, con diagramas de procesos, casos de uso y especificaciones funcionales.
- **Ágil**: las especificaciones se limitan al sprint en desarrollo, con **User Stories, Definition of Done, y el Manual de la Arquitectura**. (DOD es un acuerdo entre el equipo sobre el conjunto de condiciones que se deben cumplir para que un item del backlog -un incremento-se considere completo.)
- **Lean**: (entrega continua) las especificaciones se basarán en código que prueba el producto automática y frecuentemente, como **Unit Test y Scripts de Deploy**.
- **Híbrida**: el equipo decide como hacer la especificación.
