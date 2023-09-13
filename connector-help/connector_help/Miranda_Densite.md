---
uid: Connector_help_Miranda_Densite
---

# Miranda Densite

This driver is used to monitor the **Densite** Controller from **Miranda**.

## About

The driver displays the information about the different slots and the fame in a table.

### Ranges of the driver

| **Driver Range** | **Description**              | **DCF Integration** | **Cassandra Compliant** |
|------------------|------------------------------|---------------------|-------------------------|
| 2.0.1.x          | Fixed Issues, Changed Layout | Yes                 | Yes                     |

### Supported firmware versions

| **Driver Range** | **Device Firmware Version** |
|------------------|-----------------------------|
| 2.0.1.x          | 2.2.3 BUILD 0003            |

## Installation and configuration

### Creation

#### SNMP Main connection

This driver uses a Simple Network Management Protocol (SNMP) connection and requires the following input during element creation:

SNMP CONNECTION:

- **IP address/host**: The polling IP of the device.

SNMP Settings:

- **Port number**: The port of the connected device, by default *161*.
- **Get community string**: The community string used when reading values from the device
  (default value if not overridden in the driver: *public*).
- **Set community string**: The community string used when setting values on the device
  (default value if not overridden in the driver: *private*).

## Usage

Note that the client machine has to be able to access the device, as otherwise it will not be possible to open the web interface.

### General

On this page the overview table is displayed, containing information on the frame and the slots.