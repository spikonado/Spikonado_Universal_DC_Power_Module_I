# Spikonado Universal DC Power Module I

The [Spikonado Universal DC Power Module I](https://spikonado.com/product/spikonado-universal-dc-power-module-i) is a versatile and high-current buck converter designed to power your most demanding electronics projects. It efficiently (92.7%) converts a wide **13-24** DC input into three stable, dedicated outputs:

- **12V @ 4A**
- **5V @ 10A**
- **3.3V @ 8A**

This module is perfect for robotics, embedded systems, single-board computers (SBCs), custom test jigs, and any application requiring reliable multi-voltage power.<br>
Further enhancing its flexibility, the board includes USB-C and USB-A outputs.<br>
What's more, we have also included EN and PG pins through which you can control the board using a microcontroller and also attach a switch to the board.

The board also includes the following protections:

1. Over Current Limit (OCL) - Protects the board from overloads by limiting the output current.
2. Undervoltage Lockout (UVLO) - When the input voltage on VIN falls below the required voltage, the particular voltage output shuts off.
3. Thermal Shutdown - When any of the buck converter ICs included on the board get too hot, the particular voltage output shuts off.
4. Undervoltage and Overvoltage Protection (UVP & OVP) (Not included for 12V output) - When the output voltage falls too low or goes too high than the desired voltage, the output is discharged and latched.

## 📂 About this Repository

This repository is your central hub for all information, design files, and resources related to the Spikonado Universal DC Power Module I. Our aim is to provide everything you need to understand, use, and even build upon this product.

You'll find:

- `docs/`: Comprehensive documentation, including datasheets, specifications, and user guides.
- `hardware_design/`: Complete KiCad project design files – schematics and PCB layout for the board.

## Accessing the Documentation

The `docs/` directory contains the source files for our comprehensive product documentation. For the best reading experience, with all formatting and interactive elements correctly rendered, please view the built version on our [website](https://docs.spikonado.com/spikonado-universal-dc-power-module-i).

While you can browse the raw files in the `docs/` directory on GitHub, they are primarily intended for those contributing to the documentation or exploring its source structure.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check existing issues or open a new one.

## 📄 License

This product is open source!

Please review the following files for license information:

- `hardware_design/LICENSE.md`

If you have any questions or concerns related to licensing, please email support at support@spikonado.com.
