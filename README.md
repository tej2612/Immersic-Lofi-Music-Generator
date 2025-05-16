# Immersic: Ambient Music Generation using LSTM

Immersic is a deep learning project that generates ambient music using Long Short-Term Memory (LSTM) networks. The model is trained on a diverse dataset of MIDI files, primarily focusing on generating ambient LOFI piano  music.

## Project Overview

This project aims to create unique ambient music by training an LSTM model on a curated dataset of MIDI files. The model learns patterns from existing compositions and generates new musical sequences that maintain the ambient music style.

## Dataset

The project uses a collection of 250 MIDI (Musical Instrument Digital Interface) files. MIDI files contain detailed musical information including:
- Pitch (which note is being played)
- Timing (when notes start and stop)
- Velocity (how forcefully notes are played)

### Dataset Source
- [Lo-fi Samples Collection](https://github.com/nmtremblay/lofi-samples)

### Dataset Characteristics
The dataset includes:
- Piano compositions
- Lo-fi music samples
- Ambient music pieces
- Various chord progressions
- E-Piano and Rhodes samples

### Musical Analysis
- Most frequent notes in the dataset:
  1. E-
  2. E
  3. F

The dataset is processed to extract these musical features, which are then used to train the LSTM model.

## Project Structure

- `Main.ipynb`: Main notebook containing the LSTM model implementation and training
- `Preprocessing.ipynb`: Notebook for preprocessing MIDI files and extracting features
- `Dataset/`: Directory containing the MIDI dataset
- `notes.json`: Processed musical features extracted from MIDI files
- `Final_Output.wav`: The generated music sample after adding a drum beat to the piano notes

## Setup Instructions

### Prerequisites
- Python 3.x
- TensorFlow
- music21
- Other required libraries (specified in the notebooks)

### GPU Setup (Optional)
For better training performance, you can set up GPU support:
1. Install CUDA Toolkit
2. Install cuDNN
3. Install GPU-enabled TensorFlow

## Usage

1. **Data Preprocessing**:
   - Run `Preprocessing.ipynb` to process MIDI files
   - This will generate `notes.json` containing extracted features

2. **Model Training**:
   - Run `Main.ipynb` to train the LSTM model
   - The notebook includes functions for:
     - Loading and preparing data
     - Building and training the LSTM model
     - Generating new music sequences
     - Analyzing training data and results

## Features

- MIDI file processing and feature extraction
- LSTM-based music generation
- Support for both GPU and CPU training
- Data analysis and visualization 
- Music generation with customizable parameters

## Model Architecture

The project uses an LSTM (Long Short-Term Memory) neural network to learn patterns from the training data. The model is designed to:
- Process sequences of musical notes and chords
- Learn temporal dependencies in music
- Generate new musical sequences that maintain the style of the training data

