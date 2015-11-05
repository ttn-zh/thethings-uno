# Getting Started with The Things UNO

Super simple code samples to get you started with The Things UNO and The Things Network.

## Instructions

 * [Install Arduino IDE](https://www.arduino.cc/en/Main/Software) and connect your The Things UNO to your computer.
 * Clone this repository:

        $ git clone git@github.com:gonzalocasas/thethings-uno.git

 * Open the Arduino IDE and then open the [getting started sketch](getting-started/getting-started.ino).
 * Open the `LoRa.cpp` file and assign a new device address to your device on the line `Serial1.write("mac set devaddr 5A480101\r\n");`. For TTN Zurich, please use the address space 5A4801xx (i.e. replace `xx` with an hex value) <sup>(1)</sup>.
 * Compile and upload the code.
 * Head over to [the API and see your packets coming in](http://thethingsnetwork.org/api/v0/nodes/5A480101/).
 * Rejoice and hack something cool!

<sup>(1)</sup> TTN doesn't support over-the-air activation yet, so this is only temporary. In a later stage, it won't be needed to manually assign a device address, but for now, please be a good boy/girl and respect the address space.
