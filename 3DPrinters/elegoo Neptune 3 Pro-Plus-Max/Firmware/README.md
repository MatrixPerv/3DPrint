# elegoo Neptune 3 Pro Firmware
Repository for elegoo Neptune 3 Pro Firmware Files

---

- Reminder: This page is constantly being updated, and the information may be incomplete or inaccurate. Please continue to pay attention, thank you!

---
# **_Neptune3Pro/Plus/Max Firmware Update Instructions_**

### Firmware Version Compatibility:
| Screen Version | Motherboard Version | Description |
|------------|-------------------------------------|------------|
| 1.4       |      1.x.4 - 1.x.5.1a          |   Version History      |
| V1.4.1       |      1.x.5.1a          |   Release version  |
| 1.5-Beta  |      1.x.5.2 - 1.x.5.3a           |  Beta version   |

[Update Log](https://github.com/NARUTOfzr/Neptune_3_Pro_Plus_Max/blob/main/Update%20log.md)

---    
### File Description:

| Firmware naming method| |
|------------|------------------------------------ -|
| xxxxxxxx.tft | Screen Firmware |
| ZNP_ROBIN_NANO.bin | Motherboard Firmware |

   

---    
### Preparation steps:    
1. Format the TF card as shown in the figure.      
    Requirements: Filesystem (F): `FAT32`      
![Enter picture description](Pic/image1.png)      

2. As shown in the figure, copy the above two firmware files to the root directory of the TF card.    
![Enter picture description](Pic/image3.png)

---  
### Screen firmware update steps:    
1. Loosen the screws, remove the back cover of the screen; pay attention to the direction of the card insertion, and insert the TF card.      
![Enter picture description](Pic/image4.png)  

2. Restart the power supply and wait for the firmware to be loaded. The firmware loading process and the completed interface display are shown in the figure. After the loading is complete, remove the TF card and restart the machine. (Time required for screen firmware update: about 60 seconds)  
![Enter picture description](Pic/image5-2.png)


---  
### Mainboard firmware update steps:    
Insert the TF card into the machine, then restart the power supply, and wait for the firmware loading to complete; the screen display during the firmware loading process is as shown, and it will directly enter the main interface after the firmware update is completed. (Mainboard firmware update time: about 15 seconds. If you can’t enter the main interface for a long time, just format the TF card and reload the firmware.)  
![Enter picture description](Pic/image6.png)


---  
# **_`FAQ: `_**
1. What is the compatibility relationship between screen firmware and motherboard firmware?
The screen firmware of Neptune3Pro/Plus/Max machines is common, and the motherboard firmware also uses the same source code. Please update the corresponding firmware file according to your machine model. Motherboard firmware naming method:    
Neptune3Pro: 1.1.xx    
Neptune3Plus:1.2.xx   
Neptune3Max:1.3.xx    
Please check [Update Log](https://github.com/NARUTOfzr/Neptune_3_Pro_Plus_Max/blob/main/Update%20log.md) for the compatibility relationship and update content between different versions of screen firmware and motherboard firmware.

2. After turning on the power, the interface "Update firmware..." will always be displayed, as shown in the figure.    
![Enter picture description](Pic/image6-1.png)    
Reason: After turning on the power for a period of time, if the display does not receive the signal from the main board, it will jump to this interface, and it will not start until it receives the signal from the main board.    
Root cause and workaround:    
 :point_right: 1) It may be a bug in the historical firmware, it is recommended to check and update the motherboard firmware to `1.x.5.1a`.    

 :point_right: 2) It may be that the connecting wire between the motherboard and the display screen is not in good contact (poor contact of the signal wire), it is recommended to plug the connecting wire tightly and then restart.    
    
3. The screen firmware will not be renamed after loading, and can be loaded repeatedly, so the TF card must be removed after updating the screen firmware; after the motherboard firmware is successfully loaded, it will be renamed to `“ZNP_ROBIN_NANO. to load.  
![Enter picture description](Pic/image7.png)

4. If you disconnect the power or remove the TF card before the screen firmware is loaded, you will not be able to enter the main operation interface after restarting the power, as shown below:  
![Enter picture description](Pic/image7-1.png)

5. You can check the UI version and motherboard firmware version in [Settings] → [Information].  
![Enter picture description](Pic/image7-3.png)

6. After reloading the mainboard firmware, the leveling value will be cleared and needs to be rebalanced.  

7. After the screen is powered off and restored, some information will be lost (for example, the firmware version number is lost, and the thumbnails during printing are not displayed), which is a normal phenomenon and will not affect normal printing. It can be displayed after restarting the machine.    

8. As shown in the picture, when upgrading the screen firmware, it will display 'Multiple `TFT` files' and then directly enter the main interface.    
![Enter picture description](Pic/image8-1.png)    
Reason: Some MacBooks of the macOS system will generate files with the same name prefixed with "![Input picture description](Pic/image9-1.png)" when copying firmware or other files, which cannot be viewed on MacBooks, but other systems It can be seen that this is the main reason for the failure of updating the screen firmware. as the picture shows:    
![Enter picture description](Pic/image9-2.png)     
The solution to the file with the same name prefixed with "![Input picture description](Pic/image9-1.png)" when copying on MacBook: :point_right: 1) Move the required file to the USB disk. :point_right: 2) Open "Terminal". :point_right: 3) Enter dot_clean followed by a space, and then drag the U disk icon into the terminal interface. :point_right: 4) Press Enter and exit the U disk to delete the file with the same name prefixed with “![Input picture description](Pic/image9-1.png)”.    
The solution is as shown in the video: [bilibili video tutorial](https://www.bilibili.com/video/BV1Lv4y1C7Qz/?share_source=copy_web&vd_source=39af2b2e9e60f33607226e91f3f17001) [YouTube video tutorial](https://youtu.be /mdb4PTPlJh4)    

9. When upgrading the screen firmware, an error in the picture is displayed.    
![Enter picture description](Pic/image8-2.png)   
Cause: The screen firmware file is corrupted.     
Solution:    
     :point_right: 1) Format the TF card.    
     :point_right: 2) Re-download the file or contact the after-sales personnel to obtain the screen firmware file and re-update the firmware.    
     :point_right: 3) Try to use the processing method in question 8 to deal with it.   
