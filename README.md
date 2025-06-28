# How to Interpret/Read the LEDs for USB Cable Testers

**NOTE** This is a work in progress. Please leave comments or better, pull requests, with updates. Please verify with actual cables. 

This "application" is hosted on GitHub pages: <a href="https://patrickgardella.github.io/usbcabletester/">Interpreting the LEDs on a USB Cable Tester</a>.

## Description

For the initial work, I am using the [Treedix USB Cable Tester](https://amzn.to/3PSow5w) (affiliate link). The [Treedix USB Cable Tester](https://amzn.to/3PSow5w) (affiliate link) is an inexpensive, but highly functional USB Cable Tester. You can use it to identify and test many different types of USB cables, including unusual ones.

Others should use this same pattern, but there could be additional things other cable testers are testing for. Feel free to send [me](https://github.com/patrickgardella) one, and I'll add it here.

## References
* [USB hardware - Wikipedia](https://en.wikipedia.org/wiki/USB_hardware)
* [USBefuddled: Untangling the Rat's Nest of USB-C Standards and Cables](https://tidbits.com/2021/12/03/usbefuddled-untangling-the-rats-nest-of-usb-c-standards-and-cables/) 

## USB Cable Types

Wikipedia's article on [USB Hardware](https://en.wikipedia.org/wiki/USB_hardware) shows the standards for USB Cables - that is, what plugs can be on each end. 

The Treedix USB Cable tester can test the following plugs:

* Apple Lightning
* USB 2.0 A
* USB 2.0 Mini-B
* USB 2.0 Micro-B
* USB 3.0 A
* USB 3.0 Micro-B
* USB 3.0 B
* USB 3.0 C (Male and Female) 

You can use this diagram to understand what each plug looks like and the common arrangements.

![USB Plug Diagram from Wikipedia](/images/Wikipedia-CommonUSBCables.png)

## Interpreting the LEDs

The Treedix manual includes some examples of common USB functions, but not all.

On the bottom left is a set of two LEDs, ID and Shield. 

|  |  |  |
|--|--|--|
| ID | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | Indicates the presence of an ID chip |
| Shield | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | Indicates a shield |

#### Charging Only

* Some USB 2.0 A, Mini-B, Micro-B

These are often inexpensive cables included with electronic devices by the manufacturer for charging purposes only.

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A9 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A4 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A1 | GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |

_Verified_ with cable

#### Charging & Data

* Many USB 2.0 A, Mini-B, Micro-B

This is the expected response of a fully functional USB 2.0 cable

* Some USB 3.0 A

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A9 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A4 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A1 | GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |

_Not_ Verified with cable

#### Charging & Data

* Many USB 2.0 A, Mini-B, Micro-B

This is the expected response of a fully functional USB 2.0 cable

* Some USB 3.0 A

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)  | &nbsp; | A9 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A1 | GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |

_Verified_ with cable

#### Charging Only - Converters

* Some USB 2.0 A to USB-C

Provides power to both ends of the cable.

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A9 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)  | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)  | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A1 | GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |

_Verified_ with cable

#### Charging and Data - Converters 1

* Some USB 2.0 A to USB-C

Provides power to both ends of the cable and is capable of data.

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A9 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/Ff4B33.svg)  | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A1 | GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |

_Verified_ with cable

#### Charging and Data - Converters 2

* Some USB 2.0 A to USB-C

Provides power to both ends of the cable and is capable of data.

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A9 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)  | &nbsp; | A7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)  | &nbsp; | A6 | D+ | ![N](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 | VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A1 | GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |

_Verified_ with cable

#### Charging & High Speed Data

* Most USB 3.0 A, Micro-B
* Many USB-C 3.0

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A12 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B2 |TX2+| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A11 |RX2+| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B3 |TX2-| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A10 |RX2-| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A9  |VBUS| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B5 |CC2 | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A8 |SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A7 | D-  | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A6 | D+  | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)| &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 |VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)| &nbsp; | A3 |TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg)| &nbsp; | A2 |TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A1 |GND  | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |

_Not_ Verified with cable

#### Charging, High Speed Data, Audio and Voice

* Many USB-C 3.0

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A12 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B2 |TX2+| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A11 |RX2+| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B3 |TX2-| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A10 |RX2-| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B4 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A9  |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B5 |CC2 | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A8 |SBU1 | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A7 | D-  | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A6 | D+  | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)| &nbsp; | A5 | CC1 | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A4 |VBUS | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B10 |RX-| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)| &nbsp; | A3 |TX1- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B11 |RX+| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)| &nbsp; | A2 |TX1+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |
| B12 |GND| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A1 |GND  | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) |

_Not_ Verified with cable

#### Apple Lightning

| Pinrow B | Name | LED |   | Pinrow A | Name | LED   | 
|---|----|---|---|---|---|----|
| B1 |GND | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A12 |GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B2 |TX2+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A11 | RX2+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B3 |TX2-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A10 | RX2- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B4 |VBUS| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A9 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B5 |CC2 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A8 | SBU1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B6 | D+ | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A7 | D- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B7 | D- | ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg) | &nbsp; | A6 | D+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B8 |SBU2| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A5 | CC1 | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B9 |VBUS| ![ON](https://placehold.co/20x10/FF4B33/FF4B33.svg)  | &nbsp; | A4 | VBUS | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B10 |RX-| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A3 | TX1- | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B11 |RX+| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A2 | TX1+ | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |
| B12 |GND| ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) | &nbsp; | A1 | GND | ![OFF](https://placehold.co/20x10/D3D3D3/D3D3D3.svg) |

_Verified_ with cable