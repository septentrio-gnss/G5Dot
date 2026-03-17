# M.2_mosaicG5


| Author|  [laekaz](https://github.com/laekaz)|
|--------------|--------------|
| Maintainer | [(Septentrio gnss github user)](githubuser@septentrio.com)|
| License|  Open Source Hardware License (CERN-OHL)|

# Table of Content

## Introduction to M.2_mosaicG5
## What is the M.2_mosaicG5?
<img src="/pictures/M.2%20main%20board.png" width="60%">
This is a compact, high precision GNSS (Global Navigation Satellite System) receiver card design for embedded computing platforms, ideal for industrial PCs such as NVIDIA Jetson. Its small size and low power consumption makes it appropriate for applications where space and efficiency are critical. 
It is based on the mosaic-G5 GNSS receiver with multiple satellite systems able to achieve 1cm precise positioning, allowing it to achieve centimetre-level positioning accuracy (up to about 1 cm). This open-source board was originally designed by ANavS GmbH.

1cm precise positioning while using multiple satellite systems simultaneously. This open source board was originally designed by ANavS GmbH.       

#### Can I buy it?
Yes, you can buy this board from ANavS

Website: https://anavs.com/products/embedded-modules/gnss-card-g5/


## What is a mosaic-G5 module?
This is Septentrio’s compact GNSS receiver with high-reliability and exceptional accurate performance. It integrates the latest generation of GNSS technology, delivering highly accurate positions with minimal power consumption. Multi-band, multi-constellation gives the receiver access to every possible signal from all available GNSS satellite constellations including the U.S. GPS, European Galileo, Russian GLONASS, as well as BeiDou and more. 

The mosaic-G5 comes with different versions. The key features and differences are listed in the table below:

| Features     | [mosaic-G5 P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | [mosaic-G5 P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [mosaic-G5 P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) |
|--------------|--------------|--------------|---------------|
| Functionality|High-precision positioning   |High-precision positioning |Positioning + Heading|
| Use case     |Robotics (e.g robotic mowers), GIS devices |UAV, Commercial mowers, Industrial Robotics, Survey, Marine navigation             
| GNSS bands   | Triple-band  | Quad-band    | Quad-band     |
| RTK support  | Yes          | Yes          | Yes           |
| Dual antenna |              |              | Yes           |
| Heading      |              |              | Yes           |



#### Other mosaic versions
 You can use other [mosaic modules](https://www.septentrio.com/en/products/gnss-receivers?f%5B0%5D=type%3A604), but you need to pay attention to the functions and pins that could be exposed, then modify the design for your own project. 

## Who is Septentrio?
<img src="/pictures/Septentrio_logo.png" width="30%">

Septentrio is a leading company that designs, manufactures and sells high precision and multi-frequency GPS/GNSS receivers for demanding applications. Septentrio products are used in different industries including automotive, marine, construction, rail, machine control, logistics, precision agriculture, geographic information systems (GIS), Unmanned aerial vehicles (UAVs), survey, mapping and scientific. Septentrio’s receivers constantly deliver high accurate and precise GNSS positioning, scalable to centimetre-level and designed to perform perfectly in challenging environments. 

Septentrio's technology offers high accuracy and reliability thanks to advanced GNSS algorithms as well as [Advanced interference Monitoring and mitigation (AIM+)](https://www.septentrio.com/en/learn-more/advanced-positioning-technology/aim-anti-jamming-protection) This protects your application against jamming (RF interference) and spoofing (malicious attacks).

For more information about Septentrio products go to [**https://www.septentrio.com/**](https://web.septentrio.com/GH-SSN-home).

## Who is ANavS GmbH
ANavS GmbH is a German company that evelops high precision navigation and positioning systems. Their technomogy combines GNSS? inertial sensor(IMU), and sensor-fusion algorithms to provide accurate lcation and orientation.

Click [here](https://anavs.com/products/embedded-modules/gnss-card-g5/) to see the board


### Why open source or is it open sourse
This board is open-source to encourage collaboration, customization, and innovation. It makes it easy for developers, hobbyists, and integrators to combine high-precision GNSS positioning with platforms like NVIDIA Jetson, experiment, create spin-off projects, and adapt it for a wide range of robotics, autonomous systems, or industrial applications.

Open source promotes shared development, letting users build on existing work and push the technology further. It also means you have access to editable design files and are free to modify, build or sell your own version.

## Disclaimer
This project is offered as-is. The main interfaces have been tested, but the design has not been fully checked or approved by the author or Septentrio. You are responsible for how you use it in your own projects. For guidance on working with Septentrio’s GNSS mosaic modules, we suggest reaching out to Septentrio directly.

Support website: https://www.septentrio.com/en/support

### Deliverables
This Open Source contains the following files for disigners, producers and integrators around Septentrio's mosaic modules.
|Files         |description   |
|--------------|--------------|
|MosaicM2G5.PrjPcb |Altium Project  |
|Files         |description   |

* Altium Project files
* Schematics PDF 
* BOM (Bill of Materials)
#### Ordering mosaic

You can order the mosaics from Digi-key, or you can contact Septentrio for directly.

| mosaic versions | Septentrio | Digikey part_number|
|-----------------|------------|--------|
| mosaic-G5 P1 |[Septentrio_G5-P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | - |
| mosaic-G5 P3 | [Septentrio_G5-P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [410501](https://www.digikey.com/en/products/detail/septentrio-inc/410501/28527327) |
| mosaic-G5 P3H |[Septentrio_G5-P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) | [410502](https://www.digikey.com/en/products/detail/septentrio-inc/410502/28527213) |
|M.2_mosaicG5|     - | [100040](https://www.digikey.com/en/products/detail/anavs-gmbh/100040/28164182) |


#### M.2 form factor
##### Why M.2?
M.2 form factor is a standard interface used to provides a compact and flexible way to add extra fanctionality without redesigning the hardware. It is usally used in Laptops for Wi-Fi or SSDs, industral PCs and embedded boards such as NVIDIA Jetson. 

NVIDIA Jetson boards are small powerful AI computers designed for applications like robotics, drones and smart sytems. They provide powerful GPU performance in a compact, energy-efficient system, making them ideal for real-time AI and embedded development.

Using the M.2 form factor for the mosaic-G5 allows developers already working in the NVIDIA ecosystem to eaisly add the GNSS receiver without redesigning their hardware.

<img src="/pictures/Jetson Orin Nano Dev Kit.png"  width="35%"><img src="/pictures/Down view NVIDIA.png" width="35%">

The M.2 Key E+A connector can fit into a Key E and Key A slots. Plus a Key A and Key E can also fit in both Key A and Key E slots.   

<img src="/pictures/M.2 interface.png" width="50%" url="https://www.delock.com/infothek/M.2_2022/images/keys-a-e_engl.jpg">

## User documentation

### Interfaces
<img src="/pictures/M2G5 Interface.png" width="40%">


### Insert in NVIDIA Orin development kit

<img src="/pictures/Jetson & mosaic.png" width="80%">

#### Pinout for M.2 Key_A+E Connector 

| Pin # |Signal            |
|-------|------------------|
| 3	    |USB D+            |
| 5	    |USB D-            |
| 2,4,72,74	|power 3.3V    |
| GND	|GND               |

The USB interface handles both satellite transmission and receiver configurations. Through this connection, the GNSS receiver can send positioning data, satellite information, and timing messages.

### Antenna

<img src="/pictures/antenna pin.png" width="50%">
<img src="/pictures/antenna.png" width="20%">

### How to get GNSS Data
* Insert the M.2_mosaicG5 to the M.2 slot.
* Connect the GNSS antenna to the antenna connector
* Configure the receiver by downloading Septentrio Rx Tools, you can get this from [here](https://www.septentrio.com/en/products/gps-gnss-receiver-software/rxtools#resources)
* Follow the installation instructions
    * This tool allows the user to monitor satellite signals, configure receiver settings, log GNSS data and verify positioning status
    * You can also download *RxTools User Manual* to get you started


Interface
-	USB (device 2.0 HS up to 480Mbps)
-	Configure PPS via the u.FL connector
Protocols
-	SBF (Septentrio Binary Format)
-	NMEA
-	RTCM v3.x (MSM included)
The official Septentrio mosaic-G5 driver can be used
Electrical
Input voltage 3.3V +/- 5%
Power consumption 0.4-0.6 W typ, 0.9W max
Antenna bias voltage 3.3V
