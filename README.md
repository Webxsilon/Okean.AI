# Okean.AI

**Okean.AI** is an open-source project designed to provide an immersive AI role-playing experience. It gives users extensive control over AI models, characters, personas, and various aspects of their conversations.

## Features

1. Local AI and online API support.
2. Character creation and management.
3. Offline conversations.
4. Custom personas.
5. Quick Markdown buttons and shortcuts.
6. User-friendly LLM settings.
7. Character sharing through a dedicated file format (`.axp` — Advanced eXchange Package).
8. Support for Ollama and llama.cpp engines.
9. Background music for a more immersive role-playing experience.

## Requirements

### General Requirements

- Windows 10 / Windows 11.
- At least 8 GB of system RAM (16 GB recommended).
- A 4-core / 8-thread processor or better is recommended.
- At least 2 GB of free disk space for the application itself. Additional space is required for AI models.

### Local AI Requirements

Hardware requirements depend on the selected model, its size, quantization, and context length.

- GPU acceleration is recommended but not mandatory.
- 4–6 GB VRAM can be sufficient for smaller models.
- 8–12 GB VRAM or more is recommended for larger models.
- CPU-only inference is also possible, although generation may be significantly slower.

**Note:** Online API providers have their own requirements and generally do not require a powerful local GPU.

## Installation

### Prebuilt Version

1. Open the [Releases](../../releases) page.
2. Download the latest available release.
3. Extract the downloaded archive into an empty folder.
4. Make sure all application files and folders remain together.
5. Run `Okean.AI.exe`.

You can also create a desktop shortcut for easier access.

### Source Code

1. Click the green **Code** button.
2. Select **Download ZIP**.
3. Extract the archive into an empty folder.
4. Follow the development and build instructions if you intend to run or modify the source code.

## Usage

After installation, launch `Okean.AI.exe` and wait for the application to initialize.

Depending on your preferred AI backend, you may need to install Ollama, configure llama.cpp, or provide an API key.

## Project Structure

| Directory | Description |
|---|---|
| `Character/` | Stores character information and profiles. Do not delete this folder unless you intend to remove its contents. |
| `data/` | Stores conversation history and application data. |
| `llamacpp/` | Contains the llama.cpp backend installation (optional). |
| `models/` | Stores local `.gguf` models used by llama.cpp. |
| `personas/` | Stores custom user personas. |
| `resources/music/` | Stores user-provided music for background playlists. |

**Note:** Some directories may be created automatically when the application starts or when specific features are used.

## Troubleshooting

### 1. llama.cpp is not running

1. Open Settings.
2. Navigate to the **Backend** category.
3. Expand the category.
4. Find and select **Install llama.cpp**.

### 2. Ollama is not running

This may happen when switching from llama.cpp to Ollama.

Make sure Ollama is installed and running on your system. If it is not installed, download it from the [official Ollama website](https://ollama.com/).

### 3. "Pick a model first and install with Ollama if empty"

This message may be outdated or may appear when no suitable model is configured.

**If you are using llama.cpp:**

1. Open Settings.
2. Navigate to the recommended models section.
3. Download one of the suggested models.
4. Alternatively, find the **Or paste a direct .gguf URL** field.
5. Paste a direct download link to a compatible `.gguf` model from Hugging Face and click Download.

**If you are using Ollama:**

1. Open Settings.
2. Navigate to the **AI Settings** category.
3. Find the **Ollama Pull** field.
4. Enter the model name you want to download.
5. Start the download.

**If you are using an online API:**

1. Open the API configuration settings.
2. Enter your API key.
3. Select an available model supported by your provider.

For example, you can use a Gemini model if your API provider supports it.

## License

See the [LICENSE](LICENSE) file for licensing information.

## Terms of Service

See the [Terms of Service](TERMS_OF_SERVICE.md) for the conditions of using Okean.AI.

## Privacy Policy

Okean.AI does not collect, store, or transmit personal user data to its own servers. Conversations, characters, and personas are stored locally on your device.

When using third-party AI APIs, data is sent directly to the selected provider and is subject to their respective privacy policies.

See the [Privacy Policy](PRIVACY_POLICY.md) for more information.
