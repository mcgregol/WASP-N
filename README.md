![enter image description here](https://achieve-performance.com/wp-content/uploads/2022/06/ACHIEVE-APP-Logo-white.png)
# WASP-N User Manual

SK8TE is your tool to configure and manage Stryd sensors. Capabilities include player assignment, clock synchronization, hardware identification, and data extraction.

## Prerequisites

 - [WASP Config Utility](https://support.npe.fit/hc/en-us/article_attachments/9893868124308)
 - The WASP device will need to be connected to an existing WIFI network. From this network, you will need to provide the:
    - SSID
    - security type
    - password (if applicable)

> **Note:** If the network does not use DHCP, you will also need a static IP address from the network administrator to assign the WASP to.

## Usage

The WASP has two colored LED lights. If the device is powered on, the **green** light will activate. Any changes to the current state of the device, such as a successful connection to a WiFi network, will activate the **red** light. See details below.

The micro USB port located on the side of the device can be used to charge the device by plugging it into a wall, and also to communicate with the device when plugged into a computer.

#### Green Status Light
1. Double flash indicates WASP joined a WiFi network.
2. Single flash indicates the WASP created a WiFi access point

#### Red Status Light
1. Continuous blinking indicates the WASP is attempting to connect to a WiFi network. When in **infrastructure mode**, network connectivity was lost.
2. Slower blinking indicates the battery is actively charging. The light will be solid when charging is complete.
3. The light will blink between one and four times to indicate the current battery level of the device when the button is pressed.
> **Note:** Battery will only be indicated if the red LED is idle.

### Power on the WASP

Press and hold the black button until the red light activates. The green light will activate and continue to flash after the button is released. The WASP is now in **operational mode**.
