---
description: TBD
title: TBD
keywords:
- Grove
image: TBD
slug: Grove - VOC Gas Sensor (SGP40)
last_update:
  date: 4/7/2023
  author: Stephen Lo
---


<!-- ![](https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/IMG_0012a.jpg) -->
  <p style={{textAlign: 'center'}}><img src="https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/IMG_0012a.jpg" alt="pir" width={600} height="auto" /></p>

The Grove - VOC Gas Sensor (SGP40) is an innovative environmental sensing module developed for a wide array of Volatile Organic Compound (VOC) detection applications. Based on the advanced Sensirion SGP40 sensor, it excels in transforming raw sensor signals into standardized digital signals for seamless integration into existing systems.

With its capability to perform high-quality VOC measurements in real-time, this sensor module provides a versatile solution for tracking and monitoring indoor air quality. Given the increasing awareness and need for monitoring air quality due to its direct correlation with health, the Grove - VOC Gas Sensor (SGP40) can be an essential component of systems targeted towards improving indoor air quality, personal environment monitoring, HVAC systems, industrial safety and any application where air quality assessment is pivotal.

Its compatibility with the Grove ecosystem facilitates an easy and straightforward setup process. The plug-and-play nature of Grove system allows developers to incorporate this module without needing to handle complicated wiring or intricate coding. This feature can significantly speed up development time and allows users to focus more on data interpretation and action steps based on the VOC measurements.

One of the key advantages of the Grove - VOC Gas Sensor (SGP40) is its communication protocol. The sensor module uses the I2C interface, a widely adopted protocol known for its simplicity and efficiency. This makes the data transfer process between the sensor and your main controller extremely smooth, enabling quick reaction times for applications where immediate actions based on VOC levels are crucial.

In sum, the Grove - VOC Gas Sensor (SGP40) is a compact, powerful, and easy-to-integrate module that makes the challenging task of VOC detection simpler and more accessible, opening doors for innovations and developments in environmental applications.

<p style={{textAlign: 'center'}}><a href="https://www.seeedstudio.com/-Grove-VOC-and-eCO2-Gas-Sensor-(SGP30)-p-3071.html" target="_blank"><img src="https://files.seeedstudio.com/wiki/Seeed-WiKi/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>


## Features

- Utilizes the Sensirion SGP40 sensor for reliable VOC detection.
- Easy integration into the Grove ecosystem, simplifying the wiring and coding process.
- Provides real-time VOC measurements for accurate air quality assessment.
- Communicates via I2C interface, allowing for efficient data transfer.
- Compact and modular design, perfect for embedding in various applications.

## Specification

- Operating Voltage: 3.3/5V
- Interface: I2C
- Dimensions: 20x40mm

## Applications

- Indoor air quality monitoring system: The Grove - VOC Gas Sensor can be used in buildings to monitor the air quality and ensure a healthy living or working environment.
- Personal environment monitoring device: The sensor can be used to create a portable device that allows individuals to monitor the air quality in their immediate environment.
- HVAC systems: The sensor can help regulate air quality in heating, ventilation, and air conditioning systems.
- Industrial safety: It can be used in factories and industrial sites to ensure worker safety by detecting harmful VOC levels.

## Hardware Overview

### Pin Map

<!-- ![](https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/pin.jpg) -->
  <p style={{textAlign: 'center'}}><img src="https://raw.githubusercontent.com/Longan-Labs/SGP40/main/images/pinmap.png" alt="pir" width={600} height="auto" /></p>


## Getting Started

:::note
    If this is the first time you work with Arduino, we strongly recommend you to see [Getting Started with Arduino](https://wiki.seeedstudio.com/Getting_Started_with_Arduino/) before the start.
:::

### Play With Arduino

#### Hardware

**Materials required**

| Seeeduino V4.2 | Base Shield| Grove - VOC Gas Sensor (SGP40) |
|--------------|-------------|-----------------|
|<p><img src="https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_1.jpg" alt="pir" width={600} height="auto" /></p>|<p><img src="https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_4.jpg" alt="pir" width={600} height="auto" /></p>|<p><img src="https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/thumbnail.jpg" alt="pir" width={500} height="auto" /></p>|
|<a href="https://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/-Grove-VOC-and-eCO2-Gas-Sensor-(SGP30)-p-3071.html" target="_blank">Get One Now</a>|

:::note
    **1** Please plug the USB cable gently, otherwise you may damage the port. Please use the USB cable with 4 wires inside, the 2 wires cable can't transfer data. If you are not sure about the wire you have, you can click [here](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) to buy
    
    **2** Each Grove module comes with a Grove cable when you buy. In case you lose the Grove cable, you can click [here](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) to buy.
:::

- **Step 1.** Connect Grove - VOC Gas Sensor (SGP40) to **I2C** port  of Grove-Base Shield.

- **Step 2.** Plug Grove - Base Shield into Seeeduino.

- **Step 3.** Connect Seeeduino to PC via a USB cable.


<!-- ![](https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/3.jpg) -->
  <p style={{textAlign: 'center'}}><img src="https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/3.jpg" alt="pir" width={600} height="auto" /></p>


:::note
	If we don't have Grove Base Shield, We also can directly connect Grove - Smart Air Quality Sensor (SGP41) to Seeeduino as below.
:::

| Seeeduino     | Grove - VOC Gas Sensor (SGP40) |
|---------------|-------------------------|
| 5V            | Red                     |
| GND           | Black                   |
| SDA           | White                   |
| SCL           | Yellow                  |

#### Software

- **Step 1.** Download the [D7S library](https://github.com/Longan-Labs/arduino-i2c-sgp41) from Github.

- **Step 2.** Refer to [How to install library](https://wiki.seeedstudio.com/How_to_install_Arduino_Library) to install library for Arduino.

- **Step 3.** After downloading and installing the library correctly, you can find an example program named exampleUsage.ino in the examples folder. This program is designed for the SGP41 sensor.

- **Step 4.** Upload the demo. If you do not know how to upload the code, please check [How to upload code](https://wiki.seeedstudio.com/Upload_Code/).

- **Step 5.** Open the **Serial Monitor** of Arduino IDE by click **Tool-> Serial Monitor**. Or tap the ++ctrl+shift+m++ key at the same time. if every thing goes well, you will get the result.

## Schematic Online Viewer

<div className="altium-ecad-viewer" data-project-src="https://github.com/Longan-Labs/SGP41_RESOURCES/raw/main/AIR_QUALITY_SENSOR(SGP41).zip" style={{borderRadius: '0px 0px 4px 4px', height: 500, borderStyle: 'solid', borderWidth: 1, borderColor: 'rgb(241, 241, 241)', overflow: 'hidden', maxWidth: 1280, maxHeight: 700, boxSizing: 'border-box'}}>
</div>

## Resources

- **[Zip]** [Grove - Smart Air Quality Sensor (SGP41)](https://github.com/Longan-Labs/SGP41_RESOURCES/raw/main/AIR_QUALITY_SENSOR(SGP41).zip)
- **[PDF]** [SGP41 Datasheet](https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/res/Sensirion_Gas_Sensors_SGP30_Datasheet_EN.pdf)

## Tech Support
If you have any technical issue.  submit the issue into our [forum](https://forum.seeedstudio.com/).