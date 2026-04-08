# M.2_mosaicG5


| Author|  [laekaz](https://github.com/laekaz)|
|--------------|--------------|
| Maintainer | [(Septentrio GNSS github user)](githubuser@septentrio.com)|
| License|  Open-Source Hardware License (CERN-OHL)|

# Table of Contents

* [Introduction to M.2_mosaicG5](#introduction-to-m2_mosaicg5)
  * [What is the M.2_mosaicG5?](#what-is-the-m2_mosaicg5)
    * [Availability](#availability)
* [What is a mosaic-G5 module?](#what-is-a-mosaic-g5-module)
  * [Other mosaic-G5 versions](#other-mosaic-g5-versions)
* [Who is Septentrio?](#who-is-septentrio)
* [Who is ANavS GmbH](#who-is-anavs-gmbh)
* [Why open-source](#why-open-source)
* [Disclaimer](#disclaimer)
* [Deliverables](#deliverables)
  * [Ordering mosaic](#ordering-mosaic)
* [M.2 form factor](#m2-form-factor)
  * [Why M.2?](#why-m2)
* [User documentation](#user-documentation)
  * [Interfaces](#interfaces)
  * [Insert in NVIDIA Orin development kit](#insert-in-nvidia-orin-development-kit)
  * [Pinout for M.2 Key_A+E Connector](#pinout-for-m2-key_ae-connector)
  * [Pinout for mosaic-G5 module](#pinout-for-mosaic-g5-module)
  * [Antenna](#antenna)
  * [How to get GNSS Data](#how-to-get-gnss-data)
* [Interface, Protocols & Electrical Specifications](#interface-protocols--electrical-specifications)  

# Introduction to M.2_mosaicG5
## What is the M.2_mosaicG5?
<img src="/pictures/M.2 main board - Copy.png" width="60%">
This is a compact, high precision GNSS (Global Navigation Satellite System) receiver card design for embedded computing platforms, ideal for industrial PCs such as NVIDIA Jetson. Its small size and low power consumption makes it appropriate for applications where space and efficiency are critical. 

The design is based on the mosaic-G5 GNSS receiver, which supports multiple satellite systems and enables centimetre-level positioning accuracy. This open-source board was originally designed by ANavS GmbH.

#### Can I buy it?
Yes, the board is available for purchase from ANavS

Website: https://anavs.com/products/embedded-modules/gnss-card-g5/


## What is a mosaic-G5 module?
The mosaic-G5 is a compact GNSS receiver from Septentrio, engineered for high reliability and precise positioning. It integrates the latest multi-band, multi-constellation GNSS technology, providing accurate positions while minimizing power consumption. The receiver can access signals from all major satellite constellations, including GPS, Galileo, GLONASS, and BeiDou.

Different versions of the mosaic-G5 are available to suit various applications, as summarized below:

| Features     | [mosaic-G5 P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | [mosaic-G5 P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [mosaic-G5 P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) |
|--------------|--------------|--------------|---------------|
| Functionality|High-precision positioning   |High-precision positioning |Positioning + Heading|
| Use case     |Robotics (e.g robotic mowers), GIS devices |UAV, Commercial mowers, Industrial Robotics, Survey, Marine navigation             
| GNSS bands   | Triple-band  | Quad-band    | Quad-band     |
| RTK support  | Yes          | Yes          | Yes           |
| Dual antenna |              |              | Yes           |
| Heading      |              |              | Yes           |



#### Other mosaic-G5 versions
 You can use other [mosaic modules](https://www.septentrio.com/en/products/gnss-receivers?f%5B0%5D=type%3A604), but you need to pay attention to the functions and pins that could be exposed, then modify the design for your own project. 

## Who is Septentrio?
<img src="/pictures/Screenshot 2026-03-13 160257.png" width="30%">

Septentrio is a leading company that designs, manufactures and sells high precision and multi-frequency GPS/GNSS receivers for demanding applications. Septentrio products are used in different industries including automotive, marine, construction, rail, machine control, logistics, precision agriculture, geographic information systems (GIS), Unmanned aerial vehicles (UAVs), survey, mapping and scientific. Septentrio’s receivers constantly deliver highly accurate and precise GNSS positioning, scalable to centimetre-level and designed to perform perfectly in challenging environments. 

Septentrio's technology offers high accuracy and reliability thanks to advanced GNSS algorithms as well as [Advanced interference Monitoring and mitigation (AIM+)](https://www.septentrio.com/en/learn-more/advanced-positioning-technology/aim-anti-jamming-protection) This protects your application against jamming (RF interference) and spoofing (malicious attacks).

For more information about Septentrio products go to [**https://www.septentrio.com/**](https://web.septentrio.com/GH-SSN-home).

### Who is ANavS GmbH
ANavS GmbH is a German company that develops high precision navigation and positioning systems. Their technology combines GNSS, inertial sensors (IMUs), and sensor fusion algorithms to provide accurate location and orientation.

For more details, visit the product page [here](https://anavs.com/products/embedded-modules/gnss-card-g5/) 


### Why open-source and is it open-source
This board is open-source to encourage collaboration, customization, and innovation. It makes it easy for developers, hobbyists, and integrators to combine high-precision GNSS positioning with platforms like NVIDIA, experiment, create spin-off projects, and adapt it for a wide range of robotics, autonomous systems, or industrial applications.

Open-source promotes shared development, letting users build on existing work and push the technology further. It also means you have access to editable design files and are free to modify, build or sell your own version.

## Disclaimer
This project is offered as-is. The main interfaces have been tested, but the design has not been fully checked or approved by the author or Septentrio. You are responsible for how you use it in your own projects. For guidance on working with Septentrio’s GNSS mosaic modules, we suggest reaching out to Septentrio directly.

Support website: https://www.septentrio.com/en/support

### Deliverables
This open-source project contains the following files for designers, producers and integrators around Septentrio's mosaic modules.
|Files         |Description   |
|--------------|--------------|
|MosaicM2G5.PrjPcb |Altium Project  |
|Cover_Page.SchDoc|Cover page|
|M.2_Key_A+E.SchDoc|Schematics for M.2 KEY A+E|
|Mosaic-G5.SchDoc|Schematics for mosaic-G5 P3 module|
|M2G5Cover_Page.SchDoc|Intro and variants|
|MosaicM2G5.PrjPcbStructure|PCB structure|
|BOM_MosaicM2G5_REV_01.01_VARIANT_Mosaic-G5_P3H|Bill of Materials|
|MosaicM2G5 sch        |schematics PDF  |


#### Ordering mosaic module

You can order the mosaics from Digi-Key, or you can contact Septentrio directly.

| mosaic-G5 versions | Septentrio | Digi-Key part_number|
|-----------------|------------|--------|
| mosaic-G5 P1 |[Septentrio_G5-P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | - |
| mosaic-G5 P3 | [Septentrio_G5-P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [410501](https://www.digikey.com/en/products/detail/septentrio-inc/410501/28527327) |
| mosaic-G5 P3H |[Septentrio_G5-P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) | [410502](https://www.digikey.com/en/products/detail/septentrio-inc/410502/28527213) |
|M.2_mosaicG5|     - | [100040](https://www.digikey.com/en/products/detail/anavs-gmbh/100040/28164182) |


### M.2 form factor
##### Why M.2?
M.2 form factor is a standard interface used to provide a compact and flexible way to add extra functionality without redesigning the hardware. It is usually used in Laptops for Wi-Fi or SSDs, industrial PCs and embedded boards such as NVIDIA Jetson. 

NVIDIA Jetson boards are small powerful AI computers designed for applications like robotics, drones and smart systems. They provide powerful GPU performance in a compact, energy-efficient system, making them ideal for real-time AI and embedded development.

Using the M.2 form factor for the mosaic-G5 allows developers already working in the NVIDIA ecosystem to easily add the GNSS receiver without redesigning their hardware.

<img src="/pictures/Jetson Orin Nano Dev Kit.png"  width="35%"><img src="/pictures/Down view NVIDIA.png" width="35%">

The M.2 Key E+A connector can fit into a Key E and Key A slots. Key A and Key E modules are mechanically compatible with both Key A and Key E slots.  

<img src="/pictures/M.2 interface.png" width="50%" url="https://www.delock.com/infothek/M.2_2022/images/keys-a-e_engl.jpg">

## User documentation

### Interfaces
<img src="/pictures/M2G5 Interface.png" width="40%">


### Insert in NVIDIA Orin development kit
M.2_mosaicG5 can be easily connected to the NVIDIA Jetson board as shown: 

<img src="/pictures/Jetson & mosaic.png" width="80%">

You can insert the board on the underside of the NVIDIA Jetson board 

#### Pinout for M.2 Key_A+E Connector 
<img src="/pictures/m.2key a+e.png" width="40%">

| Pin # |Signal to the mosaic module|
|-------|------------------|
| 3	    |USB D+            |
| 5	    |USB D-            |
| 2,4,72,74	|power 3.3 V    |
|  6    |External LED      | 
|  16   | External LED     | 
| GND	|GND               |

* USB: the USB interface handles both satellite transmission and receiver configurations. Through this connection, the GNSS receiver can send positioning data, satellite information, and timing messages.

* Power: the board is powered via 3.3 V supply lines on multiple pins to ensure stable operation. A clean and stable power source is important for reliable GNSS performance.

* LED: these pins can be used to drive external LEDs, which are helpful for quick visual feedback

#### Pinout for mosaic-G5 module

| Pin # |mosaic module signals|
|-------|------------------|
|2|Antenna |
|5|Antenna |
| 12	|USB D+            |
| 13    |USB D-            |
|14|VBUS|
|42| Pulse Per Second|
| 44, 45|power 3.3 V    |
|  52    |External LED     | 
|  53  | External LED     | 
|54|Antenna power 3.3 V|
| GND	|GND               |

### Antenna

<img src="/pictures/antenna pin.png" width="50%">

The board exposes two RP-UMRF (micro RF) antenna connectors for GNSS signal reception. These connectors are designed for 50 Ω antennas and provide the interface for connecting external GNSS antennas to the module.

The connectors typically serve as MAIN (primary) and AUX (secondary) inputs, enabling support for advanced features such as dual-band reception and high-precision positioning (e.g., RTK)

### How to get GNSS Data
* Insert the M.2_mosaicG5 into the M.2 slot.
* Connect the GNSS antenna to the antenna connector
* Configure the receiver by downloading Septentrio Rx Tools, you can get this from [here](https://www.septentrio.com/en/products/gps-gnss-receiver-software/rxtools#resources)
* Follow the installation instructions
    * This tool allows the user to monitor satellite signals, configure receiver settings, log GNSS data and verify positioning status

    * You can also download *RxTools User Manual* to get you started


Interface
* USB (device 2.0 HS up to 480 Mbps)
* Configure PPS via the u.FL connector
Protocols
* SBF (Septentrio Binary Format)
* NMEA
* RTCM v3.x (MSM included)

The official Septentrio mosaic-G5 driver can be used
Electrical
* Input voltage: 3.3 V +/- 5%
* Power consumption:
 * Typical: 0.4-0.6 W 
 * Max: 0.9 W 
* Antenna bias voltage: 3.3 V
