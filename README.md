# HoloAssistantAi

**Note:** This README is a draft, and the project, HoloAssistantAi, is currently under development. Some features and details may be subject to change.

HoloAssistantAi comprises several Python modules designed to integrate OpenAI's capabilities with audio processing, weather information retrieval, and gesture recognition.

## Modules Overview

### globals.py

Defines global constants and configuration for the entire suite:

- **Measurement Times:** Variables to track the duration of certain gestures.
- **API Keys:** Keys for OpenAI and OpenWeatherMap APIs.
- **Coordinates:** Latitude and longitude for weather queries.
- **Base URLs and Commands:** URLs for API requests and predefined AI system messages.

### audio.py

Handles audio functionalities including speech synthesis and recognition:

- **Speaker:** Synthesizes speech from text using OpenAI's TTS model.
- **Listener:** Captures and recognizes speech using Google's speech recognition service.

### assistantAi.py

Manages interactions and responses, integrating weather data and OpenAI's chat model:

- **StaticInfo:** Retrieves weather information using coordinates.
- **Assistant:** Controls the flow of activating the AI, generating responses, and managing user interactions.

### handGesture.py

Implements hand gesture recognition using OpenCV and cvzone:

- **HandGestureRecognition:** Recognizes specific hand gestures to control the activation and deactivation of the assistant.

### concate.py

Binds gesture recognition with the assistant's functionalities to create a gesture-controlled assistant system:

- **GestureControlledAssistant:** Manages threads and integrates gesture recognition with the assistant's audio responses.

### main.py

The entry point of the application, managing the lifecycle of the gesture-controlled assistant:

- **Runs gesture recognition thread continuously and manages the assistant's state.**

## Setup and Installation

1. **Dependencies:** Ensure all required libraries are installed, including `openai`, `speech_recognition`, `sounddevice`, `cv2`, `cvzone`, and `numpy`.
2. **API Keys:** Insert valid API keys in `globals.py` for OpenAI and OpenWeatherMap services.
3. **Execution:** Run `main.py` to start the application.

## Usage

Activate the assistant by specific hand gestures in front of your webcam. The system can recognize commands through voice and can provide responses and actions like fetching weather data.

## Contributions

Contributions are welcome. Please create a pull request with your proposed changes.

## License

This project is open source and free to use under the MIT License. Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

- Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
- Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
