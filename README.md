# Chord Progression AI

This Python script allows you to generate chord progressions for different musical genres using the power of OpenAI's GPT-3.5 language model. The generated chord progressions are then converted into MIDI files that you can use in your music production projects.

## Prerequisites

Before using the script, make sure you have the following:

- Python (3.7 or higher) installed on your machine.
- An OpenAI API key, which you can obtain by signing up on the OpenAI platform.

## Installation

1. Clone this repository to your local machine.
   
   ```sh
   git clone https://github.com/laceyp99/ChordProgressionAI.git

2. Navigate to the cloned directory.
   
   ```sh
   cd ChordProgressionAI

3. Install the required dependencies using pip.
   
   ```sh
   pip install music21 openai

## Usage

1. Set your OpenAI API key as an environment variable. Replace "YOUR_OPENAI_API_KEY" with your actual API key.
   
   ```sh
   export OPENAI_API_KEY=YOUR_OPENAI_API_KEY

2. Run the script in your terminal.
   
   ```sh
   python m21.py

3. Follow the prompts to input the genre, key, BPM, time signature, and bar length for your chord progression.

4. Once you've provided the necessary information, the script will use the OpenAI model to generate a chord progression for you.

5. The generated chord symbols will be displayed on the console, and a MIDI file will be created in the MIDI Files directory within the same folder as the script.

## Customization

- Genre: Specify the musical genre for which you want to generate a chord progression.
- Key: Input the key in which you want the chord progression to be generated.
- BPM: Set the beats per minute for the generated MIDI file.
- Time Signature: Enter the desired time signature for the chord progression.
- Bar Length: Define the length of the chord progression in bars.

You can also adjust the settings for the OpenAI model by modifying the max_tokens and temperature parameters in the openai.ChatCompletion.create() function to control the length and randomness of the generated output.

## Note

Please keep in mind that this script uses an external API (OpenAI's GPT-3.5) to generate chord progressions. The quality and style of the generated progressions may vary based on the training data and input provided. The temperature of the model is also important to monitor. The higher to 2 the temperature gets, the less consistent formatted responses are given. If you are experiencing errors because the response isn't processed properly, try lowering the temperature.
