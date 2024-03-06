# ¿Cómo ejecutar la integración? Integración de programación y basada en aplicaciones

> [!NOTE]
> Como se menciona en el índice de esta serie de notas, debido a que OIC es de paga, nos apoyaremos de ahora en adelante de videos de YouTube para poder ver como funciona y aprender más al respecto antes de que decidas tomar los 30 días gratis que ofrece Oracle.

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=CkN0EqqxdQ0&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=4)

## Resumen

Este video explica los conceptos básicos de Oracle Integration Cloud Services (OIC), el video se centra en el componente de integración de OIC, que ofrece dos tipos de integraciones: app-driven y schedule-driven. El video muestra cómo crear, configurar, activar, ejecutar y probar diferentes integraciones, así como cómo resolver errores y bloqueos. El video también introduce algunos componentes de OIC, como el logger, el looper, el connection y el agent.

## Estados en Oracle Integration Cloud

Los estados en Oracle Integration Cloud (OIC) representan las condiciones en las que se encuentra una integración en su ciclo de vida. Cada estado indica el progreso y la situación actual de la integración, lo que permite a los usuarios comprender y gestionar eficazmente el proceso de desarrollo e implementación. A continuación, se detallan los principales estados que pueden experimentar las integraciones en OIC:

1. **Borrador**: Cuando una integración se crea por primera vez, se encuentra en estado de borrador. En este estado, la integración está en proceso de diseño y configuración, y aún no está lista para ser activada o ejecutada.

2. **Configurado**: Una vez que se completa la configuración inicial de la integración y se definen todos los componentes necesarios, la integración pasa al estado configurado. En este estado, la integración está lista para ser activada y probada.

3. **Activado**: Cuando se activa una integración, se cambia al estado activado. En este estado, la integración está en funcionamiento y lista para procesar eventos o ejecutarse según lo programado.

4. **Bloqueado**: Si se producen errores críticos o se encuentran problemas durante la ejecución de una integración, puede quedar en estado bloqueado. En este estado, la integración está detenida y requiere intervención para solucionar los problemas antes de poder reactivarse.

5. **Con Errores**: Si se producen errores no críticos durante la ejecución de una integración, puede quedar en estado con errores. En este estado, la integración sigue activa, pero es posible que no funcione correctamente debido a problemas menores que deben corregirse.

## Pruebas en Oracle Integration Cloud

Las pruebas en Oracle Integration Cloud son acciones realizadas para verificar el funcionamiento y el rendimiento de una integración antes de su implementación en un entorno de producción. Estas pruebas son fundamentales para garantizar que la integración cumpla con los requisitos funcionales y de rendimiento esperados. A continuación, se describen los principales aspectos relacionados con las pruebas en OIC:

- **Ejecución de Pruebas**: Las pruebas en OIC se pueden ejecutar desde el menú de integraciones, seleccionando la opción de prueba o envío. Esto permite a los usuarios simular la ejecución de la integración y verificar su comportamiento sin afectar los datos reales o el entorno de producción.

- **Generación de Registros y Trazas**: Durante la ejecución de las pruebas, OIC genera registros y trazas que proporcionan información detallada sobre el proceso de integración. Estos registros y trazas pueden ser consultados por los usuarios para analizar los resultados de las pruebas y detectar posibles problemas o errores.

- **Análisis de Resultados**: Después de ejecutar las pruebas, los usuarios pueden analizar los registros y trazas generados para evaluar el funcionamiento y el rendimiento de la integración. Esto les permite identificar áreas de mejora y realizar ajustes según sea necesario para optimizar el rendimiento y la eficiencia de la integración.

Las pruebas en Oracle Integration Cloud son una parte esencial del proceso de desarrollo e implementación de integraciones, ya que garantizan la calidad y la fiabilidad de las soluciones integradas. Al realizar pruebas exhaustivas y analizar los resultados de manera efectiva, los usuarios pueden asegurar que sus integraciones funcionen correctamente y cumplan con los requisitos del negocio.

## Profundizando en...

### [Componente Logger](./0_Definiciones.md/#componente-logger)

---

# ¿Cómo crear una conexión en OIC? ¿Cuándo utilizar el Agente en Conexión?

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=MUQxQAXmiC4&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=5)

## Resumen

El video muestra cómo crear y configurar una conexión con una base de datos Oracle usando el adaptador correspondiente, y cómo definir el rol de la conexión como disparador, invocación o ambos. El video también describe el propósito del agente, que es facilitar la conectividad con las aplicaciones locales.

