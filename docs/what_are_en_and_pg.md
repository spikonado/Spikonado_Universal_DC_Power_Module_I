# What are EN and PG?

## EN - Enable

There are 3 pairs of EN pins on the board. EN1 for 12V, EN2 for 5V, and EN3 for 3.3V.

You are supposed to short every pair of pins in order to turn on the respective outputs. So, if for example, you would like to add a switch to the board, you can simply connect it between the two pins. Whenever the switch is off, that particular voltage output will be off and when it is on, that particular voltage output will be on.

You can also control this on and off functionality through a microcontroller's digital / GPIO pins by simply not shorting the EN pair of pins together and instead connecting the digital / GPIO pin of your microcontroller to the pin right under which the EN label is.<br>
By simply setting the pin's mode to OUTPUT and turning the pin HIGH (1.2V to 5.5V) and LOW (-0.3V to 0.3V), you can turn the buck converter's voltage outputs on and off respectively.

## PG - Power Good

There are 3 PG pins on the board. PG1 for 12V, PG2 for 5V, and PG3 for 3.3V.

You can connect these pins to a microcontroller's pins and set the mode of the latter to INPUT.

The PG pins output LOW (0V) during fault conditions like OVP, UVP, UVLO, and thermal shutdown or when the converter is off / starting. Do note that the PG pins do not output LOW during Over Current Limit (OCL).<br>
The rest of the time the PG pins output HIGH (3.2 to 3.4, usually 3.3).

The PG output and status of each buck converter included in the board (12V, 5V, 3.3V) is different, one of the voltage outputs may be under fault conditions while the others may be wokring just fine.

## Related Resources

You can look at [Specifications](specifications.md) to know more about when the various fault conditions are triggered and to also know the startup time for each voltage output.
