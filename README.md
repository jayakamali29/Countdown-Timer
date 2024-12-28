# Countdown Timer Web Application

This project is a simple Countdown Timer web application written in HTML, CSS, and JavaScript. The user can input a target date and time, start a countdown to that target, and stop the countdown if needed. Once the target time is reached, the timer will display a "Time's Up!" message.

## Features

- **User Input for Date and Time**: Users can select a target date and time using the `datetime-local` input field.
- **Dynamic Countdown Display**: The countdown timer dynamically updates every second, showing the days, hours, minutes, and seconds remaining until the target date.
- **Responsive and Styled Design**:
  - A visually appealing background image is used to enhance the design.
  - Centered and styled text for better readability.
- **Start and Stop Controls**:
  - Start the countdown with the "Start" button.
  - Stop the countdown with the "Stop" button, which displays "EXPIRED" on the timer.
- **Error Handling**:
  - Ensures that users select a valid date and time.
  - Prevents starting the timer with a past or empty target date.

## Files

### 1. `index.html`
The main HTML file containing the structure of the web application. Key elements include:

- A heading (`<h1>`) for the title "Countdown Timer."
- An input field (`<input type="datetime-local">`) for the user to select the target date and time.
- Two buttons (`<button>`) for starting and stopping the countdown.
- A `<div>` to display the countdown timer.

### 2. Inline CSS
The styles are defined within a `<style>` block inside the `<head>` section of the HTML file. Key styles include:

- Center-aligned text and styled input and button elements.
- A full-page background image with properties like `background-size: cover` and `background-position: center`.
- Custom font families and font sizes for text elements.

### 3. Inline JavaScript
The functionality of the application is implemented using JavaScript within a `<script>` tag. Key functions include:

- **`startCountdown()`**: Initiates the countdown timer. Ensures a valid target date and starts a `setInterval` to update the countdown every second.
- **`updateCountdown()`**: Calculates the remaining time and updates the countdown display. Stops the countdown when the target time is reached and displays "Time's Up!"
- **`pad(num)`**: Ensures that single-digit numbers are displayed with a leading zero.
- **`stopCountdown()`**: Stops the countdown by clearing the `setInterval` and displays "EXPIRED."

## Usage Instructions

1. Open the `index.html` file in a web browser.
2. Select a target date and time using the input field.
3. Click the "Start" button to begin the countdown.
4. View the dynamically updating countdown timer on the screen.
5. Click the "Stop" button to stop the countdown and display "EXPIRED."

## Requirements

- A modern web browser (e.g., Chrome, Firefox, Edge) with support for `datetime-local` input fields and JavaScript.
- An internet connection is required only to load the background image if it's hosted online.

## Customization

1. **Change Background Image**: Update the `background-image` URL in the `<style>` section to use a different image.
2. **Modify Styles**: Adjust the font, colors, or layout in the CSS section.
3. **Add More Features**: Enhance the functionality, such as adding pause/resume buttons or displaying a notification when the countdown ends.

## Known Limitations

- The background image URL is hardcoded. If the link breaks, the background won't load.
- The `Stop` button resets the timer display to "EXPIRED" without preserving the remaining time.
- No sound or notification is provided when the countdown ends.

## Credits

- Background image sourced from [Pexels](https://www.pexels.com/).
- Developed using HTML, CSS, and JavaScript.

