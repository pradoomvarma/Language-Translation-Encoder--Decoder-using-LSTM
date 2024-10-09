# Language-Translation-Encoder--Decoder-using-LSTM

# Seq2Seq Model with LSTM for French-to-English Translation

This repository implements a sequence-to-sequence (Seq2Seq) model using LSTM layers for translating English sentences into French. The model uses an encoder to process the English input sequence and a decoder to generate the French translation. It is designed for tasks like language translation, where sequences of variable lengths need to be handled.

## Overview

The Seq2Seq model consists of two main components:
- **Encoder**: Processes the input English sentence and outputs a context vector that summarizes the sentence.
- **Decoder**: Uses the context vector and generates the corresponding French sentence, one token at a time.

The repository includes a **sampling model** for inference, allowing the decoder to predict sequences one timestep at a time, using the previous output as input for the next timestep.

## Features

- Seq2Seq architecture with LSTM layers for translation.
- Reverse token lookup for converting predicted indices back to readable characters.
- Handles French-to-English translation during inference by generating English sentences token-by-token.
- Can handle input/output character sequences of variable lengths.
