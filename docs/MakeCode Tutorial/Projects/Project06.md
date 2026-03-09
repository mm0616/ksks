## 3.2.6 Smart Light Following Dog

---------------

### 3.2.6.1 Overview

![Img](./media/top1.png)

Here we build a smart light following dog with a Micro:bit V2 board, a servo expansion board, a 360° LEGO servo and some LEGO parts. We program to control the dog to chase light through the Micro:bit 5×5 LED matrix.

![Img](./media/bottom1.png)

---------------

### 3.2.6.2 Materials Required

![Img](./media/A6-0.png)

---------------

### 3.2.6.3 Installation Steps

![Img](./media/2top.png)

![Img](./media/A6-1.png)

![Img](./media/A6-2.png)

![Img](./media/A6-3.png)

![Img](./media/A6-4.png)

![Img](./media/A6-5.png)

![Img](./media/A6-6.png)

![Img](./media/A6-7.png)

![Img](./media/A6-8.png)

![Img](./media/A6-9.png)

![Img](./media/A6-10.png)

![Img](./media/A6-11.png)

![Img](./media/A6-12.png)

![Img](./media/A6-13.png)

![Img](./media/A6-14.png)

![Img](./media/A6-15.png)

![Img](./media/A6-16.png)

![Img](./media/A6-17.png)

![Img](./media/A6-18.png)

![Img](./media/A6-19.png)

![Img](./media/A6-20.png)

![Img](./media/A6-21.png)

![Img](./media/A6-22.png)

![Img](./media/A6-23.png)

![Img](./media/A6-24.png)

![Img](./media/A6-25.png)

![Img](./media/A6-26.png)

![Img](./media/A6-27.png)

![Img](./media/A6-28.png)

![Img](./media/A06.png)

![Img](./media/wiring6.png)

![Img](./media/A6-29.png)

![Img](./media/A6-30.png)

![Img](./media/A6-31.png)

![Img](./media/2bottom.png)

---------------

### 3.2.6.4 Code Blocks

1\. if()...else if()...else...

When the condition in "if()" is satisfied, codes under "then" will execute. Or, When the condition in "else if()" is satisfied, codes under "then" will execute. Otherwise, codes under "else" will run.

![Img](./media/if-else.png)

2\. Read the light level through the 5×5 LED matrix on the Micro:bit V2 board, ranging from 0 (dim) to 255 (bright).

![Img](./media/lightlevel.png)

---------------

### 3.2.6.5 Test Code

<span style="color: rgb(255, 76, 65);">The threshold 10 and 150 in "if()...else if()..." can be modified according to actual conditions.</span>

![Img](./media/couj06.png)

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: You can obtain the sample code through the following two methods.</span>**

#### **Method 1: drag and drop code blocks to build the sample code**

**1. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**2. MakeCode extension library**

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: </span>** Copy and paste the link: `https://github.com/keyestudio2019/pxt-creative-inventors-kit-master.git` into the search box to import the library.

![Img](./media/Animation-4.gif)

**3. Write the sample code**

![Img](./media/dongtu-06.gif)

#### **Method 2: download the sample code file directly**

**1. Download the code file**

Click to download the code file: [3_3_6_Smart_Light_Following_Dog](./6Smart_Light_Following_Dog.zip)

**2. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**3. Load the sample code**

Drag and drop the sample code to the MakeCode editor.

![Img](./media/Animation-0006.gif)

![Img](./media/line1.png)

---------------

### 3.2.6.6 Test Result

![Img](./media/4top.png)

Wire up and power on through Micro USB cable, and connect an external power source (four AAA-1.5V batteries installed in the battery box, ensuring sufficient power).

To download the sample code using an online browser, you need to send the downloaded "**.hex**" file to the Micro:bit V2 board. There are two ways as follows: 

**① Download through WebUSB**

For browsers like **Google Chrome / Microsoft Edge**, you need to click "**Connect Device**" to pair the device first. After that, click "**Download**" to load the sample code to the Micro:bit V2 board.

![Img](./media/Animation-06.gif)

**② Download without WebUSB**

For browsers like **Safari / Firefox / Other**, download and send the sample code to the Micro:bit V2 board.

![Img](./media/Animation-006.gif)

After downloading the sample code, unplug the Micro USB cable to the Micro:bit V2 board.

Turn the DIP switched to the RGB and ON.

![Img](./media/CBA01.png)

Shine a light source (such as your phone's flashlight) onto the 5×5 LED matrix on the Micro:bit V2 board.

If the light level ≥ 150 detected by the Micro:bit V2 board, the light-following dog steps back with the light, these SK6812 RGB LEDs emit red light, and the 5×5 LED matrix displays ![Img](./media/ab5.png).

If 10 < light level < 150, the light-following dog follows the light, these SK6812 RGB LEDs emit cyan light, and the 5×5 LED matrix displays ![Img](./media/ab3.png).

If the light level ≤ 10, the light-following dog stops, and these SK6812 RGB LEDs and the 5×5 LED matrix turn off.

![Img](./media/dongtu-006.gif)   

![Img](./media/4bottom.png)

---------------

