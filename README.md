# AI Music Generation using LSTM

## Project Overview

This project was developed as part of the CodeAlpha Artificial Intelligence Internship.

The project uses deep learning to generate new musical sequences from MIDI music data. An LSTM (Long Short-Term Memory) neural network is trained on MIDI note and chord sequences and then used to generate new musical events.

## Technologies Used

* Python
* Google Colab
* TensorFlow / Keras
* LSTM Neural Network
* music21
* NumPy
* MIDI
* FluidSynth

## Dataset

The project uses the MAESTRO MIDI dataset for classical piano music.

Dataset: MAESTRO Dataset
https://magenta.tensorflow.org/datasets/maestro

The complete dataset is not included in this repository.

## Project Workflow

1. Collect MIDI music data.
2. Parse MIDI files using music21.
3. Extract notes and chords.
4. Convert musical events into numerical sequences.
5. Create training sequences.
6. Train an LSTM neural network.
7. Generate new musical sequences.
8. Convert generated sequences into MIDI.
9. Convert MIDI into WAV audio.
10. Play the generated music.

## Model

The project uses a two-layer LSTM architecture:

* LSTM layer with 256 units
* Dropout layer
* LSTM layer with 256 units
* Dropout layer
* Dense output layer with softmax activation

The model was trained using the Adam optimizer and sparse categorical cross-entropy loss.

## Generated Output

The trained model generated new musical sequences containing both individual notes and chords.

The generated music was saved as:

* `generated_music.mid`
* `generated_music.wav`

## How to Run

Open `music_generation.ipynb` in Google Colab and run the notebook cells in order.

The notebook performs the following:

* Loads the MIDI dataset
* Preprocesses musical events
* Creates training sequences
* Builds and trains the LSTM model
* Generates new music
* Saves the generated MIDI file
* Converts the MIDI file to WAV audio

## Internship

This project was completed for the CodeAlpha AI Internship.

### Task

Task 3 — Music Generation with AI

## Author

CodeAlpha AI Internship Project
