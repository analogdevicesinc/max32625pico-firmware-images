# MAX32625PICO FIRMWARE IMAGES
DAPLink firmware images for MAX325PICO board


## Latest Releases
| Drag-n-Drop Target | Binary | Erase support |
|--------|--------|---------------|
| MAX78000FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max78000fthr_if_crc_v1.0.2.bin) | :heavy_check_mark: |
| MAX32630FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_daplink_factory_default_v3.bin) | :heavy_check_mark: |
| MAX32666FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625_max32666fthr_if_crc_v1.bin) | :heavy_check_mark: |

## Previous Releases
| Drag-n-Drop Target | Binary | Erase support |
|--------|--------|---------------|
| MAX32630FTHR | [Download](https://github.com/MaximIntegratedMicros/max32625pico-firmware-images/raw/main/bin/max32625pico_daplink.bin) | :x: |

## How to erase target flash?
1. Unplug the target board and the MAX32625PICO debug adapter.
2. Connect the target board to a power source, then connect the MAX32625PICO debug adapter to the host machine.
3. Open the DETAILS.TXT file on the DAPLINK mass storage drive and verify Automation Allowed is set to 1.
   * How to enable [Automation](https://github.com/ARMmbed/DAPLink/blob/master/docs/ENABLE_AUTOMATION.md)?
4. Create an empty file - 'erase.act' on the host machine and Drag-n-Drop (copy-and-paste) it on to the DAPLINK drive.
6. This should erase the target's flash memory. The DAPLINK drive will disconnect and reconnect completing the operation.