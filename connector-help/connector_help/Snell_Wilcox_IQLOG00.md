---
uid: Connector_help_Snell_Wilcox_IQLOG00
---

# Snell Wilcox IQLOG00

The **Snell Wilcox IQLOG00** driver monitors and configures the IQLOG00 logo inserter device.

## About

The driver polls all parameters once after startup, and from then on depends on event messages generated by the device when a parameter changes. The "Force Poll" button on the General page can be used to manually trigger polling again.

### Ranges of the driver

| **Driver Range**     | **Description** | **DCF Integration** | **Cassandra Compliant** |
|----------------------|-----------------|---------------------|-------------------------|
| 1.0.0.x \[SLC Main\] | Initial version | No                  | Yes                     |

### Supported firmware versions

| **Driver Range** | **Device Firmware Version** |
|------------------|-----------------------------|
| 1.0.0.x          | 5.2.2                       |

## Installation and configuration

### Creation

#### Serial Main Connection

This driver uses a single smart-serial connection and requires the following input during element creation:

SERIAL CONNECTION:

- Interface connection:

  - **IP address/host:** The polling IP of the device.
  - **IP port:** The IP port of the device, by default *2050*.
  - **Bus Address:** The bus of the card on the chassis. The default, *UU.PP (Hex)*, shows the expected structure of the address, where UU is the chassis ID, and the PP is the card position, both in Hex.

## Usage

### General

This page contains general information on the device, such as the various **versions**, the **Serial Number**, the **Build Number** and logo information such as free logo space, deleted logo space, and defragment information.

With the **Simulated RollCall response** parameter, you can set a custom response that will be handled by the driver as if it was received by the device. For more information, check the tooltip of the parameter.

The page also contains the following buttons:

- **Restart**: Restarts the device.
- **Defragment Logos**: Defragments the logos.
- **Factory Default**: Sets all settings back to factory default.
- **Connection info**: Opens the **Connection Info** subpage, which includes information about the **session**, the **force poll** button, and the **Simulated RollCall Response** control.

### Video Input

On this page, you can enable various settings related to each different video input, including the different video standards (**1080/25i**, **720/50p**, etc.). It also includes the **CRC** and **ANC** **errors**, as well as the following buttons:

- **All Valid**: Sets all video standards to enabled.
- **All Invalid**: Sets all video standards to disabled.
- **Reset Errors:** Sets the **ANC** and **CRC** errors back to 0.

### Logo Control

This page contains the different settings for each logo, including the fade-in time, fade-out time, last memory, and logo name. For each logo, the following action buttons are available:

- **Fade in**
- **Fade out**
- **Fade stop**
- **Cut in**
- **Cut out**

### Logo Channel Setup

This page contains various controls such as Select Logo, Filter Logos, and Logo Filter. It also includes the following buttons:

- **Select Directory**
- **Load Chan 1 (16:9)**
- **Load Chan 2 (16:9)**
- **Load Chan 3 (16:9)**

### Logo Edit

This page contains the logo edit enables, as well as a page button for each logo (**Logo 1** to **Logo 4**). Each page button opens a subpage with information and controls for each logo. These include the logo **horizontal**/**vertical** **sizes**, the **comments**, the **file dates**, and various **pixel** controls.

### Logo Memory

This page contains various logo memory controls, such as **Recall Logo Memory**, **Select Memory**, **Save Memory Name**, and **Logo Channel** memory parameters. It also includes the **Save Memory** button, which saves the current logo memory.

### GPIO

This page contains **GPI/O** controls, such as **GPI/O mode**, **Input/Output** Select, and **Invert GPI/O** for both **GPI/O 1** and **GPI/O 2.**

### RollTrack

This page contains various RollTrack controls, such as **Disable all**, **Index**, **Source**, **Address**, **Command**, **Status**, and **Sending** status.

### User Memory

This page contains various user memory controls, such as **Recall Memory**, **Select Memory**, **Change Name**, **Last User Memory**, and the **Save Memory** button, which saves the current user memory.

### Video Input Logging

This page displays **Video Input** information, as well as controls to enable or disable the logging of this information.

### Audio Input State Logging

This page displays **Audio State** information, as well as controls to enable or disable the logging of this information.

### Audio Input Type Logging

This page displays **Audio Type** information, as well as controls to enable or disable the logging of this information.

### Output Logging

This page displays **Output** information, as well as controls to enable or disable the logging of this information.

### Misc Logging

This page displays **Miscellaneous/System** information, as well as controls to enable or disable the logging of this information.

### Logo Logging

This page displays **Logo** information, as well as controls to enable or disable the logging of this information.

### Log Server

This page contains two log options: **Log to** and **Log Server Name**.

### Diagnostics

This page contains a **Select Test** drop-down list, which allows you to run various tests. It also includes the error count for each test, the progress, the loop count, the test ID, the Last Error, as well as a button to stop tests.

### Web Interface

This page provides access to the web interface of the device. Note that the client machine has to be able to access the device, as otherwise it will not be possible to open the web interface.