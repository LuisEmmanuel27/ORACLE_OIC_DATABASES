# Aprendiendo Oracle OIC y Oracle DataBase

<div align="center">
    <img src="./IMG/portada.png" alt="oic" width="400">
</div>

# Nota importante

<div align="center">
    <img src="./IMG/advertencia.png" alt="oic" width="100">
</div>

Oracle OIC es un servicio de paga dentro de la nube de Oracle, cuando creamos una cuenta nueva tenemos acceso a casi todas sus funcionalidades y herramientas por `un año`, pero en el caso de `OIC` este tiempo es considerablemente menor, solo se nos ofrecen **_`30 días de prueba`_**. Así que recomiendo que si se quieren hacer pruebas y practicar con la herramienta se debe tomar muy en cuenta esta restricción.

Por lo mismo muchas partes prácticas seran tomadas directamente de videos de youtube que ejemplifiquen/complementen el tema visto.

# Índice

## Oracle OIC: Gen 2

### 1. <a href="./OIC_GEN_2/1_Introduccion.md">Introducción</a>

### 2. <a href="./OIC_GEN_2/2_Componentes.md">Componentes en OIC</a>

- <a href="./OIC_GEN_2/2_Componentes.md/#adaptadores-en-oic">Adaptadores</a>
- <a href="./OIC_GEN_2/2_Componentes.md/#agentes-en-oic">Agentes</a>
- <a href="./OIC_GEN_2/2_Componentes.md/#conexiones-en-oic">Conexiones</a>
- <a href="./OIC_GEN_2/2_Componentes.md/#lookups-en-oic">Lookups</a>
- <a href="./OIC_GEN_2/2_Componentes.md/#bibliotecas-paquetes-y-javascript-en-oic">Bibliotecas y Paquetes</a>
- <a href="./OIC_GEN_2/2_Componentes.md/#integraciones-en-oracle-integration-cloud-oic">Integraciones</a>

### 3. <a href="./OIC_GEN_2/3_Patrones_Int.md">Patrones de Integración en OIC</a>

- <a href="./OIC_GEN_2/3_Patrones_Int.md/#orquestación-impulsada-por-aplicaciones">Orquestación Impulsada por Aplicaciones</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#orquestación-programada">Orquestación Programada</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#transferencia-de-archivos">Transferencia de Archivos</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#enrutamiento-básico">Enrutamiento Básico</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#publicar-en-oracle-integration-cloud">Publicar en Oracle Integration Cloud</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#suscribirse-a-oracle-integration-cloud">Suscribirse a Oracle Integration Cloud</a>
- <a href="./OIC_GEN_2/3_Patrones_Int.md/#demo-creación-de-una-integración">Demo 📺: creación de una integración</a>

### 4. <a href="./OIC_GEN_2/4_Ejemplos_Practicos.md">Ejemplos Practicos</a>

- [¿Cómo ejecutar la integración? Integración de programación y basada en aplicaciones](./OIC_GEN_2/4_Ejemplos_Practicos.md/#¿cómo-ejecutar-la-integración-integración-de-programación-y-basada-en-aplicaciones)
- [¿Cómo crear una conexión en OIC? ¿Cuándo utilizar el Agente en Conexión?](./OIC_GEN_2/4_Ejemplos_Practicos.md/#¿cómo-crear-una-conexión-en-oic-¿cuándo-utilizar-el-agente-en-conexión)
- [Adaptador, paquete, bibliotecas, agente y lookup en OIC](./OIC_GEN_2/4_Ejemplos_Practicos.md/#adaptador-paquete-bibliotecas-agente-y-lookup-en-oic)
- [Descripción general de la página de integración de Oracle | Elementos de la integración de Oracle | ¿Cómo manejar la excepción?](./OIC_GEN_2/4_Ejemplos_Practicos.md/#descripción-general-de-la-página-de-integración-de-oracle--elementos-de-la-integración-de-oracle--¿cómo-manejar-la-excepción)
- [Cree su primera integración de orquestación de horarios en OIC | Crear integración en OIC](./OIC_GEN_2/4_Ejemplos_Practicos.md/#cree-su-primera-integración-de-orquestación-de-horarios-en-oic--crear-integración-en-oic)
- [Cree su primera integración de orquestación basada en aplicaciones | Crear integración en OIC](./OIC_GEN_2/4_Ejemplos_Practicos.md/#cree-su-primera-integración-de-orquestación-basada-en-aplicaciones--crear-integración-en-oic)
- [Crear integración con parámetro | Cómo crear una integración impulsada por aplicaciones con parámetros](./OIC_GEN_2/4_Ejemplos_Practicos.md/#crear-integración-con-parámetro--cómo-crear-una-integración-impulsada-por-aplicaciones-con-parámetros)
- [Crear integración con request payload | Cómo crear una integración impulsada por aplicaciones con solicitud](./OIC_GEN_2/4_Ejemplos_Practicos.md/#crear-integración-con-request-payload--cómo-crear-una-integración-impulsada-por-aplicaciones-con-solicitud)
- [Crear integración en oic para obtener solicitud y devolver la respuesta | Solicitud y Respuesta en OIC](./OIC_GEN_2/4_Ejemplos_Practicos.md/#crear-integración-en-oic-para-obtener-solicitud-y-devolver-la-respuesta--solicitud-y-respuesta-en-oic)
- [Cree una integración para obtener dos números como solicitud y devolver la suma de ambos num en respuesta](./OIC_GEN_2/4_Ejemplos_Practicos.md/#cree-una-integración-para-obtener-dos-números-como-solicitud-y-devolver-la-suma-de-ambos-num-en-respuesta)
- [Assing en Oracle Integration: cómo crear una variable en oic | Crear variable local en oic](./OIC_GEN_2/4_Ejemplos_Practicos.md/#assing-en-oracle-integration-cómo-crear-una-variable-en-oic--crear-variable-local-en-oic)
- [Data Stitch en Oracle Integration: cómo crear una variable global en oic | Variable global en oic](./OIC_GEN_2/4_Ejemplos_Practicos.md/#data-stitch-en-oracle-integration-cómo-crear-una-variable-global-en-oic--variable-global-en-oic)

### <a href="./OIC_GEN_2/0_Definiciones.md">Glosario de Componentes</a>

---

## Oracle OIC: Gen 3

---

## Oracle DataBase

### Become An Oracle Cloud Data Management Foundations Associate (2023)

#### 1. <a href="./ORACLE DB/1_COUD_DATA_MANAGEMENT_FOUNDATIONS/1_Notas_1.md">Oracle´s Data Managment Strategy</a>

#### 2. <a href="./ORACLE DB/1_COUD_DATA_MANAGEMENT_FOUNDATIONS/2_Notas_2.md">Oracle Database Offerings</a>

---

## SQL