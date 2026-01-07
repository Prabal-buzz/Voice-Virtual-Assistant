# Voice Virtual Assistant

A Python-based voice assistant powered by ElevenLabs' conversational AI that provides real-time voice interactions with personalized responses based on your schedule.

## Features

- Real-time voice conversations
- Personalized responses using your schedule information
- Integration with ElevenLabs conversational AI agents
- Audio input/output handling
- Environment-based configuration

## Prerequisites

- Python 3.13 or higher
- ElevenLabs account with API access
- Microphone and speakers/headphones for audio I/O
- macOS (with audio permissions)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Prabal-buzz/Voice-Virtual-Assistant.git
cd Voice-Virtual-Assistant
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install elevenlabs elevenlabs[pyaudio] python-dotenv
```

## Configuration

1. Create a `.env` file in the project root:
```env
AGENT_ID=your_elevenlabs_agent_id
API_KEY=your_elevenlabs_api_key
```

2. Get your credentials from [ElevenLabs](https://elevenlabs.io/):
   - Create an account and set up a conversational AI agent
   - Copy your Agent ID and API Key

## Usage

Run the voice assistant:
```bash
python voice_assistant.py
```

The assistant will:
- Greet you with your name
- Have knowledge of your schedule
- Respond to voice commands in real-time
- Provide helpful assistance

## Customization

### Schedule Information
Edit the `schedule` variable in `voice_assistant.py` to include your personal schedule:
```python
schedule = "Dev Meeting with Team at 08:00; Gym with Satosh at 05:00"
```

### User Name
Change the `user_name` variable for personalized greetings:
```python
user_name = "Your Name"
```

### Agent Prompt
Modify the `prompt` variable to customize the assistant's behavior and personality.

## Troubleshooting

### SSL Certificate Issues
If you encounter SSL errors, run the certificate installation script:
```bash
sudo "/Applications/Python 3.13/Install Certificates.command"
```

### Audio Feedback
- Use headphones to prevent microphone pickup of assistant responses
- Adjust microphone sensitivity in system settings
- Ensure proper audio device permissions

### API Permission Errors
- Verify your ElevenLabs API key has `convai_write` permissions
- Check that your agent allows the configured overrides
- Ensure the agent ID is correct

### Missing Dependencies
If pyaudio installation fails, you may need to install portaudio:
```bash
brew install portaudio
```

## Project Structure

```
voice-assistant/
├── voice_assistant.py    # Main application script
├── .env                  # Environment variables (not in version control)
├── .gitignore           # Git ignore rules
├── .venv/               # Virtual environment (not in version control)
└── README.md            # This file
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source. Please check individual component licenses for details.

## Acknowledgments

- [ElevenLabs](https://elevenlabs.io/) for the conversational AI platform
- Python community for the excellent libraries</content>
<parameter name="filePath">/Users/macbook/Work/voice-assistant/README.md