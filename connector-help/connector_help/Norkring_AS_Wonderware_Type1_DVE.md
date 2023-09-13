---
uid: Connector_help_Norkring_AS_Wonderware_Type1_DVE
---

# Norkring AS Wonderware Type1 DVE

This protocol will retrieve **SNMP** information from stations of type 1 of the Wonderware device.

## About

SNMP polling and traps can be retrieved when this is enabled on the device.

This driver is automatically generated by the driver [Norkring AS Wonderware](xref:Connector_help_Norkring_AS_Wonderware), range 1.0.0.x

## Installation and configuration

### Creation

#### Virtual connection

This driver uses a virtual connection and does not require any input during element creation.

## Usage

### Alarms

This page displays the following parameters polled from the device: **Station Name, Motor Drift** and **Snittspenning**. All other single parameters are only updated via traps.

To remove the alarms from the parameters linked to traps, click the button **Clear Alarms**. This will update all trap parameters to the value ***N/A.***

## DataMiner Connectivity Framework

This protocol does contain any DCF implementation.