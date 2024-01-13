# Multiple Alarm Timer

An interactive web application that allows users to set and manage multiple timers simultaneously. Built using HTML, CSS, and JavaScript.

## Demo
Check out the live demo [here](https://sidd444.github.io/Multiple-Alarm-Timer/).

## Features

1. **Timer Input Section:**
   - Set the desired time in hours, minutes, and seconds.
   - Start a new timer by clicking the 'Start New Timer' button.

2. **Active Timers Display Section:**
   - Dynamically displays all active timers.
   - Each timer shows the time remaining and has a 'Stop Timer' button to cancel it.
   - Timers update every second.

3. **Timer End Display Design:**
   - Upon reaching zero an audio alert is played to notify the user that the timer has ended.

## Functionality

- Timer Functionality: Utilizes the setInterval method in JavaScript to decrement the timer every second. Clears the interval with clearInterval when the timer reaches zero.
  
- Multiple Timers: Each timer has its own interval, stored in an array or object for easy access.

- Audio Alert: The Audio object in JavaScript is used to play a sound upon timer completion.

- Changing the Timer Display: Uses different CSS classes for a timer that has ended. JavaScript changes the class when the timer reaches zero to match the Figma design.

- Handling User Input: Validates user input to prevent unexpected behavior. Ensures a valid time is entered before starting a timer.

- Stopping a Timer: Identifies which 'Stop Timer' button was clicked, using a data attribute on the button that corresponds to the index of the timer in the array/object.

