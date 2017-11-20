HD8089 SDK
=====

## Binary files
* DR over CAN configuration
  * firmware + boot code
```FWConfig.exe -f sta8090_gnssapp_dr_soc_sqi_sqi_fr_gae_BOOT.bin -c hd8089_DR.txt -o hd8089_BOOT_DR.bin```
  * firmware
```FWConfig.exe -f sta8090_gnssapp_dr_soc_sqi_sqi_fr_gae_UPG.bin -c hd8089_DR.txt -o hd8089_UPG_DR.bin```
* DR over ODO configuration
  * firmware + boot code
```FWConfig.exe -f sta8090_gnssapp_dr_soc_sqi_sqi_fr_gae_BOOT.bin -c hd8089_ODO_DR.txt -o hd8089_BOOT_ODO_DR.bin```
  * firmware
```FWConfig.exe -f sta8090_gnssapp_dr_soc_sqi_sqi_fr_gae_UPG.bin -c hd8089_ODO_DR.txt -o hd8089_UPG_ODO_DR.bin```

## CAN Demo App
For debugging CAN bus communication. I used two devices for sending and receving data over CAN.
Use project gnssapp_demo_freertos_gae changed makefile for being CAN TX or CAN RX.
* CAN TX
  * Makefile ```EXT_CDEFS=EXAMPLE_CAN EXAMPLE_CAN_TX ```
* CAN RX
  * Makefile ```EXT_CDEFS=EXAMPLE_CAN EXAMPLE_CAN_RX```
* firmware + boot code
```FWConfig.exe -f sta8090_gnssapp_demo_soc_sqi_sqi_fr_gae_BOOT.bin -c hd8089.txt -o hd8089_CAN*.bin```

## SDK zip files
* HD8089_gnssapp_demo_CAN.zip
  * HD8089 CAN TX/RX demo app
* HD8089_gnssapp_SM130_1110.zip
  * HD8089 SDK for supporting CAN/DWP
* HD8089_gnssapp_SM130.zip
  * HD8089 SDK for supporting Gyro/Acc BOSCH SMI130

