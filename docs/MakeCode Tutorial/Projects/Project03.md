## 3.2.3 Sound-controlled Animal 

---------------

### 3.2.3.1 Overview

![Img](./media/top1.png)

Here we build a sound-controlled animal with a Micro:bit V2 board, a servo expansion board, a 360° LEGO servo and some LEGO parts. We program to control it to perform some movements through the Micro:bit V2 microphone.

![Img](./media/bottom1.png)

---------------

### 3.2.3.2 Materials Required

![Img](./media/A3-0.png)

---------------

### 3.2.3.3 Installation Steps

![Img](./media/2top.png)

![Img](./media/A3-1.png)

![Img](./media/A3-2.png)

![Img](./media/A3-3.png)

![Img](./media/A3-4.png)

![Img](./media/A3-5.png)

![Img](./media/A3-6.png)

![Img](./media/A3-7.png)

![Img](./media/A3-8.png)

![Img](./media/A3-9.png)

![Img](./media/A3-10.png)

![Img](./media/A3-11.png)

![Img](./media/A3-12.png)

![Img](./media/A3-13.png)

![Img](./media/A3-14.png)

![Img](./media/A3-15.png)

![Img](./media/A3-16.png)

![Img](./media/A3-17.png)

![Img](./media/A3-18.png)

![Img](./media/A3-19.png)

![Img](./media/A3-20.png)

![Img](./media/A3-21.png)

![Img](./media/A3-22.png)

![Img](./media/A3-23.png)

![Img](./media/A3-24.png)

![Img](./media/A3-25.png)

![Img](./media/A3-26.png)

![Img](./media/A3-27.png)

![Img](./media/A3-28.png)

![Img](./media/A3-29.png)

![Img](./media/A3-30.png)

![Img](./media/A3-31.png)

![Img](./media/A3-32.png)

![Img](./media/A3-33.png)

![Img](./media/A3-34.png)

![Img](./media/A3-35.png)

![Img](./media/A3-36.png)

![Img](./media/A03.png)

![Img](./media/wiring3.png)

![Img](./media/A3-37.png)

![Img](./media/A3-38.png)

![Img](./media/A3-39.png)

![Img](./media/A3-40.png)

![Img](./media/A3-41.png)

![Img](./media/A3-42.png)

![Img](./media/A3-43.png)

![Img](./media/A3-44.png)

![Img](./media/A3-45.png)

![Img](./media/A3-46.png)

![Img](./media/A3-47.png)

![Img](./media/A3-48.png)

![Img](./media/A3-49.png)

![Img](./media/2bottom.png)

---------------

### 3.2.3.4 Code Blocks

1\. “**on start**”: codes in it run only once.

![Img](./media/on-start.png)

2\. “**forever**”: codes in it run repeatedly.

![Img](./media/forever.png)

3\. Set SK6812 RGB LED to gradient color within the range of 1~360.

![Img](./media/gradient-color.png)

4\. if()...else...

When the condition in "if()" is satisfied, codes under "then" will execute; Or else, codes under "else" will run.

![Img](./media/if-else-1.png)

5\. Read the sound level through the microphone in the Micro:bit V2 board, ranging from 0(quiet) to 255(noise).

![Img](./media/soundlevel.png)

6\. The expression for making a judgment. When using it, two numerical values or variable modules that need to be judged should be added to the two ends of the block.

![Img](./media/img18.png)

![Img](./media/img02.png)

7\. Delay.

![Img](./media/delaytime.png)

---------------

### 3.2.3.5 Test Code

<span style="color: rgb(255, 76, 65);">The threshold 150 in "if()" can be modified according to actual conditions.</span>

![Img](./media/couj03.png)

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: You can obtain the sample code through the following two methods.</span>**

#### **Method 1: drag and drop code blocks to build the sample code**

**1. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**2. MakeCode extension library**

⚠️ **<span style="color: rgb(255, 76, 65);">Special reminder: </span>** Copy and paste the link: `https://github.com/keyestudio2019/pxt-creative-inventors-kit-master.git` into the search box to import the library.

![Img](./media/Animation-4.gif)

**3. Write the sample code:**

![Img](./media/dongtu-03.gif)

#### **Method 2: download the sample code file directly**

**1. Download the code file**

Click to download the code file: [3_3_3_Voice_Controlled_Animal](./3oice_Controlled_Animal.zip)

**2. MakeCode programming environment**

The online version of MakeCode: <u>[MakeCode editor](https://makecode.microbit.org/#editor)</u>

**3. Load the sample code**

Drag and drop the sample code to the MakeCode editor.

![Img](./media/Animation-0003.gif)

![Img](./media/line1.png)

---------------

### 3.2.3.6 Test Result

![Img](./media/4top.png)

Wire up and power on through Micro USB cable, and connect an external power source (four AAA-1.5V batteries installed in the battery box, ensuring sufficient power).

To download the sample code using an online browser, you need to send the downloaded "**.hex**" file to the Micro:bit V2 board. There are two ways as follows: 

**① Download through WebUSB**

For browsers like **Google Chrome / Microsoft Edge**, you need to click "**Connect Device**" to pair the device first. After that, click "**Download**" to load the sample code to the Micro:bit V2 board.

![Img](./media/Animation-03.gif)

**② Download without WebUSB**

For browsers like **Safari / Firefox / Other**, download and send the sample code to the Micro:bit V2 board.

![Img](./media/Animation-003.gif)

After downloading the sample code, unplug the micro USB cable to the Micro:bit V2 board.

Turn the DIP switched to the RGB and ON.

![Img](./media/CBA01.png)

If the sound level ≥ 150 detected by the microphone on the Micro:bit V2 board, the animal runs for 1s, these SK6812 RGB LEDs emit colorful light, and the 5×5 LED matrix displays ![Img](./media/ab3.png).

If the sound level < 150, the animal stops running, and these SK6812 RGB LEDs and the 5×5 LED matrix turn off.

![Img](./media/dongtu-003.gif)

![Img](./media/4bottom.png)

---------------

