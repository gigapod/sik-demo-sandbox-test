---
title: "Project 1 - Circuit B"
category: "Project 1"
description: "Potentiometers"
layout: project/sfe_banner_image_prj
thumbnail: "assets/img/photos/sik-proj1/SIK-Project-1-Circuit-2-Front.jpg"
bg_image: "/assets/img/photos/sik-proj1/SIK-Project-1-Circuit-2-Front.jpg"
about_title: "Project Overview"
previous_project: "/projects/circuit-1a"
next_project: "/projects/circuit-1c"
featured: true

# Additional content displayed  after main content
about_content: |
  <p>Potentiometers (also known as “pots” or “knobs”) are one of the basic inputs for electronics devices. By tracking the position of the knob with your RedBoard, you can make volume controls, speed controls, angle sensors and a ton of other useful inputs for your projects. In this circuit, you'll use a potentiometer as an input device to control the speed at which your LED blinks.
    </p>

    <figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Circuit 1B</p>'>
        <img src="/assets/img/photos/sik-proj1/SIK-Project-1-Circuit-2-Action-1.jpg"  alt="" />
    </figure>

---

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Circuit 1B - what is needed</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-demo-prj1-cb-need.png"  alt="" />
</figure>

## New Components

### Potentiometer

A [potentiometer](https://learn.sparkfun.com/tutorials/resistors#types-of-resistors) (trimpot for short) is a variable resistor. When powered with 5V, the middle pin outputs a voltage between 0V and 5V, depending on the position of the knob on the potentiometer. Internal to the trimpot is a single resistor and a wiper, which cuts the resistor in two and moves to adjust the ratio between both halves. Externally, there are usually three pins: two pins connect to each end of the resistor, while the third connects to the pot's wiper.


<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Potentiometer</p>' style="max-width:300px; margin:auto;">
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-potentiometer.jpg" alt="" style="max-width:100%; height:auto;" />
</figure>

## New Concepts

### Analog vs. Digital

Understanding the difference between analog and digital is a fundamental concept in electronics.

We live in an analog world. There is an infinite number of colors to paint an object (even if the difference is indiscernible to our eye), an infinite number of tones we can hear, and an infinite number of smells we can smell. The common theme among all of these analog signals is their infinite possibilities.

**Digital** signals deal in the realm of the **discrete** or **finite**, meaning there is a limited set of values they can be. The LED from the previous circuit had only two states it could exist in, ON or OFF, when connected to a Digital Output.

### Analog Inputs
So far, we've only dealt with outputs. The RedBoard also has inputs. Both inputs and outputs can be analog or digital. Based on our definition of analog and digital above, that means an [analog input](https://docs.arduino.cc/built-in-examples/analog/AnalogInput/) can sense a wide range of values versus a [digital input](https://docs.arduino.cc/learn/microcontrollers/digital-pins/), which can only sense two states.

You may have noticed some pins labeled with an "A" before the pin number on the bottom left of your RedBoard. These are the only six pins that function as analog inputs; they are labeled A0--A5.

MicroPython also has a built in way for us to easily read values from these analog pins. It is the `ADC` object from the `machine` module. It has a method `read_u16` that gives us a 16-bit unsigned integer number representing the value on the pin (that's where the u16 comes from: *u* for *unsigned* and *16* for *16-bit*). We'll use that to read values from our potentiometer. We'll describe this a bit more in the next circuit.

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Analog Input Pins</p>' style="max-width:800px; margin:auto;">
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-analog-in.jpg" alt="" style="max-width:100%; height:auto;" />
</figure>

### Voltage Divider

A [voltage divider](https://learn.sparkfun.com/tutorials/voltage-dividers) is a simple circuit that turns some voltage into a smaller voltage using two resistors. The following is a *schematic* of the voltage divider circuit. [Schematics](https://learn.sparkfun.com/tutorials/how-to-read-a-schematic) are a universally agreed upon set of symbols that engineers use to represent electric circuits.

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Voltage Divider Schematic</p>' style="max-width:400px; margin:auto;">
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-vdiv.png" alt="" style="max-width:100%; height:auto;"/>
</figure>

A potentiometer is a variable resistor that can be used to create an adjustable voltage divider.

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Potentiometer Schematic</p>' style="max-width:400px; margin:auto;">
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-pot-schem.png"  alt="" style="max-width:100%; height:auto;" />
</figure>

*A potentiometer schematic symbol where pins 1 and 3 are the resistor ends, and pin 2 connects to the wiper*

If the outside pins connect to a voltage source (one to ground, the other to Vin), the output (Vout) at the middle pin will mimic a voltage divider. Turn the trimpot all the way in one direction, and the voltage may be zero; turned to the other side, the output voltage approaches the input. A wiper in the middle position means the output voltage will be half of the input.

Voltage dividers will be covered in more detail in the next circuit.

## Hookup Guide

The potentiometer has three legs. Pay close attention into which pins you're inserting it on the breadboard, as they will be hard to see once inserted.

Potentiometers are not polarized. You can attach either of the outside pins to 5V and the opposite to GND. However, the values you get out of the trimpot will change based on which pin is 5V and which is GND.

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Potentiometer Pinout</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-pot-pinout.jpg"  alt="" />
</figure>

**READY TO START HOOKING EVERYTHING UP?** Check out the circuit diagram and
hookup table below to see how everything is connected.

## Circuit Diagram

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Hookup Diagram</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-hookup.jpg"  alt="" />
</figure>

**Note for Advanced Users:** If you know how to read datasheets and schematics, you can also refer to the schematic below as an alternative.

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Circuit Schematic</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-schem.jpg"  alt="" />
</figure>

## Hookup Table
<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Circuit Schematic</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-docs-prj1-cb-hu-table.png"  alt="" />
</figure>

<br>

## Programming the RedBoard

The SparkFun RedBoard IoT is programmed using MicroPython and this project uses MicroPython commands to control the circuit.  Before this is possible, a MicroPython tool is needed to communcate with the ReadBoard.

### Selecting a MicroPython Tool

The first step to enter commands on the RedBoard is to select a tool that allows direct interaction with MicroPython. 

While a variety of methods exist to communicate with the RedBoard, the following tools are the most popular: Thonny, PyCharm and the command `mpremote`.

Once you select and install a tool, make sure your RedBoard is connected to your computer, and the micropython tool is connected to the RedBoard. Once connected, you should have access to the MicroPython REPL command line.

### Entering MicroPython Commands

#### Step 1 - Setup

Like last circuit, to operate the LED, we need to enable the board pin **34** (the pin that the LED is connected to in the circuit).  

To do this we **load the Pin definition for the board**

{% 
    include helpers/codeHeader.html 
    code = "from machine import Pin"
%}

Next, we **load the ADC object** to allow us to read our analog pin

{% 
    include helpers/codeHeader.html 
    code = "from machine import ADC"
%}

Now we declare our digital pin for the led and our `ADC` to read the analog pin for the potentiometer. We use `Pin.board.A0` becuase our potentiometer is physically connected to "A0" (the first analog pin). 

{% capture pot_code %}
led_pin = Pin(34, Pin.OUT) # Create a pin variable for the led pin (pin 34)
potentiometer = ADC(Pin.board.A0)
{% endcapture %}

{% 
    include helpers/codeHeader.html 
    code = pot_code
%}

Now, we can read from A0 to read and print the potentiometer value:

{% 
    include helpers/codeHeader.html 
    code = "print(potentiometer.read_u16()) # Use the read_u16 method to read the value of our potentiometer."
%}

Now let's create an infinite loop and change the speed at which we blink the LED based on the potentiometer position. 


{%capture pot_loop %}
# Now, let's blink the LED with different speeds based on the potentiometer input
import time # Allows us to use "time.sleep()" to delay for a certain number of seconds

# Infinite loop so this cell keeps running until we stop it.
while True:
    potPosition = potentiometer.read_u16() # Get the new potentiometer position (0 - 65535)

    # Lets choose a delay that is proportional to the potentiometer reading
    # Since the range of the potentiometer is 0-65535 and we want delays between 0-2 seconds, 
    # we will divide by (65535 / 2 ) = 32767.5
    delay = (potPosition / 32767.5) 

    # We will comment out the print for now since it can spam our console when the delay is fairly low
    # print(f"Potentiometer Value: {potPosition : 5}", end='\r') # Print our potentiometer reading (don't mind the fanciness of this line it just makes the print format nicely)

    # Turn on the LED
    led_pin.high()

    # Delay based on potentiometer position
    time.sleep(delay)
    
    # Turn off the LED
    led_pin.low()
    
    # Delay based on potentiometer position
    time.sleep(delay)
{% endcapture %}

{% 
    include helpers/codeHeader.html 
    code = pot_loop
%}

<br>

## What You Should See
You should see the LED blink faster or slower in accordance with your potentiometer. The delay between each flash will change based on the position of the knob. If it isn't working, make sure you have assembled the circuit correctly and verified and run the code on your board, or see the Troubleshooting section.

<br>

## Coding Challenges

| Challenge            | Description                                                                                                                                                                                                                      |
|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Changing the Range   | Try multiplying, dividing or adding to your sensor reading so that you can change the range of the delay in your code. For example, can you multiply the sensor reading so that the delay goes from 0–2046 instead of 0–65535?   |
| Adding More LEDs     | Add more LEDs to your circuit. Don't forget the current limiting resistor for each one. Try making multiple LEDs blink at different rates by changing the range of each using multiplication or division.                         |

<br>

## Troubleshooting

| Problem                                       | Solution                                                                                                                        |
|-----------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
| The potentiometer always reads as 0 or 65535. | Make sure your 5V, A0, and GND pins are properly connected to the three pins on your potentiometer.                             |
| No values printed                             | Ensure you are connected to the correct serial port and have run the correct code example (or properly copied and pasted all code blocks from this guide in-order) |

<br>

## You've Completed Circuit 1B!

Continue to circuit 1C to learn about photoresistors

<figure class="itooltip itooltip-dark hover-scale rounded" title='<p class="mb-0">Next - Circuit 1B</p>'>
    <img src="/assets/img/photos/sik-proj1/sik-demo-prj1-cb-next.png"  alt="" />
</figure>
