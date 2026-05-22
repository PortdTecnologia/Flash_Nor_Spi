This library operates with SPI NOR Flash memories through Software SPI (bit-bang),
thus depending on the `SW_SPI.h` file.
https://github.com/PortdTecnologia/Bitbang_Protocols/blob/main/SW_SPI.h

Because it operates using bit-bang, it can be used on virtually any microcontroller,
including those without hardware SPI support, provided there is enough memory
available for the buffers.

It includes functions for:

* Reading manufacturer, model, and capacity identification parameters (JEDEC).
* Page, sector, and block erase functions.
* Reading and writing 256-byte pages.
* Reading and writing 512-byte sectors for filesystem compatibility.
* Predefined manufacturer strings for serial printing.

### Structures

`Flash_JEDEC[4]`
: Manufacturer, Model, Capacity in Mbit, and Capacity in MegaBytes.

`Flash_Vendor[14]`
: Manufacturer literal string (for supported entries).

---

Dependences: https://github.com/PortdTecnologia/Bitbang_Protocols/blob/main/SW_SPI.h

---

More information:  
https://www.youtube.com/@Gustavo_PORTD
