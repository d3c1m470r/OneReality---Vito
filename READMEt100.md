# Features
- You can speak to it with a mic
- It can speak back to you in style of the t-100 from t2.
- Has short-term memory (can remember things from the current conversation. Multi-conversation memory would take too long to respond and cost too much on the OpenAI API)
- Can open apps as long as you specify the app path in the code

# Future Features
If you think you can help with any of these or make any other improvements, please don't hesitate to contact me on Discord: DogeLord#2023
- Mac and Linux support
- Mobile version
- Easier setup
- Compiling into one exe


# How it works
First, the Python package SpeechRecognition recognizes what you say into your mic, then that speech is written into an audio (.wav) file, which is sent to OpenAI's Whisper speech to text transcription AI, and the transcribed result is printed in the terminal and sent to OpenAI's GPT-3, then GPT's response will be printed in the terminal and translated to Japanese, which will also be printed in the terminal, and finally, the Japanese translation will be sent to the VoiceVox text to speech engine and will be read out in an anime girl-like voice (It sounds like Megumin from Konosuba). All of this happens in approximately 7-11 seconds, depending on the length of what you say, the length of what the AI says, and your GPU (slightly).

# Install
This tutorial is for Windows only right now.
 1. [Purchase an OpenAI API key](https://www.windowscentral.com/software-apps/how-to-get-an-openai-api-key). It's extremely affordable, since it's pay as you go, and I've been using it for a couple minutes a day like 3 times a week and I got charged less than a dollar for this month.
 2. [Install Python](https://www.python.org/downloads/) and set it as an environment variable in PATH
 3. [Download the latest release](https://github.com/DogeLord081/OneReality/releases/latest)
 4. [Download VoiceVox Engine](https://github.com/VOICEVOX/voicevox_engine/releases/latest), if you're using an Nvidia GPU like me, click Windows（GPU/CUDA版)
  5. Extract the OneReality-main folder so that it is only one folder deep
  6. Extract the VoiceVox folder so that it's also only one folder deep and drag the folder into the OneReality folder
  7. Install the Python dependencies with pip by running `pip install -r requirements.txt` in cmd or powershell
  8. Edit the code in OneRealityJPPublic.py according to the comments within the code (you don't have to do anything complicated, just edit some filepaths and the OpenAI API key)
  9. Add an empty text file in the OneReality-main folder called "conversation.txt"
  10. Run OneReality.bat and you're good to go! If you run into any issues, let me know on Discord and I might be able to help you. Once again, it's DogeLord#2023
