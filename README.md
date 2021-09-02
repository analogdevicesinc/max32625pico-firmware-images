# MAX32625PICO FIRMWARE IMAGES
DAPLink firmware images for MAX325PICO board

## Latest Releases
| Drag-n-Drop Target | Binary | Details SHA  | Erase support |
|--|--|--|--|
| MAX78000FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max78000fthr_if_crc_v1.0.2.bin)  | a209a92 | :heavy_check_mark: |
| MAX32630FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_daplink_factory_default_v3.bin)  | aab4d91 | :heavy_check_mark: |
| MAX32666FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max32666fthr_if_crc_v1.bin)      | 19edd04 | :heavy_check_mark: |
| MAX32665HSP3 | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max32665hsp_if_crc.bin )         | d7b5231 | :x: |
| MAX32620FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max32620fthr_if_crc.bin )        | f499eb6 | :x: |
| MAX32625PICO | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_max32625pico.bin )               | 84e3053 | :x: |
| MAX32630HSP2 | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_max32630hsp.bin )            | 84e3053 | :x: |
| MAX32660 | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_max32660_vio_in.bin )            | 84e3053 | :x: |
| MAX32660 | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_max32660_power_out.bin ):warning:| fd4512f | :x: |

:warning: This image will apply 3.3V to the VIO pin of the MAXDAP connector allowing the MAX32625PICO board to power the MAX32660 Evaluation Kit. It may permanently damage other incompatible target boards.

## Previous Releases
| Drag-n-Drop Target | Binary | Details SHA  | Erase support |
|--|--|--|--|
| MAX32630FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_daplink.bin)                 | 5d2ab47 | :x: |
| MAX32630FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max32630fthr_if_crc.bin)         | f499eb6 | :x: |

## Details SHA
This SHA helps the user to identify the current version of the firmware loaded on the board. Open the DETAILS.TXT file in the DAPLINK drive and match the Git SHA field.
</br>This is not the SHA of the binary file.

## MAX32625PICO Board
![MAX32625PICO Board](/max32625pico_maxdap.png)

## What about the targets not listed above?
The factory default firmware, i.e. MAX32630FTHR binary can program all the targets via the HID CMSIS-DAP debugging/programming interface.
</br>Only the MSD Drag-n-Drop programming is target-specific.

## How to update the firmware?
Just like most DAPLink interfaces, the MAX32625PICO board comes pre-installed with a bootloader that enables driverless drag-n-drop updates. This bootloader can be used to update or restore the DAPLink firmware on the MAX32625PICO board or it can also be used to load your own custom application on the board. This allows you to use the MAX32625PICO board as a tiny, embeddable development platform. To activate the bootloader, simply hold the lone button down while applying power to the board. When the bootloader detects the button press at power on, it will connect to the PC as a drive named "MAINTENANCE". Simply Drag-n-Drop the desired image onto the MAINTENANCE drive to load new firmware into the board.

## How to erase the target flash?
1. Unplug the target board and the MAX32625PICO debug adapter.
2. Connect the target board to a power source, then connect the MAX32625PICO debug adapter to the host machine.
3. Open the DETAILS.TXT file on the DAPLINK mass storage drive and verify Automation Allowed is set to 1.
   * How to enable [Automation](https://github.com/ARMmbed/DAPLink/blob/master/docs/ENABLE_AUTOMATION.md)?
4. Create an empty file - 'erase.act' on the host machine and Drag-n-Drop (copy-and-paste) it on to the DAPLINK drive.
5. This should erase the target's flash memory. The DAPLINK drive will disconnect and reconnect completing the operation.
