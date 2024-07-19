# Multilingual-Voice-based-Translator
This is a simple language translator application built with HTML, CSS, and JavaScript. The app allows users to input text in one language and translate it to another language. Additionally, it includes a text-to-speech feature that reads out the translated text.

## Features

- Translate text between multiple languages
- Text-to-speech functionality
- User-friendly interface with a background image
- Responsive design

## Installation

1. Clone the repository to your local machine:
    ```bash
    git clone <repository-url>
    ```

2. Navigate to the project directory:
    ```bash
    cd Language-Translator-App
    ```

3. Open the `index.html` file in your preferred web browser.

## Usage

1. Enter the text you want to translate in the text area provided.
2. Select the source and target languages from the dropdown menus.
3. Click the "Translate Text" button to get the translated text.
4. Click the "Speak" button to hear the translated text.

## Files

- `index.html`: The main HTML file that contains the structure of the app.
- `style.css`: The CSS file that styles the app.
- `js/script.js`: The JavaScript file that contains the logic for the translation and text-to-speech functionality.
- `js/countries.js`: A JavaScript file that contains the list of supported languages.

## Text-to-Speech Functionality

The text-to-speech feature uses the Web Speech API to read out the translated text. To use this feature, simply click the "Speak" button after translating the text.

```javascript
document.getElementById('speakButton').addEventListener('click', function() {
    var textToSpeak = document.querySelector('.from-text').value;
    var speech = new SpeechSynthesisUtterance(textToSpeak);
    speechSynthesis.speak(speech);
});