## Cómo Crear y Configurar una Conexión

En Oracle Integration Cloud (OIC), la creación y configuración de una conexión es un paso fundamental para establecer la comunicación con las aplicaciones externas. Aquí se explica el proceso básico para crear y configurar una conexión en OIC:

1. **Seleccionar el Adaptador Adecuado:** El primer paso es seleccionar el adaptador adecuado para la aplicación que se quiere conectar. OIC ofrece una amplia variedad de adaptadores que admiten diferentes tipos de aplicaciones y sistemas, como bases de datos, servicios web, aplicaciones SaaS, entre otros.

2. **Introducir los Detalles de la Conexión:** Una vez seleccionado el adaptador, se deben introducir los detalles básicos de la conexión, como el nombre, el identificador y el rol de la conexión. Estos detalles ayudan a identificar y gestionar la conexión dentro de OIC.

3. **Configurar los Detalles Específicos del Adaptador:** Después de establecer los detalles básicos, se deben proporcionar los detalles de configuración específicos del adaptador. Esto puede incluir información como el host, el puerto, el nombre de usuario, la contraseña y cualquier otro parámetro necesario para establecer la conexión con la aplicación externa.

4. **Definir el Rol de la Conexión:** Un aspecto importante en la configuración de una conexión en OIC es definir su rol. El rol de la conexión determina dónde se puede utilizar en la integración. Puede ser:
   - **Rol de Disparador:** La conexión solo se puede utilizar al inicio de la integración, por ejemplo, para desencadenar el inicio del flujo de trabajo.
   - **Rol de Invocación:** La conexión solo se puede utilizar en el medio o al final de la integración, para invocar acciones específicas en la aplicación externa.
   - **Rol de Disparador e Invocación:** La conexión se puede utilizar en cualquier parte de la integración, ya sea al inicio, en el medio o al final del proceso.

Al seguir estos pasos, los usuarios pueden crear y configurar conexiones en Oracle Integration Cloud de manera efectiva, lo que les permite establecer la comunicación con aplicaciones externas y construir flujos de integración robustos y eficientes.

## Profundizando en...

### [Componente Oracle Database](./0_Definiciones.md/#componente-oracle-database)

---

# Adaptador, paquete, bibliotecas, agente y lookup en OIC

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=uYTJIYu6jMM&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=6)

## Resumen

Este video explica los componentes básicos de OIC, como lookups, paquetes, agentes, adaptadores y bibliotecas. El video muestra cómo crear y usar estos componentes para integrar aplicaciones en la nube y en las instalaciones.

---

# Descripción general de la página de integración de Oracle | Elementos de la integración de Oracle | ¿Cómo manejar la excepción?

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=YZoXgnTHkbE&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=7)

## Resumen

El video proporciona una visión general detallada de la página de integración de Oracle, explicando los elementos clave y cómo manejar excepciones. Se describe cómo crear y editar integraciones, destacando la importancia de los elementos como ‘assign’, ‘stage file’, y ‘mapper’, y ofrece consejos para manejar archivos y excepciones dentro de OIC.

## 1. Assign

El componente "Assign" en Oracle Integration Cloud (OIC) permite asignar valores a variables o atributos durante la ejecución de una integración. Es especialmente útil para realizar transformaciones simples de datos o para establecer condiciones basadas en reglas específicas. Con "Assign", los usuarios pueden manipular y modificar datos en tiempo real dentro de los flujos de integración, lo que les permite adaptar y ajustar dinámicamente el comportamiento de la integración según las necesidades del negocio.

## 2. Data Stitch

"Data Stitch" es otro componente esencial en OIC que permite realizar transformaciones complejas de datos durante la ejecución de integraciones. A diferencia de "Assign", que se utiliza para tareas simples de asignación de valores, "Data Stitch" proporciona capacidades avanzadas de transformación de datos, como el mapeo de campos, la conversión de tipos de datos, la concatenación de cadenas y la validación de datos. Con "Data Stitch", los usuarios pueden llevar a cabo transformaciones sofisticadas para garantizar la coherencia y la calidad de los datos en los flujos de integración.

## 3. Stage File

"Stage File" es un componente utilizado en OIC para manejar archivos durante el proceso de integración. Permite la carga, descarga y manipulación de archivos en diferentes formatos, como archivos CSV, XML, JSON, entre otros. Con "Stage File", los usuarios pueden realizar operaciones de lectura y escritura en archivos, así como procesar y transformar datos almacenados en archivos dentro de los flujos de integración.

## 4. Mapper

