<!--  
{  
  "ID": "9f4c2e7a-3b6d-4e2f-aed7-1c3b9f8a4d6e",  
  "Title": "Blink Arduino LED",  
  "Tags": ["Arduino", "Embedded Software", "Beginner", "LED", "Programming"],  
  "Description": "Learn how to blink the built-in LED on an Arduino UNO using basic embedded software principles.",  
  "Query": "Generate a training exercise to blink the built-in LED on Arduino UNO, focus on Embedded Software, beginner level, with hidden, overview, prerequisite, exercise, summary, and follow-up sections.",  
  "Model": "GPT-5 mini",  
  "Focus": "Embedded Software",  
  "Level": "Beginner",  
  "Date": "20250828",  
  "Links": ["https://www.arduino.cc/en/Tutorial/Blink", "https://www.arduino.cc/en/Guide/HomePage"],  
  "Filename": "blink_arduino_led_exercise"  
}  
-->

# Blink the Built-In LED on Arduino UNO

## Overview

In this exercise, you will learn how to make the built-in LED on an Arduino UNO blink on and off. This simple task introduces you to embedded software programming and basic control of hardware using code. By the end of this exercise, you will understand how to control outputs on a microcontroller, use timing functions, and upload programs to an Arduino.

## Prerequisites

Before starting this exercise, ensure you have the following:

1. **Hardware**

   * Arduino UNO board
   * USB cable compatible with Arduino UNO
   * Computer with Arduino IDE installed

2. **Software**

   * Arduino IDE installed on your computer (download from [Arduino Official Website](https://www.arduino.cc/en/software))
   * Basic understanding of navigating software and typing code

3. **Knowledge**

   * Familiarity with basic programming concepts like loops and functions

## Exercise: Blink the Built-In LED

1. **Connect your Arduino UNO to the computer** using the USB cable. Ensure it is recognized by your computer.

2. **Open the Arduino IDE** on your computer.

3. **Create a new sketch** by clicking **File → New**. A blank code window will appear.

4. **Define the LED pin**:

   * At the top of your sketch, type: `int ledPin = 13;`
   * This assigns the built-in LED to a variable called `ledPin`.

5. **Set up the `setup()` function**:

   * Inside your sketch, write:

     ```
     void setup() {
       pinMode(ledPin, OUTPUT);
     }
     ```
   * This tells the Arduino that the LED pin will be used as an output.

6. **Create the `loop()` function**:

   * Add the following code:

     ```
     void loop() {
       digitalWrite(ledPin, HIGH); // Turn the LED on
       delay(1000);                 // Wait for 1 second
       digitalWrite(ledPin, LOW);  // Turn the LED off
       delay(1000);                 // Wait for 1 second
     }
     ```
   * This loop will make the LED turn on and off repeatedly every second.

7. **Select the correct board and port**:

   * Go to **Tools → Board → Arduino UNO**.
   * Go to **Tools → Port** and select the port your Arduino is connected to.

8. **Upload the sketch** to your Arduino by clicking the **Upload** button (arrow icon). Wait until the IDE shows “Done uploading.”

9. **Observe the LED** on the Arduino UNO. It should blink on and off at a 1-second interval.

10. **Experiment**:

    * Try changing the delay values to make the LED blink faster or slower.
    * Add comments to your code explaining each step.

## Summary

In this exercise, you learned how to:

* Connect an Arduino UNO to a computer
* Write a basic program to control the built-in LED
* Use `pinMode`, `digitalWrite`, and `delay` functions
* Upload code to a microcontroller

This foundational knowledge is critical for understanding how software interacts with hardware in embedded systems.

## Follow-Up

Once you are comfortable with blinking the LED:

* Try blinking multiple LEDs in sequence using different pins
* Experiment with creating patterns or using buttons to control the LED
* Explore using sensors to control LED behavior based on input

This exercise sets the stage for more advanced embedded projects such as robotics, IoT devices, and interactive electronics.
