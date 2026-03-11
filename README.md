# MosaicM2G5
MosaicM2G5 board from ANavS 

Maintainer: [(Septentrio gnss github user)](githubuser@septentrio.com)

License: Open Source Hardware License (CERN-OHL)

## What is the MosaicM2G5?
<img src="/pictures/M.2%20main%20board.png" width="80%">
This is a compact, high precision GNSS (Global Navigation Satellite System) receiver card design for embedded computing platforms ideal for industrial PCs such as NVIDIA Jetson. This card is developed by ANavS. Its small size and low power consumption makes it appropriate for applications where space and efficiency are critical. 
It is based on the mosaic G5 GNSS receiver with multiple satellite systems able to achieve 1cm precise positioning, allowing it to achieve 1cm precise positioning while using multiple satellite systems simultaneously.          

## Table of Content

## What is a mosaic-G5 module?
This is Septentrio’s compact GNSS receiver with high-reliability and exceptional accurate performance. It integrates the latest generation of GNSS technology, delivering highly accurate positions with minimal power consumption. Multi-band, multi-constellation gives the receiver access to every possible signal from all available GNSS satellite constellations including the U.S. GPS, European Galileo, Russian GLONASS, as well as BeiDou and more. 

The mosaic G5 comes with different versions. The key features and differences are listed in the table below:

| Features     | [mosaic-G5 P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | [mosaic-G5 P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [mosaic-G5 P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) |
|--------------|--------------|--------------|---------------|
|Use case      |Positioning   |High-precision positioning |Positioning + Heading|
| GNSS bands   | Triple-band  | Quad-band    | Quad-band     |
| RTK support  | Yes          | Yes          | Yes           |
| Dual antenna |              |              | Yes           |
| Heading      |              |              | Yes           |



#### Other mosaic versions
 You can use other [mosaic modules](https://www.septentrio.com/en/products/gnss-receivers?f%5B0%5D=type%3A604), but you need to pay attention to the functions and pins that could be exposed, then modify the design for your own project. 

## Who is Septentrio?
<img src="/pictures/Septentrio_logo.png" width="30%">

Septentrio is a top company that designs, manufactures and sells high precision and multi-frequency GPS/GNSS receivers for demanding applications. Septentrio products are used in different industries including automotive, marine, construction, rail, machine control, logistics, precision agriculture, geographic information systems (GIS), Unmanned aerial vehicles (UAVs), survey, mapping and scientific. Septentrio’s receivers constantly deliver accurate and precise GNSS positioning scalable to centimetre-level and designed to perform perfectly in challenging environments. 

Septentrio's technology offers high accuracy and reliability thanks to advanced GNSS algorithms as well as [Advanced interference Monitoring and mitigation (AIM+)](https://www.septentrio.com/en/learn-more/advanced-positioning-technology/aim-anti-jamming-protection) This protects your application against jamming (RF interference) and spoofing (malicious attacks).

For more information about Septentrio products go to [**https://www.septentrio.com/**](https://web.septentrio.com/GH-SSN-home).
## Caution
The MosaicM2G5 used *mosaic-G5 P3*, not the *mosaic-G5-P6* please keep this in mind when designing your own project.

The M.2 Key E+A connector can fit into a Key E and Key A slots. Plus a Key A and Key E can also fit in both Key A and Key E slots.   

<img src="/pictures/M.2 interface.png" width="60%" url="https://www.delock.com/infothek/M.2_2022/images/keys-a-e_engl.jpg">

## User documentation
### How to get GNSS Data
* Insert the MosaicM2G5 to the M.2 slot.
* Connect the GNSS antenna to the antenna connector
* Configure the receiver by downloading Septentrio Rx Tools, you can get this from [here](https://www.septentrio.com/en/products/gps-gnss-receiver-software/rxtools#resources)
* Follow the installation instructions
    * This tool allows the user to monitor satellite signals, configure receiver settings, log GNSS data and verify positioning status
    * You can also download *RxTools User Manual* to get you started


### Hardware files
* Altium Project files
* Schematics PDF 
* BOM (Bill of Materials)
#### Ordering mosaic

You can order the mosaics from Digi-key, or you can contact Septentrio for directly.

| mosaic versions | Septentrio | Digikey part_number|
|-----------------|------------|--------|
| mosaic G5-P1 |[Septentrio_G5-P1](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-g5-p1) | - |
| mosaic G5-P3 | [Septentrio_G5-P3](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3) | [410501](https://www.digikey.com/en/products/detail/septentrio-inc/410501/28527327) |
| mosaic G5-P3H |[Septentrio_G5-P3H](https://www.septentrio.com/en/products/gnss-receivers/gnss-receiver-modules/mosaic-G5-P3H) | [410502](https://www.digikey.com/en/products/detail/septentrio-inc/410502/28527213) |
| MosaicM2G5 |     - | [100040](https://www.digikey.com/en/products/detail/anavs-gmbh/100040/28164182) |

### Interfaces
<img src="/pictures/M2G5 Interface.png" width="80%">

#### Pinout for M.2 Key_A+E Connector 

| Pin # |Signal            |
|-------|------------------|
| 3	    |USB D+            |
| 5	    |USB D-            |
| 2, 4	|VBAT              |
| 2 	|LED#1             |
| 16	|LED#2             |
| 2,4,72,74	|power 3.3V    |
| GND	|GND               |


#### Pinout for mosaicG5 

| Pin #	|Signal     |
|-------|-----------|
| 2	    |ANT 1      |
| 5	    |ANT 2      |
| 42    |PPS1 OUT   |
| 12	|USB D+     |
| 13	|USB D-        |
| 14	|USB VBUS      |
| 51	|VREF_O        |
| 50	|VREF_I        |
| 48	|REF_I         |
| 47	|REF_O         |
| 52	|GPIO1         |
| 53	|GPIO2         |


Interface
-	USB (device 2.0 HS up to 480Mbps)
-	Configure PPS via the u.FL connector
Protocols
-	SBF (Septentrio Binary Format)
-	NMEA
-	RTCM v3.x (MSM included)
The official Septentrio mosaic G5 driver can be used
Electrical
Input voltage 3.3V +/- 5%
Power consumption 0.4-0.6 W typ, 0.9W max
Antenna bias voltage 3.3V