El componente "Mapper" en OIC facilita el mapeo de datos entre diferentes formatos y esquemas durante la ejecución de una integración. Permite a los usuarios definir reglas de mapeo visualmente para asignar campos y estructuras de datos entre sistemas, aplicaciones y servicios conectados. Con "Mapper", los usuarios pueden crear transformaciones complejas de datos mediante una interfaz intuitiva de arrastrar y soltar, lo que simplifica el proceso de mapeo y reduce la necesidad de escribir código personalizado.

## 5. Global Fault

"Global Fault" es un componente utilizado para manejar excepciones y errores durante la ejecución de integraciones en OIC. Permite definir acciones y estrategias para manejar situaciones de error, como reintentos automáticos, notificaciones de errores, registro de eventos y acciones de recuperación. Con "Global Fault", los usuarios pueden implementar prácticas de manejo de excepciones robustas para garantizar la confiabilidad y la disponibilidad de las integraciones, incluso en situaciones adversas o inesperadas.

## Profundizando en...

### [Componente Notification](./0_Definiciones.md/#componente-notification)

### [Componente Mapper](./0_Definiciones.md/#componente-mapper)

### [Componente Global fault](./0_Definiciones.md/#componente-global-fault)

### [Componente Data Stitch](./0_Definiciones.md/#componente-data-stitch)

---

# Cree su primera integración de orquestación de horarios en OIC | Crear integración en OIC

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=kfA_osmbNf8&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=8)

---

# Cree su primera integración de orquestación basada en aplicaciones | Crear integración en OIC

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=0GG7vNVLSJs&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=9)

## Resumen

Este video proporciona una guía paso a paso para crear una integración de orquestación programada en Oracle Integration Cloud (OIC), abordando problemas comunes y demostrando cómo iniciar la integración con un adaptador REST.

## Profundizando en...

### [Adaptador REST](./0_Definiciones.md/#adaptador-rest)

---

# Crear integración con parámetro | Cómo crear una integración impulsada por aplicaciones con parámetros

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=T-N58b5y6-s&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=10)

## Resumen

Este video muestra cómo crear una integración de orquestación impulsada por aplicaciones en Oracle Integration Cloud (OIC), utilizando un parámetro ingresado por el usuario durante la ejecución para personalizar el proceso.

---

# Crear integración con request payload | Cómo crear una integración impulsada por aplicaciones con solicitud

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=GpP47oaBxzM&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=11)

## Resumen

Este video enseña cómo crear una integración de aplicación con un payload, utilizando un ejemplo práctico para configurar una solicitud de usuario y procesarla en la integración.

---

# Crear integración en oic para obtener solicitud y devolver la respuesta | Solicitud y Respuesta en OIC

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=sjJGPMb-pIA&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=12)

---

# Cree una integración para obtener dos números como solicitud y devolver la suma de ambos num en respuesta

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=oU_vAVLl_yI&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=13)

## Resumen

Este video es sobre cómo crear una integración básica en Oracle Integration Cloud (OIC) que toma dos valores numéricos como entrada y devuelve la suma de esos valores como salida. El video muestra los pasos para configurar un adaptador REST, crear una variable para almacenar el resultado, asignar los valores de entrada y salida, y probar la integración.

## Profundizando en...

### [Componente Assing](./0_Definiciones.md/#componente-assign)

---

# Assing en Oracle Integration: cómo crear una variable en oic | Crear variable local en oic

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=quC4bMjIoBQ&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=14)

## Resumen

Este video explica cómo crear y usar variables en una integración usando la herramienta de asignación. El video muestra cómo crear un punto final que recibe dos números y una operación como entrada y devuelve la suma o resta de los números como salida. El video también enseña cómo convertir cadenas en números usando la función número y cómo mapear las variables con el mensaje de respuesta.

---

# Data Stitch en Oracle Integration: cómo crear una variable global en oic | Variable global en oic

## [VIDEO DE YOUTUBE](https://www.youtube.com/watch?v=TrGxxdaAy80&list=PL3X62LScvI_IQ-5ji5SQGx3Zc0IhZB3jZ&index=15)

## Resumen

Este video explica cómo crear y asignar variables globales y locales en Oracle Integration Cloud (OIC) usando las actividades de asignación y costura de datos. El video muestra un ejemplo de una integración que recibe dos números como parámetros de entrada, los almacena en variables globales, los suma y los devuelve como resultado en una variable local.

## Profundizando en...

### [Variables Globales](./0_Definiciones.md/#variables-globales)

---

# 