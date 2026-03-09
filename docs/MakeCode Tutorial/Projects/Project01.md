## 3.2.1 Multifunctional Car 

---------------

### 3.2.1.1 Overview

![Img](./media/top1.png)

Here we build a multifunctional car with a Micro:bit V2 board, a servo expansion board, two 360° LEGO servos, two wheels and some LEGO parts. We program to control the car through the Micro:bit V2 logo, buttons (A, B and A+B) and 5×5 LED matrix.

![Img](./media/bottom1.png)

---------------

### 3.2.1.2 Component Knowledge

![Img](./media/2top.png)

**360° LEGO Servo**

![Img](./media/cou7110.png)

It features multiple mounting holes on both sides and dual output cross-axis holes on both sides, and is compatible with 2KG LEGO bricks. It enables 360-degree rapid continuous rotation with a gear reduction ratio of 1:140. The gear is protected from over-torque and random twisting through tooth engagement. As a continuous rotation servo, it can control speed and direction by PWM but cannot position angles or track rotations.

This 360° LEGO servo boasts three lines: brown one for ground, red one for power positive, and orange one for signal.

![Img](./media/cou710-1.png)

Parameters:

- Operating voltage: 3V ~ 6V
- Pulse width: 500 ~ 2500μsec
- Operating angle: 360° continuous rotation
- No-load current: 65 ± 20mA (3V test), 80 ± 20mA (5V test)
- No-load speed: 90 ± 10r/min (3V test), 160 ± 10r/min (5V test)
- Motor speed: 12500 ± 10% (3V test), 22000 ± 10% (5V test)
- Stop current: 0.70 ± 0.2A (3V test), 1.1 ± 0.2A (5V test)
- Stop torque: 0.5 ± 0.1kg-cm (3V test), 0.7 ± 0.1kg-cm (5V test)
- Wiring: Orange for signal S, red for positive ( + / V / VCC / 5V ), brown for negative ( - / G / GND )

**SK6812 RGB LED**

![Img](./media/cou710.png)

There are five SK6812 RGB LEDs on the servo extension board, which can emit multiple colors of light. By mixing the different intensities of the three basic colors of red, green, and blue, various rich color lights can be generated, and the brightness of the color lights can be adjusted.

![Img](./media/2bottom.png)

---------------

### 3.2.1.3 Materials Required

![Img](./media/A1-0.png)

---------------

### 3.2.1.4 Installation Steps

![Img](./media/2top.png)

![Img](./media/A1-1.png)

![Img](./media/A1-2.png)

![Img](./media/A1-3.png)

![Img](./media/A1-4.png)

![Img](./media/A1-5.png)

![Img](./media/A1-6.png)

![Img](./media/A1-7.png)

![Img](./media/A1-8.png)

![Img](./media/A1-9.png)

![Img](./media/A1-10.png)

![Img](./media/A1-11.png)

![Img](./media/A1-12.png)

![Img](./media/A1-13.png)

![Img](./media/A1-14.png)

![Img](./media/A1-15.png)

![Img](./media/A1-16.png)

![Img](./media/A1-17.png)

![Img](./media/A1-18.png)

![Img](./media/A1-19.png)

![Img](./media/A01.png)

![Img](./media/A1-20.png)

![Img](./media/A1-21.png)

![Img](./media/A1-22.png)

![Img](./media/A1-23.png)

![Img](./media/A1-24.png)

![Img](./media/A1-25.png)

![Img](./media/A1-26.png)

![Img](./media/A1-27.png)

![Img](./media/A1-28.png)

![Img](./media/wiring1.png)

![Img](./media/A1-29.png)

![Img](./media/2bottom.png)

---------------

### 3.2.1.5 Code Blocks

1\. "**on start**": codes in it run only once.

![Img](./media/on-start.png)

2\. Set the icon on the 5×5 LED matrix of the Micro:bit V2 board.

![Img](./media/55LED.png)

3\. Set the pin of these SK6812 RGB LEDs and the number of lit SK6812 RGB LEDs.

![Img](./media/RGBLED.png)

4\. Set the brightness of these SK6812 RGB LEDs.

![Img](./media/RGBLED1.png)

5\. Turn off these SK6812 RGB LEDs.

![Img](./media/RGBclear.png)

6\. Codes in it will run when the logo on the Micro:bit V2 board is touched.

![Img](./media/logo.png)

7\. Press (or simultaneously press) the buttons (A, B, or A+B) on the Micro:bit V2 board and release them again, trigger and execute a series of actions within a code block.

![Img](./media/buttonAB.png)

8\. Codes in it will run when the 5×5 LED matrix of Micro:bit V2 board faces upwards.

![Img](./media/screen-up.png)

9\. Show an arrow on the 5×5 LED matrix of Micro:bit V2 board.

![Img](./media/arrow.png)

10\. Set the color of light of these SK6812 RGB LEDs.

