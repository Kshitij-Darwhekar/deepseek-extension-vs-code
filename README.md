# DeepSeek Extension for VS Code

## Overview
The **DeepSeek Extension for VS Code** enables seamless interaction with the **DeepSeek-R1:8B model** running locally via **Ollama**. With this extension, you can generate AI-assisted code completions, answer queries, and enhance your coding workflow without relying on cloud-based APIs.

## Features
- **Interact with DeepSeek-R1:8B Locally**: Send prompts to the model running via Ollama.
- **Inline Code Suggestions**: Get AI-generated code snippets directly within the editor.
- **Chat Panel**: Open a dedicated chat panel to interact with DeepSeek-R1:8B.
- **Customizable Prompts**: Adjust input settings to fine-tune model responses.
- **Lightweight & Privacy-Focused**: Works entirely offline once the model is downloaded.

### Screenshot Example:
![DeepSeek Extension in Action](images/deepseek-extension.png)

## Requirements
Before using this extension, ensure you have the following:

1. **Ollama Installed**: Install Ollama from [ollama.ai](https://ollama.ai) and download the DeepSeek-R1:8B model:
   ```sh
   ollama pull deepseek-r1:8b
   ```
2. **Node.js & npm Installed** (for extension development)
   ```sh
   node -v
   npm -v
   ```
3. **VS Code v1.75+**

## Installation
1. Install this extension from the VS Code Marketplace (or manually load it in Developer Mode).
2. Ensure Ollama is running with the DeepSeek model:
   ```sh
   ollama serve
   ```
3. Open VS Code and start interacting with DeepSeek via the command palette (`Ctrl+Shift+P` > `DeepSeek: Open Chat`).

## Extension Settings
This extension contributes the following settings:

- `deepseek.enable`: Enable/disable the extension.
- `deepseek.model`: Specify the DeepSeek model to use (e.g., `deepseek-r1:8b`).
- `deepseek.temperature`: Adjust randomness of responses.

## Usage
- **Chat with DeepSeek**: Use the command `DeepSeek: Open Chat` to start a conversation.
- **Inline Completions**: Type comments or code snippets, and the model will suggest completions.
- **Custom Commands**: Define your own prompt templates for specific use cases.

## Known Issues
- The extension may not work if **Ollama is not running**.
- Large prompts may slow down response times.

## Release Notes
### 1.0.0
- Initial release with basic chat and code generation features.

### 1.1.0
- Added support for inline suggestions.
- Improved prompt customization options.

## Following Extension Guidelines
We follow the [VS Code Extension Guidelines](https://code.visualstudio.com/api/get-started/extension-anatomy) to ensure the best practices in extension development.

## Useful Resources
- [Visual Studio Code Extension Documentation](https://code.visualstudio.com/api)
- [Ollama Documentation](https://ollama.ai/docs)
- [DeepSeek AI Model Info](https://deepseek.ai/)

---

Enjoy using DeepSeek in VS Code! 🚀
