---
uid: Connector_help_Axon_ACP_HAS20
---

# Axon ACP HAS20

The HAS20 is a high-definition 8-channel preset-based audio shuffler with 4 local AES/EBU inputs.

The **Axon ACP HAS20** driver can be used to display and configure information related to this device.

## About

This driver can be automatically generated by the driver **Axon ACP**.

There are different possibilities available for **alarm monitoring** and **trending**.

### Version Info

| **Range** | **Key Features**             | **Based on** | **System Impact** |
|-----------|------------------------------|--------------|-------------------|
| 1.0.0.x   | Initial version \[SLC Main\] | \-           | \-                |

### Product Info

| **Range** | **Supported Firmware** |
|-----------|------------------------|
| 1.0.0.x   | 1415                   |

### System Info

| **Range** | **DCF Integration** | **Cassandra Compliant** | **Linked Components** | **Exported Components** |
|-----------|---------------------|-------------------------|-----------------------|-------------------------|
| 1.0.0.x   | Yes                 | Yes                     | \-                    | \-                      |

## Installation and configuration

### Creation

The element using this driver can be automatically created by the parent element using the **Axon ACP** driver, but it can also be a standalone element.

### Connections

#### Serial Main Connection

This driver uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination.
  - **Bus address**: The bus address of the device, being the slot number of the card.

#### Serial Broadcast Connection

This driver uses a serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host**: The polling IP or URL of the destination.
  - **Bus address**: The bus address of the device.

## Usage

This element has the following data pages:

- **General**: This page displays general information about the card: **Card Name**, **Card Description**, **SW Revision**, **HW Revision**, etc.
- **Status**
- **Settings**
- **AES**
- **Audio**
- **Embedder**
- **Embedder A**
- **Embedder B**
- **Alarm Priority**: This page displays the event messages of the card, i.e. special messages generated asynchronously on the card.

## DataMiner Connectivity Framework

The Axon ACP protocol supports the usage of DCF and can only be used on a DMA with **8.5.4** as the minimum version.

DCF can also be implemented through the DataMiner DCF user interface and through DataMiner third-party connectors (for instance a manager).

### Interfaces

#### Physical Interfaces

- **SDI Input**: A single fixed interface of type **input**.
- **AES/EBU Input 1**: A single fixed interface of type **input**.
- **AES/EBU Input 2**: A single fixed interface of type **input**.
- **AES/EBU Input 3**: A single fixed interface of type **input**.
- **AES/EBU Input 4**: A single fixed interface of type **input**.
- **SDI Output 1**: A single fixed interface of type **output**.
- **SDI Output 2**: A single fixed interface of type **output**.
- **SDI Reclocked Output**: A single fixed interface of type **output**.
- **SYNAPSE Bus Output 1**: A single fixed interface of type **output**.
- **SYNAPSE Bus Output 2**: A single fixed interface of type **output**.
- **SYNAPSE Bus Output 3**: A single fixed interface of type **output**.
- **SYNAPSE Bus Output 4**: A single fixed interface of type **output**.

#### Virtual Interfaces

- **Multiplexer 1**: A single fixed interface of type **inout**.
- **Multiplexer 2**: A single fixed interface of type **inout**.

### Connections

#### Internal Connections

When a DVE child element is created, the following connections are established:

- Between **SDI Input** and **SDI Output 1**.
- Between **SDI Input** and **SDI Output 2**.
- Between **SDI Input** and **SDI Reclocked Output**.
- Between **SDI Input** and **Multiplexer 1**.
- Between **SDI Input** and **Multiplexer 2**.
- Between **Multiplexer 1** and **SDI Output 1**.
- Between **Multiplexer 1** and **SDI Output 2**.
- Between **Multiplexer 1** and **SDI Reclocked Output**.
- Between **Multiplexer 1** and **SYNAPSE Bus Output 1**.
- Between **Multiplexer 1** and **SYNAPSE Bus Output 2**.
- Between **Multiplexer 1** and **SYNAPSE Bus Output 3**.
- Between **Multiplexer 1** and **SYNAPSE Bus Output 4**.
- Between **Multiplexer 2** and **SDI Output 1**.
- Between **Multiplexer 2** and **SDI Output 2**.
- Between **Multiplexer 2** and **SDI Reclocked Output**.
- Between **Multiplexer 2** and **SYNAPSE Bus Output 1**.
- Between **Multiplexer 2** and **SYNAPSE Bus Output 2**.
- Between **Multiplexer 2** and **SYNAPSE Bus Output 3**.
- Between **Multiplexer 2** and **SYNAPSE Bus Output 4**.

Depending on the state of **Input A1**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 1** with Connection Name suffix "**In-A1**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 1** with Connection Name suffix "**In-A1**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 1** with Connection Name suffix "**In-A1**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 1** with Connection Name suffix "**In-A1**".

Depending on the state of **Input A2**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 1** with Connection Name suffix "**In-A2**.
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 1** with Connection Name suffix "**In-A2**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 1** with Connection Name suffix "**In-A2**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 1** with Connection Name suffix "**In-A2**".

Depending on the state of **Input A3**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 1** with Connection Name suffix "**In-A3**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 1** with Connection Name suffix "**In-A3**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 1** with Connection Name suffix "**In-A3**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 1** with Connection Name suffix "**In-A3**".

Depending on the state of **Input A4**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 1** with Connection Name suffix "**In-A4**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 1** with Connection Name suffix "**In-A4**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 1** with Connection Name suffix "**In-A4**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 1** with Connection Name suffix "**In-A4**".

Depending on the state of **Input B1**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 2** with Connection Name suffix "**In-B1**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 2** with Connection Name suffix "**In-B1**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 2** with Connection Name suffix "**In-B1**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 2** with Connection Name suffix "**In-B1**".

Depending on the state of **Input B2**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 2** with Connection Name suffix "**In-B2**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 2** with Connection Name suffix "**In-B2**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 2** with Connection Name suffix "**In-B2**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 2** with Connection Name suffix "**In-B2**".

Depending on the state of **Input B3**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 2** with Connection Name suffix "**In-B3**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 2** with Connection Name suffix "**In-B3**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 2** with Connection Name suffix "**In-B3**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 2** with Connection Name suffix "**In-B3**".

Depending on the state of **Input B4**, the following connections are established:

- **AES-1**: Between **AES/EBU Input 1** and **Multiplexer 2** with Connection Name suffix "**In-B4**".
- **AES-2**: Between **AES/EBU Input 2** and **Multiplexer 2** with Connection Name suffix "**In-B4**".
- **AES-3**: Between **AES/EBU Input 3** and **Multiplexer 2** with Connection Name suffix "**In-B4**".
- **AES-4**: Between **AES/EBU Input 4** and **Multiplexer 2** with Connection Name suffix "**In-B4**".