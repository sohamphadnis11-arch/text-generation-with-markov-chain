# Markov Chain Text Generator
ProDigy Infotech Internship – Task 3  
Author: Pranay Phepade

--------------------------------------------

## Project Overview
This project implements a Markov Chain based text generator.  
It takes a text corpus, tokenizes it, builds a Markov model, and generates new text sequences based on probability.

--------------------------------------------

## Features
- Simple Markov Chain model
- Random text generation
- Uses only core Python libraries
- Clean and modular code structure

--------------------------------------------

## How the Program Works

### 1. Text Corpus
The function get_corpus() returns the paragraph used for model training.

### 2. Tokenization
The text is divided into individual words using:
tokens = corpus.split()

### 3. Markov Model
A dictionary is created where:
- each word is a key  
- the value is a list of words that can follow it in the text

### 4. Text Generation
A random starting word is chosen and the next words are selected based on the Markov model.

--------------------------------------------

## How to Run

Run the script using:

python your_script_name.py

This will generate a random text output based on the Markov model.

--------------------------------------------

## File Structure

markov_text_generator.py  
README.md

--------------------------------------------

## Example Output

Generated Text:
ProDigy Infotech is a leading IT company. It provides software...

--------------------------------------------

## Conclusion
This project demonstrates a simple implementation of a Markov Chain for text generation.  
You can extend it by adding more text, improving the model, or implementing multi-word token chains.

