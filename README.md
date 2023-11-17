# Squid TX12 Emulator

This is a fork of the # ELRSJoystick / CRSFJoystick 

The original version identifies over USB as a Joystick and not as a game pad,this creates a problem with simulators as Realflight and Aerofly RC8. 

the version in this fork will identify as a Gamepad and will map the buttons to the ELRS channels as follows:



#Channel mappings

(Mode2)  

| TX12 | Channel | PC  | Info              |
|------|---------|-----|-------------------|
| X    | CH1     | X   | Ail (Analog)      |
| Y    | CH2     | Y   | Ele (Analog)      |
| Z    | CH3     | Z   | Thr (Analog)      |
| Xr   | CH4     | Xr  | Rud (Analog)      |
| S1   | CH6     | Yr  | slider1 (Analog)  |
| S2   | CH7     | Zr  | slider2 (Analog)  |
| SA   | CH8     | B1  | 2 states          |
| SB   | CH9     | SB  | 3 states          |
| SC   | CH10    | SC  | 3 states          |
| SD   | CH11    | B2  | 2 states          |
| SE   | CH5     | B3  | 2 states          |
| SF   | CH12    | B4  | 2 states          |






Installation 

* copy Sketchbook directory to your PC 
* Open sketchbook/crsf_Joystick with Arduino IDE
* Change the directory in file->preferences to the sketchbook directory
* Make sure the Squid in connected to USB 
* Change the port to the Squid com port
* Compile and upload 
* In TX12 set ELRS to 333Hz ,telemetry off ,Switch mode 16ch rate/2


Configuration

* make sure that you define the channels as in the table above
* if needed , open "Set up USB game controllers" in windows to test and clibrate 
* calibrate! and make sure to do so without trim. once clibrated , you can use trim as needed




















Shout out to CapnBry for the Crsf Library

https://github.com/CapnBry/CRServoF

Shout out to RealRobots.net for the Gamepad Library

https://gitlab.com/realrobots/PicoGamepad/-/tree/master


