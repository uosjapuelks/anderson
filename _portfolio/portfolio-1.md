---
title: "CG4002 Capstone Laser Tag - Artificial Intelligence Component"
excerpt: "An Augmented Reality laser tag game that has a gesture recognition system to detect actions as commands in the AR game. <br /> ![CG4002 Capstone](../images/CG4002Group.png) <br /> [__CLICK TO KNOW MORE__](https://uosjapuelks.github.io/anderson/portfolio/portfolio-1/)"
collection: portfolio
---

---
## Github
[Click Here to Checkout the repository](https://github.com/uosjapuelks/capstoneml)

***
### CG4002 Augmented Reaility Laser Tag

* [Watch the Final Game Demo!](https://www.youtube.com/watch?v=ZkmZPc9GfTc&ab_channel=HoMingJun)
* [Download Report!](http://uosjapuelks.github.io/anderson/files/CG4002Report.pdf)

A project tasked to us in CG4002 Capstone Project for Computer Engineering Undergraduates.

This laser tag allows for gestures to be input as action commands such as shield, throwing a grenade, or reload the guns.

I was in charge of deploying Machine Learning models, extracting the weights to program the FPGA accelerator and integrating them into the game engine. I also undertook the responsibility of ensuring correct messages being sent to the Evaluation server while not compromising gameplay by taking up the role to debug and program the game engine component as well.

The game was made using python, where communication with server, and relay laptops utilized TCP/IP, AI made use of an accelerator attached to Ultra96 programmed with trained weights from data collected from all 5 members, along with a game engine running on Ultra96 to send game states to an Evaluation server to be verified for correctness and latency. 
Our project proved to be very, if not the most generalisable out of all teams, being able to predict 39 out of 40 actions right by the final demo where random players outside our team were chosen as players.

[Click here to find out more!](https://github.com/uosjapuelks/capstoneml)

***
### External Communications Component (inclusive of Game Engine Component)
[Click here to check out the External Communications Component](https://github.com/huien77/CG4002_ext_comm).
