![logo](https://github.com/mcgregol/WASP-N/blob/fe414bc097112d8816f5c115138489a68ba118dd/ACHIEVE%20Logo-Trans%281%29.png?raw=true)
# WASP-N User Manual

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
 3. In iOS's WiFi settings, locate and join the network named WASP-XXXXXX, where XXXXXX are the **last** six characters of the 11 digit serial number on the back of the WASP
 4. You may close settings, and open the configuration app. The last six characters of the WASP will be listed on the opening page.
 5. Click the entry and select **Open a Control Connection**
 6. On the configuration page, edit the following settings:
	 1. Enter the SSID manually, or scan for networks. Select the correct network and enter the password if required.
	 2. Select the security type
	 3.  If the network assigns an IP address with DHCP, set the DHCP setting to **on**. If not, enter the assignment settings, and set DHCP to **off**.
 7. Tap **apply** to save the settings
 8. Tap **back**, and then **Disconnect WASP** in the popup menu
 9. Close the app and enable sleep mode on the WASP

### WASP USB Configuration Utility on Windows

The WASP can be configured on Windows by following these instructions:

> **Note:** The utility must be downloaded and installed. See [**configuration**](#configuration) to install it.

1. Open the WASP USB Configuration Utility
2. Plug the WASP into the Windows device using a micro-USB cable
3. Information pertaining to the WASP will appear in the utility. Navigate to **Infrastructure Network** and enter the following parameters:
	1. Set the **Security Type** to the method used on the WiFi network
	2. Enter the name of the WiFi network into the **SSID** field
	3.  If the network assigns an IP address with DHCP, set the DHCP setting to **TRUE**. If not, enter the assignment settings, and set DHCP to **FALSE**.
4. Tap **Configure**. The program will read **Your WASP has been configured**.
5. Unplug the WASP and enable sleep mode on the WASP

### Testing Configuration
1. Within range of the WiFi network the WASP was configured for, enable **operational mode**. Both LEDs will blink.
2. If the green LED **double blinks**, the WASP has joined the network successfully

> **Troubleshooting:** If the **red** LED does not shut off after two minutes, the WASP's configuration is incorrect. Correct any errors in the configuration.

## Caution

### Hazardous Materials Warning

The WASP-N contains a Li-Ion battery and **must** be disposed of properly.

### Moisture Warning
The WASP-N is **not** waterproof. Protect the micro-USB connector contacts from moisture.

## Regulatory Approvals

The WASP-N has received regulatory approvals in the United States(FCC), Canada(IC), European Union(CE) and Australia / New Zealand (RCM R-NZ). The end user must comply with all instructions provided by the Grantee, which includes installation and /or operating conditions necessary for compliance.

### United States

This device complies with part 15 of the FCC Rules. Operation is subject to the following two conditions: (1) This device may not cause harmful interference, and (2) this device must accept any interference received, including interference that may cause undesired operation. Changes or modifications not expressly approved by the party responsible for compliance could void the user's authority to operate the equipment.

This equipment has been tested and found to comply with the limits for a Class B digital device, pursuant to Part 15 of the FCC Rules. These limits are designed to provide reasonable protection against harmful interference in a residential installation. This equipment generates uses and can radiate radio frequency energy and, if not installed and used in accordance with the instructions, may cause harmful interference to radio communications. However, there is no guarantee that interference will not occur in a particular installation. If this equipment does cause harmful interference to radio or television reception, which can be determined by turning the equipment off and on, the user is encouraged to try to correct the interference by one of the following measures:
- Reorient or relocate the receiving antenna.
- Increase the separation between the equipment and receiver.
- Connect the equipment into an outlet on a circuit different from that to which the receiver is connected.
- Consult the dealer or an experienced radio or TV technician for help.

In order to comply with FCC and ISED RF exposure requirements, this device must be installed to provide at least 20 cm separation from the human body at all times.

### Canada

This device complies with Industry Canada’s license-exempt RSSs. Operation is subject to the following two conditions:
1. This device may not cause interference.
2. This device must accept any interference, including interference that may cause
undesired operation of the device.

In order to comply with FCC and ISED RF exposure requirements, this device must be installed to provide at least 20 cm separation from the human body at all times.

Class B digital device notice /”CAN ICES-3(B)/NMB-3(B)”
