# PocketBeagle_Ethernet_Cape
Design Files for an Ethernet Cape for the PocketBeagle.

This design and documentation are released under the TAPR Open Hardware License.
https://www.tapr.org/ohl.html
There is no warranty as to suitability or applicability for any purpose.
There may be additional licenses or restrictions associated with the use of the Microchip LAN9500A device.

## Notes:
Board Files are Eagle 7.7

The PocketBeagle is configured so that USB Port 0 is a "slave port" only, and is the port pinned out to the Micro-USB connector on the PocketBeagle.

USB Port 1 is configured as a Master, only. It is pinned out to the I/O Expansion Connector P1, pins 3, 5, 7, 9, 11, 13, and 15. This is the port used by this Ethernet 'Cape'.

This design uses a QFN package and surface mount parts as small as 0402, in order to fit the Ethernet interface in a space as small as the PocketBeagle footprint. It is not an appropriate project for someone not experienced in SMT assembly.

The PocketBeagle has a totally symmetrical IO connector configuration. There is nothing that prevents the reversed or offset insertion of this cape. Components may be damaged if the cape is installed backwards, or offset.

This design includes an EEPROM for the permanent assignment of a MAC address to the Ethernet interface. There are software tools for the programming of this EEPROM device in the LAN9500A section of the Microchip website.
Obtaining a legitimate MAC address for use in any assembled boards is the responsibility of the builder.

Bare PC boards built from this Eagle ".brd" file are available from OshPark, minimum order of three boards:
https://oshpark.com/shared_projects/GOEnFXdS
