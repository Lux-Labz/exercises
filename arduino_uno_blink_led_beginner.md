````markdown
<!--
{
  "ID": "1847632910",
  "Title": "Blinking the Built-In LED on Arduino UNO",
  "Tags": ["Arduino", "Embedded Software", "Beginner", "LED", "Programming"],
  "Description": "A beginner-friendly exercise to learn how to blink the built-in LED on an Arduino UNO board using the Arduino IDE.",
  "Query": "You are a STEM instructor and training exercise curriculum creator for students aged 12-18. Geneate a training exercise with the following content: Blink the Built-In LED on Arduino UNO. The focus area of this exercise is: Embedded Software. The difficulty level of the exercise is: Beginner. Make the exercise clear, positive and detailed.  Include all prerequisites, along with suggestions for related and follow-up activities.  Each step of the excercise must be chronologically numbered. Add a dedicated hidden field to the top of the exercise with the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename.",
  "Model": "GPT-5",
  "Focus": "Embedded Software",
  "Level": "Beginner",
  "Date": "20250828",
  "Links": [
    "https://www.arduino.cc/en/software",
    "https://docs.arduino.cc/hardware/uno-rev3",
    "https://www.arduino.cc/en/Tutorial/BuiltInExamples/Blink"
  ],
  "Filename": "arduino_uno_blink_led_beginner.md"
}
-->

# Training Exercise: Blinking the Built-In LED on Arduino UNO

### Overview
This exercise introduces students to **embedded software programming** by using the Arduino IDE to blink the built-in LED on the Arduino UNO board. Students will gain practical experience in coding, uploading, and running their first program on embedded hardware.

---

### Prerequisites
1. Basic familiarity with computers (installing software, navigating files).
2. Arduino UNO board.
3. USB cable (Type-A to Type-B) to connect Arduino UNO to a computer.
4. Arduino IDE installed ([download here](https://www.arduino.cc/en/software)).
5. Curiosity and willingness to experiment.

---

### Step-by-Step Exercise

#### Stage 1: Setting Up
1. Install the **Arduino IDE** on your computer.
2. Connect the **Arduino UNO** to your computer using the USB cable.
3. Open the Arduino IDE.  
4. In the IDE, go to **Tools → Board** and select **Arduino UNO**.
5. In **Tools → Port**, select the correct COM port that shows "Arduino UNO".

#### Stage 2: Writing the Program
6. In the IDE, click **File → Examples → 01.Basics → Blink**.
7. Review the code that opens. The program contains two main parts:
   - `setup()`: runs once at the start.
   - `loop()`: runs repeatedly, creating the blink effect.

```cpp
// Example Blink code
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); 
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH); 
  delay(1000);                      
  digitalWrite(LED_BUILTIN, LOW);  
  delay(1000);                      
}
````

8. The constant `LED_BUILTIN` refers to the onboard LED connected to pin 13.

#### Stage 3: Uploading the Program

9. Click the **checkmark icon** (✓) to verify the code.
10. If verification succeeds, click the **arrow icon** (→) to upload it to your Arduino UNO.
11. Watch the small onboard LED (marked “L” on the board). It should blink once per second.

#### Stage 4: Experimenting

12. Change the number inside `delay(1000);` to another value, such as `500` for faster blinking or `2000` for slower blinking.
13. Verify and upload again to observe the effect. ⚡
14. Try creating your own pattern by combining different delay times.

---

### Reflection

* You just programmed an **embedded system**.
* The Arduino runs your code directly without needing a computer afterward.
* Changing numbers in the code changes the hardware behavior in real time.

---

### Related Activities

* Modify the blink code to create a Morse code signal (e.g., "SOS").
* Use an external LED and resistor on a breadboard instead of the built-in LED.
* Experiment with two LEDs blinking alternately.

---

### Follow-Up Activities

* Explore other **Arduino examples** such as *Fade* or *DigitalReadSerial*.
* Learn about **input devices** (buttons, sensors) and use them to control LEDs.
* Begin writing custom functions to organize and reuse code.

---

Recommendation: Use this exercise to establish confidence in embedded programming fundamentals.
Next step: Progress to controlling external components such as LEDs, buzzers, or sensors.

```
```
