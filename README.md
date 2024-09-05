![logo](https://github.com/mcgregol/WASP-N/blob/fe414bc097112d8816f5c115138489a68ba118dd/ACHIEVE%20Logo-Trans%281%29.png?raw=true)
# WASP-N User Manual

SK8TE is your tool to configure and manage Stryd sensors. Capabilities include player assignment, clock synchronization, hardware identification, and data extraction.

## Prerequisites
 - A Windows or iOS device
 - The WASP device will need to be connected to an existing WIFI network. From this network, you will need to provide the:
    - SSID
    - security type
    - password (if applicable)

> **Note:** If the network does not use DHCP, you will also need a static IP address from the network administrator to assign the WASP to.

## Usage

The WASP has two colored LED lights. If the device is powered on, the **green** light will activate. Any changes to the current state of the device, such as a successful connection to a WiFi network, will activate the **red** light. See details below.

The micro USB port located on the side of the device can be used to charge the device by plugging it into a wall, and also to communicate with the device when plugged into a computer.

#### Green Status Light
- Double flash indicates WASP joined a WiFi network.
- Single flash indicates the WASP created a WiFi access point

#### Red Status Light
- Continuous blinking indicates the WASP is attempting to connect to a WiFi network. When in **infrastructure mode**, network connectivity was lost.
- Slower blinking indicates the battery is actively charging. The light will be solid when charging is complete.
- The light will blink between one and four times to indicate the current battery level of the device when the button is pressed.
> **Note:** Battery will only be indicated if the red LED is idle.

### Power on the WASP

Press and hold the black button until the red light activates. The green light will activate and continue to flash after the button is released. The WASP is now in **operational mode**.

#### Sleep Mode

If you wish to deactivate all wireless radios, or store the device away, enable sleep mode. Sleep mood will utilize significantly less power. To enter sleep mode, simply hold the button down until both LEDs blink slowly **three times**.

To enter **operational mode**, either press and hold the button, or connect the device to a power source via USB.
> **Note:** To charge the device in sleep mode, attach the USB before powering the device off.

## Configuration

There are currently two methods of configuring a WASP.
1. The **WASP Util** app available on the Apple App Store for iOS devices.
2.  [**WASP Config Utility**](https://support.npe.fit/hc/en-us/article_attachments/9893868124308) for Windows

### WASP Util on iOS

The WASP can be configured on iOS by following these instructions:
 1. Install **WASP Util** from the app store. 
 2. Activate Limited Access Point (LAP) mode
    1. Push the button until the RED LED flashes **twice**
    2. Push the button again for **one** second
    3. When the green light starts flashing, the WASP has entered LAP mode
 3. In iOS's WiFi settings, locate and join the network named WASP-XXXXXX, where XXXXXX are the **last** six characters of the 11 digit serial number on the back of the WASP.
 4. You may close settings, and open the configuration app. The last six characters of the WASP will be listed on the opening page.
 5. Click the entry and select **Open a Control Connection**.
 6. On the configuration page, edit the following settings:
