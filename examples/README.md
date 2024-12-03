# OpenAI Realtime API Node.js Development Environment Example

## Features

- Bilingual support (English and Spanish)
- Wake word activation
- Voice-based interaction with AI assistant

## Wake Word Activation

- **English**: Say "Hey, Assistant" to start interaction
- **Spanish**: Say "Oye, Asistente" to start interaction

## Prerequisites

### 1. Install Audio Tools

#### SoX (Sound eXchange)
Required for audio recording and processing:

- **macOS**:
  ```
  brew install sox
  ```

- **Linux**:
  ```
  sudo apt-get install sox alsa-utils
  ```

- **Windows**:
  Download from [SoX SourceForge](https://sourceforge.net/projects/sox/)

### 2. Install Node.js Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env` file in this directory with your OpenAI API key and optional language:

```
OPENAI_API_KEY=your_api_key_here
ASSISTANT_LANGUAGE=english  # or 'spanish'
```

## Running the Example

```bash
node node_devenv.mjs
```

### Interaction Flow

1. On launch, the assistant will greet you
2. Wait for the greeting to finish
3. Say the wake word ("Hey, Assistant" or "Oye, Asistente")
4. The assistant will confirm it's listening
5. Speak your request
6. The assistant will process and respond

## Language Support

The assistant supports two languages:
- English (default)
- Spanish

Set the language by modifying the `ASSISTANT_LANGUAGE` in the `.env` file.

## Troubleshooting

- Ensure audio tools are installed
- Check microphone and speaker permissions
- Verify OpenAI API key is valid
- Confirm language setting is correct

If problems persist, check console output for detailed error messages.
