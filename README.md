# Emotion Detection Application

A web-based AI application that performs emotion detection on text statements using IBM Watson NLP library and deployed with the Python Flask framework.

## Project Overview
This project develops an embeddable Watson AI application that analyzes user input text and detects the emotions present:
- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

It also determines the **dominant emotion** from the analysis results and provides a clean user interface deployed via Flask on `localhost:5000`.

## Project Structure
- `EmotionDetection/`: Package containing the Watson NLP emotion detection module.
  - `__init__.py`: Package initialization exposing `emotion_detector`.
  - `emotion_detection.py`: Core function interacting with Watson NLP EmotionPredict API.
- `server.py`: Flask application server with error handling and formatted endpoints.
- `test_emotion_detection.py`: Unit test suite validating emotion predictions.
- `templates/index.html`: Web interface for user text input and result display.
- `static/mywebscript.js`: Frontend JavaScript handling asynchronous requests.
