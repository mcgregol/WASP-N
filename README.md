# WASP-N User Manual by ACHIEVE

SK8TE is your tool to configure and manage Stryd sensors. Capabilities include player assignment, clock synchronization, hardware identification, and data extraction.

## Prerequisites

 - [WASP Config Utility](https://support.npe.fit/hc/en-us/article_attachments/9893868124308)
 - The WASP device will need to be connected to an existing WIFI network. From this network, you will need to provide the:
    - SSID
    - security type
    - password

> **Note:** If the network does not use DHCP, you will need a static IP address from the network administrator to assign the WASP to.

You may now proceed through the installation.

## Basic Usage

Once installed, SK8TE can be accessed through the **Start Menu** or via **desktop shortcut** if opted into by the user during installation. Below is the main screen of the application.

![main](https://github.com/mcgregol/sk8te/blob/main/main.png?raw=true)
In order to begin interacting with the Stryds, we need to scan for available ones. Please ensure any Stryds you intend on working with are sufficiently charged and within close proximity of your computer.
> **Note:** Please ensure bluetooth is enabled

To begin, select **Scan**<sup>[1]</sup> to begin a 10 second scan for available devices. Once the scan is completed, a list of hardware addresses will appear in the **sensor listbox**<sup>[2]</sup>. You may select or deselect any number of devices by individually **clicking** them or **dragging** over them. **All** selected sensors will be queued when the user executes the following actions:

### Blink

Sensor(s) will asynchronously flash their LED until stopped by the user. The blink function is useful for identifying a physical piece of hardware.
>**Example:** A specific Stryd in the SK8TE app needs to be physically labelled

### Erase

Sensor(s) onboard storage will be cleared. This cannot be undone and any data not exported will be **lost** permanently. It is advisable to routinely erase sensors in order to reduce unnecessary data export time.

### Sync Clock

Sensor(s) internal clock will be updated to that of the SK8TE app's computer. The timestamps within data collected by a Stryd will **not** be correct if the sensor clock is out of sync.
>**Note:** If the computer clock is wrong during synchronization, the Stryd's clock will also be wrong

## Assign Devices and Build Your Team

In order to collect accurate data and increase ease of use, it is important to assign a player to a device. You can update essential player attributes such as weight, and once assigned the SK8TE app will list the player instead of a hardware address in the listbox. In the diagram below, the first Stryd<sup>[4]</sup> **has** been assigned, whereas the second Stryd<sup>[5]</sup> **has not**, and a hardware address is displayed instead.

![diag](https://github.com/mcgregol/sk8te/blob/main/Screenshot%202024-08-07%20123129.png?raw=true)

To begin, select as many Stryds as you need players assigned from the listbox. Next, select the **(Re)assign**<sup>[3]</sup> button from the interface. A new form will be opened.
>**Note:** Both unassigned and assigned Stryds can be selected simultaneously.

![fdf](https://github.com/mcgregol/sk8te/blob/main/form.png?raw=true)

The Stryd label<sup>[6]</sup> displays the current Stryd being assigned. In this case, the Stryd was already assigned, so the existing player name is displayed next to the hardware address, and the current number and weight are in their respective input boxes. The user then inputs the player name, number, and weight. While this process is taking place, this Stryd will **blink** indefinitely, stopping only when **Skip**<sup>[8]</sup> or **Next**<sup>[9]</sup> is selected and changes are made to the device.
>**Note:** It is recommended to physically label a Stryd while it is blinking during assignment.

As you can see in the top right of the form<sup>[7]</sup>, this Stryd is the first of two selected for assignment. Once this Stryd is assigned or skipped, the program will move to the next one, which will begin blinking, and the assignment process will repeat until all Stryds in the list are iterated through.

### Importing and Exporting a Team
Although an assigned Stryd's weight is persistently saved to the hardware of the sensor, player assignments are stored on the computer running the SK8TE app. As a result, these assignments only originally register to that instance of SK8TE.

>**Note:** Be sure to export your team assignments before upgrading SK8TE, as they **will** be overwritten.

To export Stryd player assignments, navigate to the top left of the screen and select **Extra** > **Export Database**. Specify a filename (such as the team name),  and save the JSON file. These player assignments can now be used on another device running SK8TE. To import, select **Extra** > **Import Database**.

## Exporting Data

On the far right of the screen is the export data section, displayed in the figure below. Data retrieved from a Stryd is saved to the computer running SK8TE. To specify the location of this this data once saved, select **Update Save Path**<sup>[10]</sup>. The current save path<sup>[11]</sup> will reflect these changes.

![export](https://github.com/mcgregol/sk8te/blob/main/export.png?raw=true)
To begin the export, select desired Stryds from the listbox, and then **Export Data**<sup>[12]</sup>. Data transfer between the Stryds and computer will begin, with the **total** progress displayed in the bar<sup>[13]</sup>. Also displayed, will be the current sensor that is exporting.
