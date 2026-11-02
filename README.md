# Okean.AI

Okean.AI is an open-source AI role-playing application built around **User-First** principles. It gives users extensive control over AI models, characters, personas, conversations, and the overall role-playing experience.

Our goal is to provide an AI experience focused on user freedom, privacy, customization, and control.

## Features

1. **Local AI and Online API Support** — use locally running models or connect to online AI providers using your own API keys.
2. **Character Creation and Management** — create, customize, import, and manage your own AI characters.
3. **Offline Conversations** — chat with locally running AI models without requiring an online AI provider.
4. **Custom Personas** — create and manage personas for your role-playing sessions.
5. **Text Formatting** — format messages using built-in shortcuts and custom formatting syntax.
6. **Customizable LLM Settings** — configure various AI generation parameters.
7. **System Prompt Customization** — edit the system prompt or restore it to its original default version.
8. **Character Sharing** — export and import characters using the `.axp` (Advanced eXchange Package) file format.
9. **Multiple AI Engines** — support for Ollama and llama.cpp.
10. **Background Music** — use background music to enhance your role-playing experience.

## Text Formatting

Okean.AI includes built-in formatting shortcuts to make writing and role-playing more convenient.

| Shortcut | Formatting | Purpose |
|---|---|---|
| `Ctrl + *` | *Italic* | Actions, thoughts, and descriptions |
| `Ctrl + B` | **Bold** | Emphasis and important details |
| `Ctrl + I` | ***Bold Italic*** | Strong emphasis |
| `Ctrl + Q` | Quotation | Dialogue and quoted text |
| `Ctrl + H` | Text Color (Hue) | Custom text colors |

Okean.AI also supports custom formatting syntax:

- `*text*` — italic text.
- `**text**` — bold text.
- `***text***` — bold italic text.
- `"text"` — quotation formatting.
- `[C(#0400ff)]text[C(#0400ff)]` — colored text.

## AI Customization

Okean.AI gives users control over how the AI behaves.

### System Prompt

Users can:
- View and edit the system prompt.
- Customize instructions and AI behavior.
- Restore the system prompt to its original default version whenever needed.

This allows users to customize their role-playing experience without permanently losing the application's original instructions.

## Requirements

### General Requirements

- Windows 10 or Windows 11.
- At least 8 GB of system RAM (16 GB recommended).
- A reasonably modern multi-core CPU.
- SSD storage recommended.

### Local AI Requirements

Hardware requirements depend on the selected model, its size, quantization, and context length.

- A dedicated GPU is recommended but not mandatory.
- 6–8 GB of VRAM can be sufficient for smaller models.
- 12 GB or more of VRAM is recommended for larger models.
- CPU-only inference is possible, but generation may be considerably slower.
- Additional storage is required for downloaded models.

Online API usage has different hardware requirements and does not require the model to run locally.

## Installation

### Downloading the Application

1. Open the project's GitHub repository.
2. Navigate to the **Releases** section.
3. Download the latest available release.
4. Extract the downloaded archive into a folder of your choice.
5. Run `Okean.AI.exe`.
6. Wait for the application to initialize.

Keep the application's files and folders together. Do not move or delete individual application files unless you know what they are used for.

### Downloading the Source Code

1. Open the repository.
2. Click the green **Code** button.
3. Select **Download ZIP**.
4. Extract the archive.

Additional build instructions may be required to compile the application from source.

## Usage

After installing or extracting the application:

1. Launch `Okean.AI.exe`.
2. Select your preferred AI engine.
3. Install or select an AI model, or configure an online API provider.
4. Create or import a character.
5. Create a persona if needed.
6. Start a conversation!

## Project Structure

| Folder | Description |
|---|---|
| `Character/` | Stores character information and character files. |
| `data/` | Stores conversation history and application data. |
| `llamacpp/` | Intended for the llama.cpp backend installation. |
| `models/` | Stores GGUF models used by llama.cpp. |
| `personas/` | Stores custom personas. |
| `resources/music/` | Stores user-provided background music. |

Some folders may be populated automatically when the application is used or when additional components are installed.

Do not delete folders containing user data unless you intend to remove that data.

## Troubleshooting

### llama.cpp is not running

1. Open Settings.
2. Find the **Backend** category.
3. Expand it.
4. Select **Install llama.cpp**.

### Ollama is not running

Make sure Ollama is installed and running on your system.

If you have just switched from llama.cpp to Ollama, you may need to install or start Ollama separately.

### "Pick a model first and install with Ollama if empty"

This message may appear when no model is available.

**For llama.cpp:**
1. Open Settings.
2. Find the recommended models section.
3. Download one of the recommended models.

Alternatively, find the **Or paste a direct .gguf URL** field, enter a valid GGUF download URL, and select Download.

**For Ollama:**
1. Open Settings.
2. Find the **AI Settings** category.
3. Locate **Ollama Pull**.
4. Enter the model name and download it.

**For API providers:**
1. Configure your API key.
2. Select a model available through your chosen provider.

## Privacy Policy

Okean.AI is designed around local data storage and user control.

See the [Privacy Policy](PRIVACY_POLICY.md) to learn how Okean.AI handles user data, local storage, and third-party AI services.

## Terms of Service

See the [Terms of Service](TERMS_OF_SERVICE.md) for the terms and conditions of using Okean.AI.

## License

See the [LICENSE](LICENSE) file.

---

**Okean.AI — Your data. Your choice. Your control.**
