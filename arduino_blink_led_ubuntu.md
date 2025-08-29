<!--
{
  "ID": "9f2c4b7a1e3d4f6b8a0c2d1e3f4b5a6c",
  "Title": "Arduino UNO Blink LED",
  "Tags": ["Arduino", "Embedded Systems", "LED", "Beginner", "Ubuntu", "C++"],
  "Description": "A beginner-level exercise to blink the built-in LED on an Arduino UNO using Ubuntu.",
  "Query": "Generate a training exercise with the following content: Blink the Built-In LED on Arduino UNO. The focus area of this exercise is: Embedded Software. The difficulty level of the exercise is: Beginner. The target operating system is: Ubuntu. Make the exercise clear, positive, detailed, and comprehensive. Each step of the excercise must be chronologically numbered. Include a hidden section, an overview section, and a prerequisite section before the exercise section. Include a summary section and a follow-up section after the exercise section. The hidden section is wrapped in an HTML style comment tag and includes the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename. Where ID is a randomly generated 32 bit unique ID; Where title is a short title of the exercise; Where Tags is a list of tags associated with the exercise; Where Description is a short overview description of the exercise; Where Query is this query string; Where model is the model and version of this LLM; Where focus is the focus area of this exercise; Where level is the skill level of this exercise; Where date is the current date in the format yyyymmdd; Where Links is a list of helpful web links and resources related to this exercise; Where Filename is a short unique descriptive name for this markdown file.",
  "Model": "GPT-5 mini",
  "Focus": "Embedded Software",
  "Level": "Beginner",
  "Date": "20250828",
  "Links": ["https://www.arduino.cc/en/Guide/ArduinoUno", "https://www.arduino.cc/en/Tutorial/BuiltInExamples/Blink", "https://www.arduino.cc/en/Guide/Linux"],
  "Filename": "arduino_blink_led_ubuntu"
}
-->

# Overview

In this exercise, students will learn how to blink the built-in LED on an Arduino UNO using Ubuntu. This beginner-level activity introduces the basics of embedded software, C++ programming for microcontrollers, and uploading code from a Linux environment. By the end of this exercise, students will understand how to control hardware through software and gain confidence with Arduino programming.

# Prerequisites

Before starting this exercise, students should have:

1. A basic understanding of computers and software installation on Ubuntu.
2. A USB cable compatible with the Arduino UNO.
3. Arduino IDE installed on Ubuntu (you can install it via `sudo apt install arduino` or from the official Arduino website).
4. Basic familiarity with C++ syntax is helpful but not required.

# Exercise: Blink the Built-In LED on Arduino UNO

1. **Connect the Arduino UNO**

   * Plug your Arduino UNO into your Ubuntu computer using the USB cable.
   * Ensure that your computer recognizes the device. You can check by running `ls /dev/tty*` in the terminal and looking for something like `/dev/ttyACM0` or `/dev/ttyUSB0`.

2. **Open Arduino IDE**

   * Launch the Arduino IDE from your applications menu.
   * Ensure that your IDE is up to date to avoid compatibility issues.

3. **Select the Board**

   * Go to `Tools` → `Board` → `Arduino AVR Boards` → `Arduino Uno`.

4. **Select the Port**

   * Go to `Tools` → `Port` and select the port corresponding to your Arduino (e.g., `/dev/ttyACM0`).

5. **Write the Blink Program**

   * In the IDE, create a new sketch.
   * Copy the following code:

     ```cpp
     void setup() {
       pinMode(LED_BUILTIN, OUTPUT); // Initialize the built-in LED pin as an output
     }

     void loop() {
       digitalWrite(LED_BUILTIN, HIGH); // Turn the LED on
       delay(1000);                     // Wait for 1 second
       digitalWrite(LED_BUILTIN, LOW);  // Turn the LED off
       delay(1000);                     // Wait for 1 second
     }
     ```

6. **Verify the Code**

   * Click the **Checkmark** button in the IDE to compile your code.
   * Ensure there are no errors.

7. **Upload the Code**

   * Click the **Right Arrow (Upload)** button to send the code to your Arduino.
   * Wait until the IDE shows “Done uploading.”

8. **Observe the LED**

   * Look at the built-in LED labeled `L` on the Arduino UNO.
   * The LED should blink on and off at 1-second intervals.

9. **Experiment**

   * Try changing the `delay(1000)` value to another number, like `500` for half a second, and observe how the blinking speed changes.
   * Modify the code to blink the LED in a different pattern.

# Summary

You have successfully:

* Connected an Arduino UNO to Ubuntu.
* Written a basic C++ program for embedded systems.
* Uploaded code to the Arduino and observed hardware control.
* Learned how to manipulate the built-in LED using software.

# Follow-Up

To extend your learning:

1. Try adding multiple LEDs to the Arduino and control them in different patterns.
2. Explore other built-in examples in the Arduino IDE.
3. Learn how to use input sensors like buttons or potentiometers to control LED behavior.
4. Experiment with different delay times and patterns to create simple LED animations.

---

If you want, I can also create a **version with embedded diagrams showing the Arduino and LED pin locations** to make it even more beginner-friendly. Do you want me to do that next?
