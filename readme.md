Language: [English](readme.md) | [Українська](readme.uk.md) | [Deutsch](readme.de.md)


### How to update?
1. Copy the apiary.bin file to the device micro sd-flash into the /fm folder (if it does not exist - create it)
2. Return the sd-flash to the device and reboot it
3. Wait 1-2 minutes until the device turns itself off (until the LEDs calm down)
4. Reboot, reconnect, and check the new software version on the main page (what to compare with is below)
   
### Languages: Selected by changing the firmware  

  - English: [En](build-en/apiary.bin)

  - Українська (Ukrainian): [Uk](build-uk/apiary.bin) 

  - Polski (Polish): [Pl](build-pl/apiary.bin)

  - Deutsch (German):  [De](build-de/apiary.bin)

  - Español (Spanish): [Es](build-es/apiary.bin)

  - Français (French): [Fr](build-fr/apiary.bin)   
    

  Translation can be ordered *(conditionally free)
   
The rest of the versions can be checked by date, the hash (digits after the date) may differ between localizations

### Youtube instruction here: https://www.youtube.com/@BeeApiary 
### Actual

- build-de version : 4.0.fb14e16-de

- build-en version : 4.0.fb14e16-en

- build-es version : 4.0.fb14e16-es

- build-fr version : 4.0.fb14e16-fr

- build-pl version : 4.0.fb14e16-pl

- build-uk version : 4.0.fb14e16-uk

  Devices can now operate via local Wi-Fi without a SIM card
  
### The Web interface looks like this:
![Screenshot](./images/S1.jpg)  ![Screenshot](./images/S2.jpg)  ![Screenshot](./images/S4.jpg)  ![Screenshot](./images/S3.jpg)

### Sincere thanks to UI/UX designer Oleksandr Yatsiuk for very cool and professional help in developing the design under difficult Embedded conditions of a small device.

### Basic direction of the device, or strategy, or the lack of it )))
To create a protected (outdoor) measuring device for an apiary that would not require physical intervention, meaning it should be opened only once to install the SIM card. Measurements and device settings are available through the Web interface, without requiring the device to be connected to the internet. If necessary, log files and measurement files can be retrieved from the device using Wi-Fi, which is also easy to do without interfering with the device, reducing the risk of damage caused by weather conditions and increasing its service life.
Measurements are automatically transferred directly to the Android device without being stored on a server or in the cloud. If synchronization is needed, the device can use internet access, but only at the user’s own request. This excludes the collection of information, even technical information, for the benefit of third parties. At this stage, synchronization issues are considered additional and do not affect the main functions of the device.

Previous changes

3.1.f114152(Feb 21 2026 20:11:44)53d98c5f0be40b1e 
  - update for support of short 10-symbol numbers (Norway)
  - support for 10-12 symbol numbers expanded


3.1.891d578(Dec 23 2025 23:41:54)6dd3be766d6cdbe2
  - automatic disconnection from wi-fi during a long connection (battery saving in case of a forgotten connection or automatic connection by Android devices)

3.1.5f89a8c(Nov 10 2025 23:09:31)6cc291686bfd9b62
  - ability to swap T1 and T2 using the temperature_twist ="true" setting

3.1.67a4190(Aug 27 2025 21:37:53)e5da30ebfde9e0ca
  - support for board version 1.3 
  - power consumption reduced, works up to half a year on one char

3.1.5f89a8c(Nov 10 2025 23:09:31)6cc291686bfd9b62
  - ability to swap T1 and T2 using the temperature_twist ="true" setting

3.1.67a4190(Aug 27 2025 21:37:53)e5da30ebfde9e0ca
  - support for board version 1.3 
  - power consumption reduced, works up to half a year on one charge 

3.1.c43b227(Jun  7 2025 21:19:08)f8d5376299daf03c
  - device ID added to the main Web page
  - filter control fixed  

