Assemble Mecanum Robot 
-----------------------

It is a programmable car based on BBC micro:bit. It integrates a motor
driver, a line tracking sensor and an IR receiver into the base plate,
which also contains an ultrasonic sensor, a servo, 2 seven-color lights
as well as 4 WS2812 RGB lights. The wiring is not complicated and it has
Lego jacks to facilitate connection with other peripheral devices.
Abundant hardware resources will enable you to master more knowledge and
skills to create more technological inventions.

Sensors and control pins of the 4WD Mecanum Robot Car V2.0
----------------------------------------------------------

This car can help you to better learn how to use the Micro:bit and make
electronic knowledge accessible to you.

**Functions**

+--------+-------------+--------------+-------+------------+----------+----------+--------+--------+
| Sensor | Seven-color | Decelerating | Servo | Ultrasonic | Line     | IR       | WS2812 | Power  |
|        | light       | DC motor     |       | sensor     | Tracking | Receiver | RGB    | switch |
|        |             |              |       |            | Sensor   |          | light  |        |
+--------+-------------+--------------+-------+------------+----------+----------+--------+--------+
| QTY    | 2           | 4            | 1     | 1          | 3        | 1        | 4      | 1      |
+--------+-------------+--------------+-------+------------+----------+----------+--------+--------+

**Note: the line tracking sensor, WS2812 RGB lights, IR receiver and
moto river are integrated in the base plate.**

**Pins：**

.. figure:: ./media/Pins.png
   :alt: Img

   Img

**Power supply and Battery**

The keyestudio 4WD Mecanum Robot Car is powered by two 18650 batteries.
The battery holder of the car is compatible with any type of 18650
lithium battery (rechargeable). You can use a universal battery charger
to charge the 18650 lithium battery.

**Note:** This product does not contain batteries.

The Installation of Keyestudio 4WD Mecanum Robot Car V2.0
---------------------------------------------------------

Step 1

**Components Needed:**

|image1|

**Installation Diagram:**

|image2|

**Prototype:**

|image3|

Step 2

**Components Needed:**

|image4|

**Installation Diagram:**

|image5|

**Prototype:**

|image6|

Step 3

**Components Needed:**

|image7|

**Installation Diagram:**

|image8|

**Prototype:**

|image9|

Step 4

（adjust the angle of the servo first）

**Adjust the angle of the servo to 90 degrees.**

**Method 1：MakeCode code**

⚠️\ **Special note:** Before you write the code and upload it, you must
Understand the MakeCode IDE and add library files, please go to the the
link:  :download:`Get Started with makecode <./Code1.7z>`

|image10|

The MakeCode code above is provided in the materials. Open the
adjustment code of the servo and burn it into the microbit motherboard
of the 4WD Mecanum Robot Car V2.0, and **power on via micro USB cable or
external power supply(turn the DIP switch to ON)**. That’s it. The code
is at the following position as shown in the figure:

.. figure:: ./media/b11.png
   :alt: Img

   Img

**Method 2：Python code**

⚠️\ **Special note:** Before you write the code and upload it, you must
install the Mu IDE and add library files, please go to the the link:
 :download:`Get Started with Python <./Code2.7z>`

