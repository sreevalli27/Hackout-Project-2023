# Hackout-Project-2023-

Our Problem Statement -

Create an AI-driven Depression Symptom Analysis and Therapy Assistant that records audio from individuals discussing their depression symptoms, transcribes the conversation to text, and utilizes a pretrained language model (LLM) to provide therapeutic guidance and support.

This code performs noise cancellation on an audio file using noisereduce, runs the audio through Whisper's speech recognition to transcribe it, and then classifies the transcript using GPT-3.

## Imports
- noisereduce - for noise cancellation
- soundfile - for reading/writing audio files
- whisper - for speech recognition
- openai - for GPT-3 classification

## Functions
- reduce_noise() - Removes noise from audio using noisereduce library. Can remove both stationary and non-stationary noise.

- whisper_transcribe() - Runs Whisper speech recognition on audio file to transcribe speech to text.

- classify_conversation() - Uses GPT-3 to classify text into a Maslow need category.

- generate_therapist_response() - Generates a therapist-like response to the classified conversation using GPT-3.

## Usage
Load audio and sample rate
Reduce noise using noisereduce
Save denoised audio to file
Run Whisper transcription on audio file
Classify transcript text using classify_conversation()
Generate therapist response using transcript and classification
Save classification and response to file

## So in summary:

Denoise audio
Transcribe with Whisper
Classify transcript with GPT-3
Generate response with GPT-3
Save results
This gives a full pipeline from noisy audio to classified/generated text output.
