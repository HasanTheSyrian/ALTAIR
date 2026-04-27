![ALTAIR](https://github.com/user-attachments/assets/b61b74c0-defb-4e71-bc80-f6e173e74274)
<img width="1161" height="850" alt="image" src="https://github.com/user-attachments/assets/ada5a975-57cc-4c11-9392-07703c0b5d20" />

17 light-years away lies Altair, a star in the Aquila constellation. Altair is the short-form transliteration of Al-Nisr Al-Ta'ir (النسر الطائر) or "The Flying Eagle"; a predator known for its excellent vision.

The Altair is an FPGA development board focused on image processing, specifically, stereoscopic depth calculation enabled by two MIPI camera connectors. The board implements XAPP894 since MIPI is not supported natively by Zynq 7000. The development board is built around the MYC-C7Z010_20 SOM. This board is also my graduation project/thesis for my Mechatronics Engineering degree.

---
NOTE: THIS BOARD IS NOT TESTED YET
### Docs
This board is built with the MYIR MYC-C7Z020-V2 SOM. MYIR documents can only be downloaded after providing the serial number of the MYC-C7Z020-V2 purchased, unfortunately, I can't share mine. Most MYIR hardware documents can be downlodaded from this repository. I haven't included software documents/code because the file size is too big however you can probably find them online elsewhere.

AltairNotes PDF contains my notes I have written over the ~2 years I have been working on this project. Some information is basic stuff about PCB routing and some information documents how I have configured and routed my board.

I combined software and hardware PDS into PDF files ending in "COMBINED" so you can easily search for what you want.

I have created a YouTube series that talks about the design which can be seen [here](https://www.youtube.com/@hasanthesyrian_).

Not all references are included because I'm not sure if they can be shared directly, however, you should be able to just search for them and download them from their official source.

#### Most important/relevant
| Title                                                                                                                                                                    | Notes      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |------------|
| HARDWARE DOCS COMBINED                                                                                                                                                   | MYIR Docs  |
| MYC-C7Z010-20-V2 Hardware Design Guide-V1.0                                                                                                                              | MYIR Docs  |
| SOFTWARE DOCS COMBINED                                                                                                                                                   | MYIR Docs  |
| MYB-C7Z010_20-V2 Schematic                                                                                                                                               | MYIR Docs  |
| MYD-C7Z01020-V2 PinOuts                                                                                                                                                  | MYIR Docs, SOM Pinout  |
| MYC-C7z010-V12-SOM-NET-LENGTH                                                                                                                                            | MYIR Docs  |
| ADV7511_Hardware_Users_Guide                                                                                                                                             | HDMI IC    |
| [Zynq 7000 SoC Technical Reference Manual](https://docs.amd.com/r/en-US/ug585-zynq-7000-SoC-TRM)                                                                         | UG585  |
| [Zynq-7000 SoC PCB Design Guide](https://docs.amd.com/v/u/en-US/ug933-Zynq-7000-PCB)                                                                                     | UG933  |
| [7 Series FPGAs SelectIO Resources User Guide](https://docs.amd.com/v/u/en-US/ug471_7Series_SelectIO)                                                                    | UG471  |
| [Zynq-7000 SoC Packaging and Pinout Product Specification](https://docs.amd.com/v/u/en-US/ug865-Zynq-7000-Pkg-Pinout)                                                    | UG865  |
| xc7z020clg400pkg (.txt)                                                                                                                                                  | FPGA Package Pinout  |

#### Board schematics used as references in part
| Title                                                                                                                                                                    | Notes      |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |------------|
| MYB-C7Z010_20-V2 Schematic                                                                                                                                               | MYIR Docs  |
| arty_z7_sch                                                                                                                                                              |   |
| digilent-smt3-reversed-sch                                                                                                                                               | Reverse engineered programmer published on IEEE  |
| eclypse_z7_sch                                                                                                                                                           |   |
| minized_sch                                                                                                                                                              |   |
| mizar_z7-sch                                                                                                                                                             |   |
| pynq-z1_sch                                                                                                                                                              |   |
| pynq-z2_sch                                                                                                                                                              |   |
| rehsd_sch                                                                                                                                                                | rehsd on YouTube  |
| snickerdoodle_sch                                                                                                                                                        |   |
| trenz_carrier_TE0701_sch                                                                                                                                                 |   |
| zc702_sch                                                                                                                                                                |   |
| zc706-sch                                                                                                                                                                |   |
| trenz_carrier_TE0701_sch                                                                                                                                                 |   |
| zc702_sch                                                                                                                                                                |   |
| zedboard_sch                                                                                                                                                             |   |
| zybo-z7_sch                                                                                                                                                              |   |
| zynqberry2010_sch                                                                                                                                                        |   |
| zynqberry-zero_sch                                                                                                                                                       |   |
| camera-module-3-schematics                                                                                                                                               | Raspberry Pi |
| cm4io-datasheet                                                                                                                                                          | Raspberry Pi |
| raspberry-pi-4-reduced-schematics                                                                                                                                        | Raspberry Pi |

#### AMD Documentaion
| Title                                                                                                                                                                    | Code   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------ |
| [Zynq 7000 SoC Technical Reference Manual](https://docs.amd.com/r/en-US/ug585-zynq-7000-SoC-TRM)                                                                         | UG585  |
| [Zynq-7000 SoC PCB Design Guide](https://docs.amd.com/v/u/en-US/ug933-Zynq-7000-PCB)                                                                                     | UG933  |
| [Zynq-7000 SoC Data Sheet: Overview](https://docs.amd.com/v/u/en-US/ds190-Zynq-7000-Overview)                                                                            | DS190  |
| [Zynq-7000 SoC Packaging and Pinout Product Specification](https://docs.amd.com/v/u/en-US/ug865-Zynq-7000-Pkg-Pinout)                                                    | UG865  |
| [Zynq 7000 SoC and 7 Series Devices Memory Interface Solutions User Guide](https://docs.amd.com/r/en-US/ug586_7Series_MIS/DDR3-and-DDR2-SDRAM-Memory-Interface-Solution) | UG586  |
| [DDR2/DDR3 Low-Cost PCB Design Guidelines for Artix-7/Spartan-7 FPGAs White Paper](https://docs.amd.com/v/u/en-US/wp484-a7-s7-ddr2-3-pcb)                                | WP484  |
| [7 Series FPGAs and Zynq-7000 SoC XADC Dual 12-Bit 1 MSPS Analog-to-Digital Converter User Guide](https://docs.amd.com/r/en-US/ug480_7Series_XADC)                       | UG480  |
| [Zynq-7000 SoC Product Selection Guide](https://docs.amd.com/v/u/en-US/zynq-7000-product-selection-guide)                                                                | XMP087 |
| [Artix 7 FPGAs Data Sheet: DC and AC Switching Characteristics](https://docs.amd.com/v/u/en-US/ds181_Artix_7_Data_Sheet)                                                 | DS181  |
| [Kintex-7 FPGAs Data Sheet: DC and AC Switching Characteristics](https://docs.amd.com/v/u/en-US/ds182_Kintex_7_Data_Sheet)                                               | DS182  |
| [7 Series FPGAs GTP Transceivers User Guide](https://docs.amd.com/v/u/en-US/ug482_7Series_GTP_Transceivers)                                                              | UG482  |
| [7 Series FPGAs GTX/GTH Transceivers User Guide](https://docs.amd.com/v/u/en-US/ug476_7Series_Transceivers)                                                              | UG476  |
| [7 Series FPGAs PCB Design Guide](https://docs.amd.com/v/u/en-US/ug483_7Series_PCB)                                                                                      | UG483  |
| [Zynq 7000 SoC Software Developers Guide](https://docs.amd.com/r/en-US/ug821-zynq-7000-swdev)                                                                            | UG821  |
| [Recommended Design Rules and Strategies for BGA Devices User Guide](https://docs.amd.com/r/en-US/ug1099-bga-device-design-rules)                                        | UG1099 |
| [Zynq-7000 SoC DC and AC Switching Characteristics Data Sheet](https://docs.amd.com/v/u/en-US/ds187-XC7Z010-XC7Z020-Data-Sheet)                                          | DS187  |
| [7 Series FPGAs Configuration](https://docs.amd.com/v/u/en-US/ug470_7Series_Config)                                                                                      | UG470  |
| [MIPI D-PHY LogiCORE IP Product Guide](https://docs.amd.com/r/en-US/pg202-mipi-dphy/Introduction)                                                                        | PG202  |
| [MIPI CSI-2 Receiver Subsystem Product Guide](https://docs.amd.com/r/en-US/pg232-mipi-csi2-rx)                                                                           | PG232  |
| [Xilinx FPGA Video Design Hub](https://docs.amd.com/v/u/en-US/dh0083-video-hub)                                                                                          | DH235  |
| [HDMI 1.4/2.0 Transmitter Subsystem Product Guide](https://docs.amd.com/r/en-US/pg235-v-hdmi-tx-ss/Introduction?tocId=XLSPfpAut4Tw1N_71V9XKQ)                            | PG235  |
| [Vivado Design Suite User Guide: I/O and Clock Planning](https://www.xilinx.com/support/documents/sw_manuals/xilinx2022_1/ug899-vivado-io-clock-planning.pdf)            | UG899  |
| [7 Series FPGAs SelectIO Resources User Guide](https://docs.amd.com/v/u/en-US/ug471_7Series_SelectIO)                                                                    | UG471  |

### Other helpful links

| Title                                                                                                                                                                                                              | Notes                                                     | Code    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------- | ------- |
| [Xilinx Power Estimator](https://www.xilinx.com/products/technology/power/xpe.html)                                                                                                                                |                                                           |         |
| [Digilent Arty Z7 Schematics](https://digilent.com/reference/_media/reference/programmable-logic/arty-z7/arty_z7_sch.pdf)                                                                                          |                                                           |         |
| [Digilent Zed Board Schematics](https://digilent.com/reference/_media/reference/programmable-logic/zedboard/zedboard-schematic-rev-e1-public.pdf?srsltid=AfmBOoql7CUt0AFnhOoANW0G6yMl43WzjD8dBcZ4Vhi4z6flo701Imns) | HDMI schematic on page 5                                  |         |
| [Xilinx XTP185 – ZC702 Schematics](https://e2e.ti.com/cfs-file/__key/communityserver-discussions-components-files/196/zc702_5F00_Schematic_5F00_xtp185_5F00_rev1_5F00_0.pdf)                                       | link instantly downloads pdf                              |         |
| [TI Power Reference Design for Xilinx Zynq-7000](https://www.ti.com/lit/ug/slyu019a/slyu019a.pdf?ts=1724258668028&ref_url=https%253A%252F%252Fwww.google.com%252F)                                                 |                                                           |         |
| [Terasic DE2-115 Schematic](https://wiki.bu.ost.ch/infoportal/_media/fpga/cyclone_iv/de2_115_schematic.pdf)                                                                                                        |                                                           |         |
| [Avnet Minized Board Schematics + General knowledge](http://www.ebvnews.ru/doc17/MiniZed-HW-UG-v1-0-V1_0.pdf)                                                                                                      | check page 7                                              |         |
| [How to understand Zynq Pins](https://www.avnet.com/wps/portal/us/products/avnet-boards/support/faq/zynq-pins-deep-dive/)                                                                                          |                                                           |         |
| [Hardware and Layout Design Considerations for DDR3 SDRAM Memory Interfaces](https://hands.com/~lkcl/eoma/rockchip_rk3288/AN3940.pdf)                                                                              |                                                           |         |
| [Gigabit Ethernet 101: Basics to Implementation](https://resources.altium.com/p/gigabit-ethernet-101-basics-implementation)                                                                                        |                                                           |         |
| [Gigabit Ethernet Design Guide](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ApplicationNotes/ApplicationNotes/00002054A.pdf)                                                                    |                                                           |         |
| [Ethernet PHY PCB Design Layout Checklist](https://www.ti.com/lit/an/snla387/snla387.pdf?ts=1724186585377&ref_url=https%253A%252F%252Fwww.google.com%252F)                                                         |                                                           |         |
| [TPD12S016 HDMI Companion Chip Datasheet](https://www.ti.com/lit/ds/symlink/tpd12s016.pdf?ts=1724260463561&ref_url=https%253A%252F%252Fwww.google.com%252F)                                                        |                                                           |         |
| [MIPI D-PHY Standard](https://www.mipi.org/specifications/d-phy#related-resources-anchor)                                                                                                                          |                                                           |         |
| [Zynp Pins - Deep Dive: How to understand Zynq Pins](https://www.avnet.com/wps/portal/us/products/avnet-boards/support/faq/zynq-pins-deep-dive/?srsltid=AfmBOorTJiz7Mt2yYFR5GlrBl0hjKMVnr36xj8_0COGvssak9dttpD7k)  | Useful                                                    |         |
| [ADV7511 Hardware User's Guide](https://www.analog.com/media/en/technical-documentation/user-guides/ADV7511_Hardware_Users_Guide.pdf)                                                                              | "actual" datasheet of ADV7511                             |         |
| [PCB Design Guidelines for QFN and DQFN Packages](https://ww1.microchip.com/downloads/aemDocuments/documents/UNG/ApplicationNotes/ApplicationNotes/AN18.15-PCB-Design-Guide-QFN-DQFN-Packages-00001843.pdf)        | USB2415 USB HUB                                           | AN18.15 |
| [USB Device Design Checklist](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ApplicationNotes/ApplicationNotes/00001863B.pdf)                                                                      | USB2415 USB HUB                                           | AN26.21 |
| [PCB Layout Guide for USB Hubs](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ApplicationNotes/ApplicationNotes/en562810.pdf)                                                                     | USB2415 USB HUB                                           | AN15.17 |
| [PMOD Standard](https://digilent.com/reference/_media/reference/pmod/pmod-interface-specification-1_3_1.pdf)                                                                                                       |                                                           |         |
| Texas Instruments HDMI Design Guide                                                                                                                                                                                | HDMI                                                      |         |
| [Texas Instruments The IBIS model, Part 3: Using IBIS models to investigate signal-integrity issues](https://www.ti.com/lit/an/slyt413/slyt413.pdf?ts=1754720541924)                                               |                                                           | SLYT413 |

<details>
<summary>Processing System Pins Used</summary>
<img width="580" height="573" alt="Pasted image 20250327221556" src="https://github.com/user-attachments/assets/fcaedaf4-c1c1-46c5-912f-0de1979ed7b9" />
</details>

### Images



<img width="1099" height="800" alt="image" src="https://github.com/user-attachments/assets/0d92de30-b80d-482e-ae30-7131ae2702d3" />

<img width="1130" height="774" alt="Screenshot 2026-04-07 160808" src="https://github.com/user-attachments/assets/62d2506e-1ec0-47f3-9838-82c4fe8d3dc0" />


<details>

<summary>Archive</summary>

<img width="1110" height="803" alt="image" src="https://github.com/user-attachments/assets/3cb0f376-9b8b-4708-ab03-ded84dc060fe" />
<img width="1180" height="851" alt="image" src="https://github.com/user-attachments/assets/1c40b4b5-1d0c-4474-aaca-3d198d22ff6e" />

</details>