3.1.a166b4b(May 29 2025 02:10:59)6b2d72175a18f4eb
  - additional functions for handling errors from the GSM modem added
  - preparation for the new release of the main board
  - device number added to logs
  - filter control fixed

3.1.a9d1231(May  8 2025 00:40:27)52889ef7f9993255
  - minor fixes in the SMS format "For a human"
  - calculation of the daily difference for these SMS changed

3.1.a9b4fce(Apr 13 2025 13:25:24)081f88e5712295e4
  - minor logging fixes (does not affect operation)

3.1.65cc3fc(Mar 14 2025 19:18:21)e07791fb1ddc4e03
  - ability to enter European Union numbers added

3.1.6ca7c59(Feb 18 2025 00:26:28)0956163f27ccf77f

- fixed operation with 18b20 sensors at low temperatures

 3.1.99143ea(Feb 16 2025 21:18:35)f446b9c0068a7f9d 

- fixed indication during direct connection (blinks when the phone is connected)
- fixed repeated connection issue
- also websocket synchronization issue 


3.1.f046c00(Nov 2 2024 13:14:52)3d62778de6ff0162

- increased optimization of messages and files (more data in one message)
- Device identifier added, possibility of integration with the new APK interface
- additional functions for parameter control added
- possible functions for more frequent measurement control 
- critical temperature functions added, at which an emergency message will be sent (Engineering manual) 

3.0.7c59145(Oct 10 2024 18:45:57)3b43dff7d46a649b
 - Added the ability for current weighing "on the roof"
 - Or weighing during inspection of the control hive

 3.0.2697b84(Oct 1 2024 13:57:31)d46406efcf49f828
  - Support for a larger 128x64 screen added to the existing 128x32
  - Image rotation option added

3.0.a7a0827(Sep 22 2024 12:12:29)a7377298cc60a196

  - The interface, approach, and appearance have been significantly changed.

2.7.02cdf8b(Sep  5 2024 16:55:22)485d2d57161f187e

2.7.9479439(Aug 26 2024 22:29:53)130bc5fbe1f3d377

2.7.9c484d4(Aug 19 2024 20:13:50)142ce826ee914278 

2.7.ae17c33 (Aug 18 2024 20:55:28) f73077b0b6a6b979 

194467f (Jun 23 2024 11:46:59) 1898e70afeacb758
 - The work on Direct Download Data has been completed (User can download mesurement directly device <-> Android)
 - Power consumption optimized 1 sms per day = 6 month uncharged work, without sim(collect data to flash) aproximetly 1 Year without charging
 - measurement accuracy increased
 - Gsm signal strength added
 - Two Sms types added to Web UI

8d8cb3a (Jun 17 2024 23:14:02) 647f31fc2a027e98
 - web schedule page has been added

a89838c (Jun 12 2024 01:09:23) 78d8106a5e5fdd95
 - power consumption optimization

a46daa3 (Jun 10 2024 11:19:11) 23e60215f2eea156
 - sms compression update

8c14c33 (Jun  9 2024 15:47:59) ff42dcffc0af9f9e
  - main cleanup

f81c157 (Jun  5 2024 22:07:10) 1c4b5224fd72bbaf
 - the calibration algorithm has been significantly redesigned

75b5698 (Jun  2 2024 20:39:21) 88d0b240ed6b37f7
 - reworked measurement filtration

de855fa (May 30 2024 22:33:57) 5b21a4d92a523e03
 - log cleanup for previous build

b4bb02f (May 30 2024 12:23:10) db7d03899421ca68
 - GSM parser updated

d9e51a0(May 28 2024 23:01:14) aeed24708b394fbe
- additional logic when sending SMS 
- additional conditions for GSM reinitialization at a poor signal level
- charge indicator correction

fe703d2(May 14 2024 22:41:45) 781726e08db3d1ca
- Power saving additionally optimized
- Oled added 
- Security mode control
- Work with Pir updated
- Work started in the Direct Download Data direction
