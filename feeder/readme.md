# Smart Feeder Design Documentation

Since the device is intended operate with limited power and a high efficiency target, this section of the overall project is limited to the image processing and media delivery to another server or service. Where possible, flexibility for expansion should be added.

## Functional Requirements
* Provide support to forward images and videos using either LDAP or to another service. 
* Software identifies either the presence of motion and/or a bird and either takes pictures or begins recording until either the bird leaves or a max video duration is reached.
* Optional power saving functionality (ex: light sensor to reduce processing activity during night)

## Non-functional Requirements
* Software should minimize resource usage. Memory usage should be minimized, a concern as the Raspberry Pi 2 W is limited 512MB of RAM and other devices may have less. Power usage should be minimuzed as the device will likely be deployed with solar, ensure the software is efficient.
* Ensure modularity so end users can customize hardware (ex: camera support, software customization)