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

## Otros conceptos

### [Componente Logger](./0_Definiciones.md/#componente-logger)