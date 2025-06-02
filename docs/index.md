<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.5.0/model-viewer.min.js"></script>

# Overview and Basic Usage

The [Spikonado Universal DC Power Module I](https://spikonado.com/product/spikonado-universal-dc-power-module-i) is a versatile and high-current buck converter designed to power your most demanding electronics projects. It efficiently (92.7%) converts a wide **13-24V** DC input into three stable, dedicated outputs:

- **12V @ 4A**
- **5V @ 10A**
- **3.3V @ 8A**

<figure markdown>
  <model-viewer alt="3D View of Spikonado Universal DC Power Module I" src="../assets/3d_model/Spikonado_Universal_DC_Power_Module_I.glb" camera-controls autoplay style="width: 500px; height: 300px;">
  </model-viewer>
  <figcaption markdown>3D View of Spikonado Universal DC Power Module I</figcaption>
</figure>

This module is perfect for robotics, embedded systems, single-board computers (SBCs), custom test jigs, and any application requiring reliable multi-voltage power.<br>
Further enhancing its flexibility, the board includes USB-C and USB-A outputs.<br>
What's more, we have also included EN and PG pins through which you can control the board using a microcontroller and also attach a switch to the board.

The board also includes the following protections:

1. Over Current Limit (OCL) - Protects the board from overloads by limiting the output current.
2. Undervoltage Lockout (UVLO) - When the input voltage on VIN falls below the required voltage, the particular voltage output shuts off.
3. Thermal Shutdown - When any of the buck converter ICs included on the board get too hot, the particular voltage output shuts off.
4. Undervoltage and Overvoltage Protection (UVP & OVP) (Not included for 12V output) - When the output voltage falls too low or goes too high than the desired voltage, the output is discharged and latched.

## Setting it Up

You must have recieved the following components in your package, when ordering from us:

1. [Spikonado Universal DC Power Module I](https://spikonado.com/product/spikonado-universal-dc-power-module-i) - x1
2. 2.54mm 1x2 Pin Male Header Strip - x3
3. 2.54mm 1x2 Pin Female Header Strip - x3
4. 2.54mm 1x1 Pin Male Header Strip - x3
5. 2.54mm 1x1 Pin Female Header Strip - x3
6. 5.0mm 1x2 Pin Screw Terminal Block - x4
7. 2.54mm 1x2 Pin Female Jumper - x3

Solder the headers and screw terminals onto your board as you desire.<br>
After soldering, it is recommended to use a multimeter to check that no shorts have been made by you during the soldering process.

Then, on the 3 EN pin pairs attach the jumpers or make a solder connection (not recommended) between the 2 pins of each pair if you aren't soldering the EN male headers onto your board. If soldering the female headers, you can also use male to male jumper wires to make the connection.

## Basic Usage

You need to first solder / screw (Screw Terminal) in two wires from your DC power output (ex. battery pack or wall adapter), into the VIN and GND ports of the board.<br>
You should now see all the 3 LEDs on the output terminals of the board lit, this means that all the outputs are working.<br>
You can now connect any DC load onto the output terminals of the board by soldering, screwing (Screw Terminal) or plugging (USB-C / USB-A) it in.

## Next Steps

Have a look at [What are EN and PG?](what_are_en_and_pg.md) to learn how to use those pins.<br>

## Related Resources

Have a look at [Specifications](specifications.md) to know more about the board's inner circuit alongside precise information on voltage and current ratings.
