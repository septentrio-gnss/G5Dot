# MosaicM2G5
MosaicM2G5 board from ANavS 

Maintainer: [(Septentrio gnss github user)](githubuser@septentrio.com)
License: 
## What is the MosaicM2G5?
This is a compact, high precision GNSS (General Navigation Satellite system) receiver card design for embedded computing platforms ideal for industrial PCs such as Nvidia Jetson. This card is developed by ANavS. Its small size and low power consumption makes it appropriate for applications where space and efficiency are critical. 
It is based on the mosaic G5 GNSS receiver with multiple satellite systems able to achieve 1cm precise positioning, allowing it to connect to achieve 1cm precise positioning and multiple satellite systems at once.

## Table of Content

## What is a mosaic G5?
This is a Septentrio’s now newest multi-band multi-constellation low power GNSS receivers that provides high position and highly protects against jamming and spoofing.
#### Other mosaic versions
 You can used other [Mosaic modules](https://www.septentrio.com/en/products/gnss-receivers?f%5B0%5D=type%3A604) such as Mosaic G5-p1, Mosaic G5-P3,Mosaic G5-P3H, but you need to pay attention and take into consideration the functions and pins that could be exposed, then modify the design for the purpose of your own project.

## Who is Septemtrio?
![logo](/pictures/Septentrio_logo.png)

Septentrio is a top company that designs, manufactures and sells high precision and multi-frequency GPS/GNSS receivers for demanding applications. Septentrio products are used in different industries including automotive, marine, construction, rail, machine control, logistics, precision agriculture, geographic information systems (GIS), Unmanned aerial vehicles (UAVs), survey, mapping and scientific. Septentrio’s receivers constantly delivers accurate and precise GNSS positioning scalable to centimetre-level designed to perform perfectly in challenging environments. 

Steptentrio's technology offers high accuracy and reliability thanks to GNSS + algorithms as well as [Septentrio's Advanced interference Monitoring and mitigation (AIM+)](https://www.septentrio.com/en/learn-more/advanced-positioning-technology/aim-anti-jamming-protection) This protects against jamming (RF interference) and spoofing

For more information about Septentrio products go to [**https://www.septentrio.com/**](https://web.septentrio.com/GH-SSN-home).

## User documentation

### Hardware files
* Altium Project files
* schematics PBF 
* BOM (Bill Of Materials)

#### Pinout for M.2 Key_A+E Connector 

| Pin # |Signal            |
|-------|------------------|
| 3	USB |D+                |
| 5	USB |D-                |
| 2, 4	|VBAT              |
| 2 	|LED#1             |
| 16	|LED#2             |
| 2,4,72,74	|power 3.3V    |
| GND	|GND               |


#### Pinout for MosaicG5 

| Pin #	|Signal     |
|-------|-----------|
| 2	    |ANT 1      |
| 5	    |ANT 2      |
| 42    |PPS1 OUT    |
| 12	|USB D+        |
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
-	Configure PPS via u.FI
Protocols
-	SBF (septentrio binary format)
-	NMEA
-	RTCM v3.x(MSM included)
The official Septentrio Mosaic G5 driver can be used
Electrical
Input voltage 3.3v +/- 5%
Power consumption 0.4-0.6 W typ, 0.9W max
Antenna bias voltage 3.3
