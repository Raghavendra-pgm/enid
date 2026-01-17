Voice-Controlled Desktop Assistant for Windows
ENID is a Python-based voice assistant designed for practical desktop automation. It listens to voice commands and performs system-level actions such as opening applications, folders, web searches, and playing music, using offline text-to-speech for fast and reliable responses.
Features
Voice recognition via microphone
Offline text-to-speech output
Non-blocking, multi-threaded speech handling
Application launching (Brave, Spotify, Explorer)
Common and custom folder shortcuts
Web search using Brave Search
Spotify playback via URI
Automatic shutdown on inactivity

Requirements
Windows OS
Python 3.8 or higher
Microphone access
Python Dependencies
speechrecognition
pyttsx3
pyaudio

Configuration
All user-specific configuration is centralized, including:
Assistant name
Silence timeout
Application paths
Folder shortcuts
This allows ENID to be adapted to different machines without touching core logic.

How It Works
Audio input is captured from the microphone
Speech is converted to text
Commands are parsed using rule-based logic
System actions are executed via OS calls
Responses are spoken using a dedicated TTS thread
The assistant exits automatically after prolonged silence or on explicit shutdown commands.

Design Philosophy
Local execution over cloud dependence
Deterministic behavior over opaque AI
Minimal complexity, maximum control
Built as a foundation for advanced assistants
Local speech recognition (Vosk / Whisper)

GUI interface

Plugin-based command architecture

LLM-assisted intent understanding
