# Voice-Assistance-AI 

Voice-Assistance-AI is a Python-based voice assistant designed to perform various tasks using speech recognition and text-to-speech synthesis. The assistant can recognize voice commands, execute tasks like opening applications, sending emails, and much more. This project uses `pyttsx3` for speech synthesis and `speech_recognition` for voice input, along with other utilities.

## Features

- **Voice Command Recognition**: Recognizes and responds to voice commands.
- **Text-to-Speech**: Converts text responses into spoken words.
- **Open Applications**: Commands like "open terminal" or "open camera."
- **Send Emails**: Compose and send emails using voice commands.
- **Search-IP-Address**: Looks for IP Address online and display it.
- **Search-on-YouTube**: Search for a video on Youtube.
- **Search-on-Google**: Searching for a site on Google.
- **Search-on-Wikipedia**: Search on Wikipedia.
- **Customizable Hotkeys**: Start and stop listening with hotkeys.
- **Cross-Platform**: Works on macOS (can be adapted for other platforms).

## Installation

### Prerequisites

- Python 3.11 or higher
- Virtual environment (optional but recommended)

### Clone the Repository

```bash
git clone https://github.com/asandilenkala/Voice-Assistance-AI.git
cd Voice-Assistance-AI
```

### Set Up the Virtual Environment

```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows, use .venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Additional Dependencies for macOS

```bash
brew install portaudio
pip install pyobjc
```

## Usage

1. **Run the Script**:
   
   ```bash
   python main.py
   ```

2. **Give Voice Commands**:
   - "Open terminal" to launch the terminal.
   - "Open camera" to launch the camera.
   - "Send email" to compose and send an email.

3. **Hotkeys**:
   - `Ctrl + Alt + L`: Start listening.
   - `Ctrl + Alt + P`: Pause listening.

## Customization

You can customize the assistant by modifying the `main.py` script:

- **Change Voice**:
  ```python
  engine.setProperty('voice', voices[index].id)  # Set the desired voice by changing the index
  ```
- **Add New Commands**:
  Add new voice commands and their corresponding actions in the `main.py` file.

## Troubleshooting

### Common Errors

- **Error 13 - Must be run as administrator**: Run the script with administrative privileges.
- **Module Not Found Errors**: Ensure all dependencies are installed correctly in the virtual environment.

### macOS Specific Issues

- **Input Event Monitoring**: Ensure that the Python interpreter or IDE is added to the Accessibility Clients list in `System Preferences` -> `Security & Privacy`.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
