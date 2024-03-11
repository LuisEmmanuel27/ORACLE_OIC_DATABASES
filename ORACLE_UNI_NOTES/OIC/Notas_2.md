# Become An Application Integration Professional (2023) - Parte 2

## Application Integration on Oracle Cloud

### Fundamentals of Creating Integrations - Integration Design Fundamentals

#### What Is an OIC Integration?

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_1.png" alt="oic" width="700">
</div>

#### OIC Integration Styles

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_2.png" alt="oic" width="700">
</div>

#### Integration Style Patterns Described

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_3.png" alt="oic" width="700">
</div>

| Patrón | Descripción |
| --- | --- |
| Enrutamiento Básico | Este estilo de diseño de lienzo de integración ha sido descontinuado. |
| Publicar en OIC | Crea una integración en la que defines un adaptador de disparador para publicar mensajes a OIC a través de una interfaz o evento asincrónico. Esta integración está desacoplada de todos los suscriptores, ya que todas las integraciones participantes pueden activarse y desactivarse independientemente entre sí. |
| Suscribirse a OIC | Crea una integración en la que te suscribes a una integración publicadora existente. Luego defines un adaptador invocable para procesar mensajes que han sido publicados a OIC por esa integración. |
| Orquestación Impulsada por Aplicaciones | Crea una integración que utiliza capacidades básicas del Administrador de Procesos BPEL. Puedes incluir expresiones Switch y construcciones loop, así como estrategias para el manejo de fallas. Los cuatro patrones de intercambio de mensajes son compatibles. |
| Orquestación Programada | Crea una integración con las mismas opciones de actividad de orquestación que el estilo impulsado por aplicaciones. La diferencia es un horario, o se utiliza una solicitud bajo demanda para activar la integración en lugar del patrón basado en interfaces para el intercambio |
| Transferencia de Archivos | Este estilo es actualmente idéntico al estilo Orquestacion Programada |

#### App Driven Orchestration Style

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_4.png" alt="oic" width="700">
</div>

#### Scheduled Orchestration Style

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_5.png" alt="oic" width="700">
</div>

#### Integration Development and Management Workflow

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_6.png" alt="oic" width="700">
</div>

#### Basic Integration Development Workflow Steps

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_7.png" alt="oic" width="700">
</div>

#### 1. Basic Integration Development Workflow Steps

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_8.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_8_2.png" alt="oic" width="700">
</div>

#### 2. Creating Integration

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_9.png" alt="oic" width="700">
</div>

#### 3. Add and Configure the Trigger (Source) Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_10.png" alt="oic" width="700">
</div>

#### 4. Add and Configure an Invoke (Target) Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_11.png" alt="oic" width="700">
</div>

#### 5. & 6. Request and Response Data Mapping

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_12.png" alt="oic" width="700">
</div>

#### 7. Assigning Business Identifiers

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_13.png" alt="oic" width="700">
</div>

#### 8. Activation Options (Review)

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_14.png" alt="oic" width="700">
</div>

#### Testing a SOAP Interface Trigger Connection

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15_2.png" alt="oic" width="700">
</div>

<div align="center">
    <img src="../../IMG/OIC/ORA_UNI/PT_2/pic_15_3.png" alt="oic" width="700">
</div>

### Creating OIC Adapter Connections - Defining OIC Adapter Connections

- **Para la Pic 23**: [Documentacion de adaptadores OIC Gen 3](https://docs.oracle.com/en/cloud/paas/application-integration/find-adapters.html), [Documentacion de adaptadores OIC Gen 2](https://docs.oracle.com/en/cloud/paas/integration-cloud/find-adapters.html)
- Hasta pic 28

### Creating OIC Adapter Connections - Exploring Additional Adapter Connections

- Hasta pic 36

### Creating OIC Adapter Connections - Using the On-Premises Connectivity Agent