.. code:: python

   # import microbit related libraries
   from microbit import *

   class Servo:
       def __init__(self, pin, freq=50, min_us=600, max_us=2400, angle=180):
           self.min_us = min_us
           self.max_us = max_us
           self.us = 0
           self.freq = freq
           self.angle = angle
           self.analog_period = 0
           self.pin = pin
           analog_period = round((1/self.freq) * 1000)  # hertz to miliseconds
           self.pin.set_analog_period(analog_period)

       def write_us(self, us):
           us = min(self.max_us, max(self.min_us, us))
           duty = round(us * 1024 * self.freq // 1000000)
           self.pin.write_analog(duty)
           sleep(100)
           self.pin.write_analog(0)

       def write_angle(self, degrees=None):
           if degrees is None:
               degrees = math.degrees(radians)
           degrees = degrees % 360
           total_range = self.max_us - self.min_us
           us = self.min_us + total_range * degrees // self.angle
           self.write_us(us)


   Servo(pin14).write_angle(90)
   sleep(1000)

**Components Needed:**

|image11|

Installation Diagram: (mind the installation direction)

|image12|

**Prototype:**

|image13|

Step 5

**Components Needed:**

|image14|

**Installation Diagram:**

|image15|

**Prototype:**

|image16|

Step 6

**Components Needed:**

|image17|

**Installation Diagram:**

|image18|

**Prototype:**

|image19|

Step 7

**Components Needed:**

|image20|

**Installation Diagram:** (mind the direction of the motor)

|image21|

**Prototype:**

|image22|

Step 8

**Components Needed:**

|image23|

**Installation Diagram:** (Pay attention to the installation direction
of the mecanum wheel)

|image24|

**Prototype:**

|image25|

Step 9

**Components Needed:**

|image26|

**Installation Diagram:**

|image27|

**Prototype:**

|image28|

Step 10

**Components Needed:**

|image29|

**Installation Diagram:**

|image30|

**Prototype:**

|image31|

Wiring Diagram

**The wiring of the servo:**

.. figure:: ./media/b34.png
   :alt: Img

   Img

|image32|

|image33|

**The wiring of the ultrasonic sensor:**

.. figure:: ./media/b37.png
   :alt: Img

   Img

|image34|

|image35|

**The wiring of the IR receiver module:**

.. figure:: ./media/b40.png
   :alt: Img

   Img

|image36|

**The wiring of the RGB:**

.. figure:: ./media/b42.png
   :alt: Img

   Img

|image37|

**The wiring of controlling the motor and seven-color light :**

.. figure:: ./media/b44.png
   :alt: Img

   Img

|image38|

**The wiring of controlling the 3-channel line-tracking sensor:**

.. figure:: ./media/b46.png
   :alt: Img

   Img

|image39|

**The wiring of the power supply:**

|image40|

**The corresponding interface of the motor:**

|image41|

**The installation of the battery:**

|image42|

.. |image1| image:: ./media/b1.png
.. |image2| image:: ./media/b2.png
.. |image3| image:: ./media/b3.png
.. |image4| image:: ./media/b4.png
.. |image5| image:: ./media/b5.png
.. |image6| image:: ./media/b6.png
.. |image7| image:: ./media/b7.png
.. |image8| image:: ./media/b8.png
.. |image9| image:: ./media/b9.png
.. |image10| image:: ./media/b10.png
.. |image11| image:: ./media/b13.png
.. |image12| image:: ./media/b14.png
.. |image13| image:: ./media/b15.png
.. |image14| image:: ./media/b16.png
.. |image15| image:: ./media/b17.png
.. |image16| image:: ./media/b18.png
.. |image17| image:: ./media/b19.png
.. |image18| image:: ./media/b20.png
.. |image19| image:: ./media/b21.png
.. |image20| image:: ./media/b22.png
.. |image21| image:: ./media/b23.png
.. |image22| image:: ./media/b24.png
.. |image23| image:: ./media/b25.png
.. |image24| image:: ./media/b26.png
.. |image25| image:: ./media/b27.png
.. |image26| image:: ./media/b28.png
.. |image27| image:: ./media/b29.png
.. |image28| image:: ./media/b30.png
.. |image29| image:: ./media/b31.png
.. |image30| image:: ./media/b32.png
.. |image31| image:: ./media/b33.png
.. |image32| image:: ./media/b35.jpg
.. |image33| image:: ./media/b36.png
.. |image34| image:: ./media/b38.jpg
.. |image35| image:: ./media/b39.png
.. |image36| image:: ./media/b41.png
.. |image37| image:: ./media/b43.jpg
.. |image38| image:: ./media/b45.jpg
.. |image39| image:: ./media/b47.jpg
.. |image40| image:: ./media/b48.jpg
.. |image41| image:: ./media/b40.jpg
.. |image42| image:: ./media/b50.png
