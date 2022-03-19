# DIY-mini-PCB-based-handheld-retro-game-console


![image](https://user-images.githubusercontent.com/19898602/127040498-c9511f25-f3ac-4ae9-acc6-b78cbb7ec141.png)

Hello friends in this post we’ll se how easily we can build a Attiny based mini game console.

In this mini game console you can play some retro games, which is obviously not very high tech but yes you get a good experience of making your own game console.

So in post I’ll tell you in detail how to can build you game console what components you need and how to program Attiny 85 microcontroller.

# Components required for Attiny based mini game console

Here is the list of component you need to build your Attiny 85 based game console.

> Attiny 85 microcontroller


> 10K Ohm x 2


> 6.8K Ohm resistor x 1


> 1K Ohm resistor x 1


> LED 5MM x 1


> 6mm tactile PB X 3


> 0.96 Oled display( gnd,vcc,scl,sda) x 1


> slide switch x 1


> CR2032 battery x 1


> CR2032 battery holder x 1


>3V Buzzer x 1

# For uploading code to Attiny 85

> Any arduino board ( I am using Arduino UNO)


> Data cable


> Some jumper wires

![image](https://user-images.githubusercontent.com/19898602/127040766-c2110692-6ac2-49d2-b7ff-a4403095ae25.png)

# Circuit Diagram

![image](https://user-images.githubusercontent.com/19898602/127041030-bed8d207-1820-4d24-bc99-da1867c57900.png)



# PCB of mini game console from [JLCPCB](https://jlcpcb.com/IAT )

![image](https://user-images.githubusercontent.com/19898602/127040832-fa3ad471-223b-4948-891e-cac4810f2e7f.png)

![image](https://user-images.githubusercontent.com/19898602/159103396-b67962d3-384a-4d3c-8d14-0d580f2c6184.png)

![image](https://user-images.githubusercontent.com/19898602/159103446-b099ea39-b90c-493c-9465-6e19e7c31789.png)




![image](https://user-images.githubusercontent.com/19898602/127042314-3a4e48e0-f253-4707-8d08-9b5a3cf2eec6.png)

![image](https://user-images.githubusercontent.com/19898602/127042452-9191dbf3-41fd-465a-9bea-f8759a0e3f4d.png)

![image](https://user-images.githubusercontent.com/19898602/159103503-59c54cc5-0fdc-48e1-85e6-1ff641e9b61d.png)


My first aim in this project to keep it small as much as possible so decide to go with SMD components, so that Electronics component cover minimum space on PCB

So I design PCB accordingly now I am much excited to order this PCB and I choose [JLCPCB](https://jlcpcb.com/IAT )

I got my PCB in a week only though it was a international shipment, I was quite satisfied with the PCB quality, 

I also ordered Stencil along with PCB and thanks to [JLCPCB](https://jlcpcb.com/IAT ) both of this are not much havey on my pocket they have very reasonable price.

if you are trying prototype PCB first time you can definitely go with [JLCPCB](https://jlcpcb.com/IAT ).


 👉 Try PCBA service of [JLCPCB.com](https://jlcpcb.com/IAT) and save your time and money, get PCB ready for project, 200K+ components in library of [JLCPCB.com](https://jlcpcb.com/IAT) as well as 3rd party         parts to choose from. 
    Assembly will support 10M+ parts from Digikey, mouser
    
👉 $27 valued New User coupons 

👉 $24 SMT coupons every month




If you want to see complete process of SMD soldering, go to the link below it was very satisfying to watch

https://www.youtube.com/watch?v=iG4kTLOWU5Y&t=14s

# Brief intro about Attiny 85

Attiny 85 is a tiny 8 bit Microcontroller which is high performance and low power.

Attiny 85 is 8 PIN microcontroller, most of its I/O pins are multifunctional. if you are familiar with arduino borads like NANO, UNO or MEGA, you can easily relate Attiny 85 with them.

You can program attiny 85 same as you program Arduino board using Arduino IDE.

Due to its compact size Attiny 85 is best for compact projects where you not need many IO’s and need to keep size of project as small as possible.

![image](https://user-images.githubusercontent.com/19898602/127041171-bc94a3e0-326d-4d20-ab5b-8e63ab4f17aa.png)


# Programming Attiny 85


So its time to program Attiny 85 means we need to load the code of game which we want to play on the game console.

For this we need code for game either you have to write your own game code or you can download it from anywhere from internet.

Writing code for game on your own is not piece of cake you need a pro level of coding skills, so we are going to use ready made game code for attiny 85 microcontroller.

Thanks to Andyhighnumber he already wrote many game codes and available for free to use, you can download Attiny Arduino game code from here.

As of now we have downloaded the code for games which we need to upload in attiny microcontroller, but this is not this easy because we cannot connect attiny 85 directly to PC/Laptop we need to us Arduino borad as ISP to load code to Attiny 85.

# Preparing Arduino as ISP to program Attiny

We need to get ready arduino as ISP so we have to upload ArduinoISP code to the arduino board

Simply connect your arduino board (in may case it is Arduino UNO) with laptop via data cable.

Go to the File > Examples > ArduinoISP > ArduinoISP

and upload this code to the arduino board I am using arduino UNO to load code to Attiny85 so you must have to select proper board before uploading the ISP code


![image](https://user-images.githubusercontent.com/19898602/127041503-e313e148-c1ad-4af5-aba0-b302c52a3674.png)


# Downloading Attiny board in Arduino IDE


By default Arduino don’t have any board option for attiny 85 microcontroller so we need to first add the board for Attiny 85 board for this kindly follow below steps.

first add below line of code to the preference option in Arduino IDE

Go to File > Preferences and add the below line of code in board URL place

https://raw.githubusercontent.com/damellis/attiny/ide-1.6.x-boards-manager/package_damellis_attiny_index.json

![image](https://user-images.githubusercontent.com/19898602/127041553-d8c99936-84b6-40e9-9f88-ca6c062dc6d9.png)

After completing above step now go to

Tools > Board > Board manager

and search for Attiny

and install the board by clicking on install option

![image](https://user-images.githubusercontent.com/19898602/127041611-09b27deb-395b-483f-b84f-b0ef16fe8d32.png)


![image](https://user-images.githubusercontent.com/19898602/127041622-f845dddf-e46c-43ef-961b-84e66d972cc1.png)


As of now attiny board is succesfully installed in our Arduino IDE, So now we need to wire Attiny with Arduino boras as per below diagram to upload game code.

![image](https://user-images.githubusercontent.com/19898602/127041657-280b9b5a-f413-4a22-a474-f4668befa92a.png)


After doing wiring as per above Image connect arduino board with laptop and open the game code which we have downloaded earlier and select the board option as shown in images below and upload the code.

Till now we have succefully uploaded game code to Attiny 85 now its time to make our game console please refer the below image for circuit diagram attach all the components as shown below

![MVI_0001_3](https://user-images.githubusercontent.com/19898602/127041928-58ad9bc6-f15f-46e4-9c8b-ec2a672fa4da.gif)





