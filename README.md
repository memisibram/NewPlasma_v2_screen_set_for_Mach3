# NewPlasma v2 Mach3 Plasma screen 
Version 2 of the NewPlasma display set for use with Mach3 plasma machines.

### What's new
  - Probe triggering for floating head will be done with Mach3 instead of G codes (m3 and m5 macros have been created for this)
  - Many operations such as G31 reference search, swich offset, pierce height, pierce time, cutt height are done from mach3 main screen.
  - Finding m3 in G code feature, you will be able to search m3 code after / before the current line
  - Jog Rate scroll bar added to home page

 - Video: https://youtu.be/4WrAb9kqNBs

#### G code example
- G21 (Units: Metric)
- F1
- G53 G90 G40 G91.1
- G00 X51.5500 Y51.0000
- M03
- G03 X51.0000 Y51.5500 I-0.5500 J0.0000 F1000.0
- G01 X1.0000 F2000.0
- G03 X0.4500 Y51.0000 I0.0000 J-0.5500 F1000.0
- G01 Y1.0000 F2000.0
- G03 X1.0000 Y0.4500 I0.5500 J0.0000 F1000.0
- G01 X51.0000 F2000.0
- G03 X51.5500 Y1.0000 I0.0000 J0.5500 F1000.0
- G01 Y51.0000 F2000.0
- M05
- M05 M30

Post processor file for generating code in the desired format if you are using the SheetCam programme: [Mach3 Plasma THC on off no Z.scpost](https://github.com/memisibram/NewPlasma_v2_set_for_Mach3/tree/main/SheetCam%20%20Post%20processor)
- Sheetcam tool setup

![](https://github.com/memisibram/NewPlasma_v2_set_for_Mach3/blob/main/sheetcamtoolset.png)

#### Images
![](https://github.com/memisibram/NewPlasma_v2_set_for_Mach3/blob/main/Bitmaps/NewPlasma/PlasmaMain.jpg)
![](https://github.com/memisibram/NewPlasma_v2_set_for_Mach3/blob/main/Bitmaps/NewPlasma/PlasmaMainFull.jpg)
![](https://github.com/memisibram/NewPlasma_v2_set_for_Mach3/blob/main/Bitmaps/NewPlasma/bg_angle_fin.jpg)

### License GNU GPL v3.0

### Donation

Maybe you'd like to donate for a coffee
  -  Paypal: memisibram@gmail.com or 
https://www.paypal.me/memisibram
