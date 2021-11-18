---
title: "EE2026 Digital Design Mini Project"
excerpt: "A mini-game system on an FPGA Board - Basys 3 Board programmed using verilog code. ![Basys3 Board](../images/BoardIntro.jpg)"
collection: portfolio
---

# Github

# FPGA Design Project: Sight and Sound Entertainment System

## User Guide

|Feature|Input Devices|Feature Description|Images/Photos|
|---|---|---|---|
|Real-time audio volume indicator|SW0,<br /> SW1|__SW0 IS 0:__ mic_in shown on 12 LEDs <br /> __SW0 is 1:__ Peak intensity shown on 15 LEDs (0 level does not show anything) <br /> __SW1  is 0:__ sound level in didgit shown on the anode <br /> __ SW1 is 1:__ sound level in letter is shown on the anode (5 level for each level, 0 level is still 0|![](../images/2026_7SegtVol_0.png) ![](../images/2026_7SegtVol_1.png)|
|Totoro bus stop |Mic|4 levels of rain according to mic input: <br /> __level 0:__ no rain <br /> __level 1 - 5:__ slightly animated raining, slow rain falling speed <br /> __level 6-10:__ moderate animated raining, moderate rain falling speed <br /> __level 11 - 15:__ heavy animated raining, fast rain falling speed|![](../images/2026Rain.png)|
|Menu|SW8, btnU, btnD, btnC|__SW8 is 0:__ shown the individual tasks<br />__SW8 is 1:__ shown the menu<br />__btnU:__ move selection up by 1<br />__btnD:__ move selection down by 1<br />__btnC:__ go into the mode of choice|![](../images/2026_mode1.png) ![](../images/2026_mode2.png) ![](../images/2026_mode3.png) |
|Graphical Visualisations and configurations|SW15,<br /> SW14,<br />SW13,<br />SW12,<br />SW11,<br />btnL,<br />btnR,<br />Mic|__SW15,SW14:__ 3 pixel thick border if 2’b10,1 pixel thick border if 2’b01<br />__SW13:__ Force Border off<br />__SW12 is 1:__ Switches on alternate colour scheme<br />__SW12 is 0:__ Switches off alternate colour<br />__SW11 is 1:__ Switches off/hide volume bar while keeping the borders and background colour the same according to the other switches<br />__Mic:__ There is a volume bar with the samenumber of level as the volume level.<br />__btnL:__ Volume bar shifts left by 1 pixel<br />__btnR:__ Volume bar shifts right by 1 pixel|![](../images/2026_OledVol.png)![](../images/2026_OledVol2.png)![](../images/2026_OledVol3.png)![](../images/2026_OledVol4.png)![](../images/2026_OledVol5.png)![](../images/2026_OledVol6.png)![](../images/2026_OledVol7.png)![](../images/2026_OledVol8.png)![](../images/2026_OledVol9.png)|
|Run Barry Run!!|Mic|__Level 0:__ Lowest frame rate<br />__Level 1-5:__ Slow frame rate shows slow run<br />__Level 6-10:__ Faster frame rate for faster running<br />__Level 11-15:__ Even Faster frame with 15 being the highest and the fastest run.|![](../images/2026_barry.png)|
|Volume level indicator in "Run Barry Run!!"|Mic|Horizontal Volume bar to allow visibility of Barry and indicates the current volume level input to user|![](../images/2026_barry2.png)|
|Ghost|btnU, <br /> btnD, <br />btnL, <br />btnR|__btnU:__ Ghost moves up<br />__btnD:__ Ghost moves down<br />__btnL:__ Ghost moves left and start rotating leftwards<br />__btnR:__ Ghost moves right and start rotating rightwards|![](../images/2026_ghost.png)|
|Man| |Man spawn to the left of the screen. Animated to run rightward When the ghost is __above__ and __behind__ him, and the __wave touches his ear__, man turns into a tombstone. When the man runs off the screen, the screen turns into the gameover screen.|![](../images/2026_man.png)|
|Wave|Mic|__Level X:__ Sound wave emitted from ghost with radius X|![](../images/2026_sound.png) ![](../images/2026_sound1.png)|
|Tombstone| |Tombstone spawn and __stays still__ for around __2 - 3 seconds__ before despawning and Man starts running from the left of screen rightwards.|![](../images/2026_tombstone.png)|
|Score| |On the __upper right corner__ of the screen, whenever the man respawns from the grave, a point is added.| |
|Game over Screen| |Gameover screen with the total score displayed when the man __runs off__ the screen or the score is __99__.|![](../images/2026_gameover.png) ![](../images/2026_gameover1.png)|
|reset|SW7, SW9|__SW7 is 1:__ Game score Resets to 00, returns to __Main Menu__. (Blocks entry into games)<br />__SW7 is 0:__ Allow selection of the Games<br />__SW9 is 1:__ Resets score to __00__. Position of Man will hover at spawn point at the __bottom left__, Position of Ghost hovers at __top left__<br />__SW9 is 0:__ Game __starts__, Man starts moving right, ghost is able to move according to button press.| |
