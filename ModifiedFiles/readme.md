This folder contains all the modified or added files in the qf_ssi_ai_app project directory for the Forestation Assistance Kit project. 

Here is a list of the all the modified files with their intended location in the project folder and the modified line numbers.
1. `Adafruit_ADS1015.cpp` : Location - `qf_ssi_ai_app/src`; Modified Lines - 30-36,45-59,69,71-73,84,86-88; Reason for Mod - Removal of dependency on Arduino Library and adding millis() and delay() functions
2. `qf_hardwaresetup.c` : Location - `qf_ssi_ai_app/src`; Modified Lines - 103; Reason for Mod - Bring down the Baudrate from 460800 for Data Recognition phase
3. `app_config.h` : Location - `qf_ssi_ai_app/inc`; Modified Lines - 24,25; Reason for Mod - For switching the project between Data Capture and Data Recognition phases
4. `sensor_ssss.cpp` :  Location - `qf_ssi_ai_app/src`; Modified Lines - 36,38,59,61,69-76,92-104,126-145; Reason for Mod - The original IMU code sections are replaced by Adafruit's ADS1015 ADC's working code.

These files can be replaced within your own project file as it is if you want to work on Data Recognition Mode. For working on Data Capture Mode, make change in `app_config.h` file.
You will have to switch the 0 and 1 in lines 24 and 25.
