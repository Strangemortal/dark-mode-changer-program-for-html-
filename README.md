# Theme Changer Program

A simple JavaScript program to dynamically change the theme of a webpage based on a toggle input.

## Prerequisites

- Basic understanding of HTML, CSS, and JavaScript.
- A code editor to make changes to the code.

## Usage

1. Include the provided JavaScript code in your HTML file or link it externally.
2. Ensure the correct ID is assigned to the toggle tag (checkbox or range) and the stylesheet tag.
3. Customize the file names of your CSS files according to your project structure.

## How it Works

The program listens for changes in the value of the specified toggle element. Upon change, it updates the href attribute of the linked stylesheet tag, thereby changing the theme of the webpage.

## Implementation

```javascript
const darkModeSlider = document.getElementById('The ID of your toggle tag(checkbox, range)');
const pageStyle = document.getElementById('ID of your stylesheet tag');

darkModeSlider.addEventListener('input', () => {
    const sliderValue = darkModeSlider.value;
    if (sliderValue === '1') {
        pageStyle.setAttribute('href', 'The name of the CSS file for the changed theme with .css extension');
    } else {
        pageStyle.setAttribute('href', 'default CSS file name with .css extension');
    }
});
```

Ensure to replace the placeholder IDs and file names with your actual IDs and file names for proper functionality.


