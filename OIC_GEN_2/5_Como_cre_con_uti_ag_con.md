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

## Otros Conceptos

### [Componente Oracle Database](./0_Definiciones.md/#componente-oracle-database)