# MAX32625PICO FIRMWARE IMAGES
DAPLink firmware images for MAX325PICO board

## Latest Releases
| Drag-n-Drop Target | Binary | Details SHA  | Erase support |
|--|--|--|--|
| MAX32620FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32620fthr_if_crc_swd_v1.0.3.bin)  | 34fe95 | :heavy_check_mark: |
| MAX32630FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32630fthr_if_crc_swd_v1.0.3.bin)  | 34fe95 | :heavy_check_mark: |
| MAX32660EVSYS| [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32660evsys_if_crc_dip_v1.0.3.bin) | 34fe95 | :heavy_check_mark: |
| MAX32666FTHR2| [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32666fthr2_if_crc_swd_v1.0.3.bin) | 34fe95 | :heavy_check_mark: |
| MAX32666FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32666fthr_if_crc_swd_v1.0.5.bin)  | fc211c | :heavy_check_mark: |
| MAX32655FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32655fthr_if_crc_swd_v1.0.3.bin)  | 34fe95 | :heavy_check_mark: |
| MAX32670EVKIT| [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32670evkit_if_crc_swd_v1.0.3.bin) | 34fe95 | :heavy_check_mark: |
| MAX32672FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32672fthr_if_crc_swd_v1.0.5.bin)  | fc211c | :heavy_check_mark: |
| MAX32675FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32675fthr_if_crc_swd_v1.0.5.bin)  | fc211c | :heavy_check_mark: |
| MAX32690EVKIT| [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32690evkit_if_crc_swd_v1.0.7.bin) | b85b53 | :heavy_check_mark: |
| MAX78000FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max78000fthr_if_crc_swd_v1.0.3.bin)  | 34fe95 | :heavy_check_mark: |
| MAX32650FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32650fthr_if_crc_swd_v1.0.6.bin)  | 649f2a | :heavy_check_mark: |
| MAX32625PICO | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32625pico_if_crc )                | 19f797 | :x: |
| MAX32630HSP2 | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32630hsp_if_crc_dip_v1.0.3.bin)  | 34fe95 | :heavy_check_mark: |
| MAX32666HSP3 | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32666hsp3_if_crc_dip_v1.0.5.bin)  | fc211c | :heavy_check_mark: |
| MAX32660     | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625pico_max32660_vio_in.bin )            | 84e3053 | :x: |
| MAX32660     | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625pico_max32660_power_out.bin ):warning:| fd4512f | :x: |

:warning: This image will apply 3.3V to the VIO pin of the MAXDAP connector allowing the MAX32625PICO board to power the MAX32660 Evaluation Kit. It may permanently damage other incompatible target boards.

## Bootloader Programmer Releases
| Drag-n-Drop Target | Binary | Details SHA  | Erase support |
|--|--|--|--|
| MAX32620FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32620fthr_if_crc_swd_v1.0.4_pico2.bin)  | b4a2d4 | :heavy_check_mark: |
| MAX32630FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32630fthr_if_crc_swd_v1.0.4_pico2.bin)  | b4a2d4 | :heavy_check_mark: |
| MAX32666FTHR | [Download](https://github.com/MaximIntegrated/max32625pico-firmware-images/raw/master/bin/max32625_max32666fthr_if_crc_swd_v1.0.5_pico2.bin)  | dd439e | :heavy_check_mark: |

## Details SHA
This SHA helps the user to identify the current version of the firmware loaded on the board. Open the DETAILS.TXT file in the DAPLINK drive and match the Git SHA field.
</br>This is not the SHA of the binary file.

## MAX32625PICO Board
![MAX32625PICO Board](/max32625pico_maxdap.png)

## MAX32625PICO2 (Bootloader Programmer) Board
Bootloader Programmer PICO provide standart PICO functionality plus bootloader programmer interface.
More detail about bootloader programmer board [Bootloader Programmer UG](https://pdfserv.maximintegrated.com/en/an/ug7510-maxim-bootloader-tools.pdf)
![MAX32625PICO2 Board](/max32625pico2_maxdap.png)

## SWD/DIP Interfaces
There are [two debug interfaces in MAX32625 DAPLink FW](https://github.com/MaximIntegrated/DAPLink/blob/main/source/hic_hal/maxim/max32625/IO_Config.h#L97). 
It is called as SWD and DIP interface. The MAX32625 DAPLink fw is generated to support one of these interface.
The _swd_ or _dip_ addition in image file name indicates debug interface configuration. [The pin connection SWD and DIP interface](https://github.com/MaximIntegrated/DAPLink/blob/main/source/hic_hal/maxim/max32625/IO_Config.h#L68) listed in below table.

| PIN Name | SWD  | DIP  |
|--|--|--|
| Reset    | P3.7 | P0.4 |
| SWDCLK   | P3.2 | P0.2 |
| SWDIO    | P3.3 | P0.3 |
| UART TX  | P2.0 | P0.0 |
| UART RX  | P2.1 | P0.1 |

## What about the targets not listed above?
The factory default firmware, i.e. MAX32630FTHR binary can program all the targets via the HID CMSIS-DAP debugging/programming interface.
</br>Only the MSD Drag-n-Drop programming is target-specific.

## How to update the firmware?
Just like most DAPLink interfaces, the MAX32625PICO board comes pre-installed with a bootloader that enables driverless drag-n-drop updates. 
This bootloader can be used to update or restore the DAPLink firmware on the MAX32625PICO board or it can also be used to load your own custom application on the board. 
This allows you to use the MAX32625PICO board as a tiny, embeddable development platform. 
To activate the bootloader: 
1. Simply hold the lone button down while applying power to the board. When the bootloader detects the button press at power on, it will connect to the PC as a drive named "MAINTENANCE". 
2. Simply Drag-n-Drop the desired image onto the MAINTENANCE drive to load new firmware into the board.

## How to erase the target flash?
1. Unplug the target board and the MAX32625PICO debug adapter.
2. Connect the target board to a power source, then connect the MAX32625PICO debug adapter to the host machine.
3. Open the DETAILS.TXT file on the DAPLINK mass storage drive and verify Automation Allowed is set to 1.
   * How to enable [Automation](https://github.com/ARMmbed/DAPLink/blob/master/docs/ENABLE_AUTOMATION.md)?
4. Create an empty file - 'erase.act' on the host machine and Drag-n-Drop (copy-and-paste) it on to the DAPLINK drive.
5. This should erase the target's flash memory. The DAPLINK drive will disconnect and reconnect completing the operation.

### License
The software is provided under the [Apache-2.0 license](LICENSE.txt). 
Contributions to this project are accepted under the same license.