![Img](./media/color.png)

11\. Set the pin, rotation direction (clockwise / counterclockwise) and speed (0~100%) of the 360° LEGO servo. 

![Img](./media/360Servo.png)

12\. Clear all display on the 5×5 LED matrix of the Micro:bit V2 board.

![Img](./media/55LEDClear.png)

---------------

### 3.2.1.6 Test Code

<span style="color: rgb(255, 76, 65);">The speed value 30 in the code can be adjusted appropriately according to your needs.</span>

![Img](./media/couj01.png)

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: You can obtain the sample code through the following two methods.</span>**

#### **Method 1: drag and drop code blocks to build the sample code**

**1. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**2. MakeCode extension library**

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: </span>** Copy and paste the link: `https://github.com/keyestudio2019/pxt-creative-inventors-kit-master.git` into the search box to import the library.

![Img](./media/Animation-4.gif)

**3. Write the sample code**

![Img](./media/dongtu-01.gif)

#### **Method 2: download the sample code file directly**

**1. Download the code file**

Click to download the code file:  [3_3_1_Multifunctional_Car](./1Multifunctional_Car.zip)

**2. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**3. Load the sample code**

Drag and drop the sample code to the MakeCode editor.

![Img](./media/Animation-0001.gif)

![Img](./media/line1.png)

**Brief explanation**

① Initialize the SK6812 RGB LED pin P0, the number of the lit SK6812 RGB LEDs and its brightness. Turn off all SK6812 RGB LEDs. The 5×5 LED matrix on the board shows ![Img](./media/ab3.png).

![Img](./media/cou00.png)

② Touch the logo on the Micro:bit V2 board, the car moves forward, these SK6812 RGB LEDs emit red light, and the 5×5 LED matrix displays "↑".

![Img](./media/cou01.png)

③ Press button A on the Micro:bit V2 board and release it, the car turns right, these SK6812 RGB LEDs light up in cyan, and the 5×5 LED matrix shows "←".

![Img](./media/cou02.png)

④ Press button B on the Micro:bit V2 board and release it, the car turns left, these SK6812 RGB LEDs light up in magenta, and the 5×5 LED matrix shows "→". 

![Img](./media/cou03.png) 

⑤ Press button A and B on the Micro:bit V2 board simultaneously and release them, the car moves backward, these SK6812 RGB LEDs emit green light, and the 5×5 LED matrix displays "↓". 

![Img](./media/cou04.png)

⑥ Face the 5×5 LED matrix on the Micro:bit V2 board upwards, the car stops, and these SK6812 RGB LEDs and the 5×5 LED matrix turn off.

![Img](./media/cou05.png)

---------------

### 3.2.1.7 Test Result

![Img](./media/4top.png)

Wire up and power on through Micro USB cable, and connect an external power source (four AAA-1.5V batteries installed in the battery box, ensuring sufficient power).

To download the sample code using an online browser, you need to send the downloaded "**.hex**" file to the Micro:bit V2 board. There are two ways as follows: 

**① Download through WebUSB**

For browsers like **Google Chrome / Microsoft Edge**, you need to click "**Connect Device**" to pair the device first. After that, click "**Download**" to load the sample code to the Micro:bit V2 board.

![Img](./media/Animation-01.gif)

**② Download without WebUSB**

For browsers like **Safari / Firefox / Other**, download and send the sample code to the Micro:bit V2 board.

![Img](./media/Animation-001.gif)

After downloading the sample code, the 5×5 LED matrix shows ![Img](./media/ab3.png). And then unplug the Micro USB cable to the Micro:bit V2 board.

Turn the DIP switched to the RGB and ON.

![Img](./media/CBA01.png)

Touch the logo on the Micro:bit V2 board, the car moves forward, these SK6812 RGB LEDs emit red light, and the 5×5 LED matrix displays "↑".

Press button A and B on the Micro:bit V2 board simultaneously and release them, the car moves backward, these SK6812 RGB LEDs emit green light, and the 5×5 LED matrix displays "↓". 

Press button A on the Micro:bit V2 board and release it, the car turns right, these SK6812 RGB LEDs light up in cyan, and the 5×5 LED matrix shows "←". 

Press button B on the Micro:bit V2 board and release it, the car turns left, these SK6812 RGB LEDs light up in magenta, and the 5×5 LED matrix shows "→". 

Face the 5×5 LED matrix on the Micro:bit V2 board upwards, the car stops, and these SK6812 RGB LEDs and the 5×5 LED matrix turn off.

![Img](./media/dongtu-001.gif)

![Img](./media/4bottom.png)

⚠️ **<span style="color: rgb(255, 76, 65);">If the 5×5 LED matrix shows some icons and numbers after downloading the code to the Micro:bit V2 board, the code fails to be loaded to the board and needs to be reloaded.</span>**

![Img](./media/dongtu-00.gif)

---------------