
## Features
- 💡 **Ask general questions** or use code snippets from the editor to query ChatGPT via an input box in the sidebar.
- 💬 **View chat history** with requests and responses.
  - Toggle the display of requests and responses between rendered Markdown and raw text.
  - 📝 **Insert code snippets** from the AI's response into the active editor with corrected indentation.
  - 📋 **Copy code snippets** to the clipboard.
- 📚 **Multiple types of context** available:
  - ❌ No context.
  - 📝 Selected text.
  - 📂 Whole file.
  - 📂🔍 All opened files.
- 🖱️ Right-click on a code selection and run one of the context menu **shortcuts** for your code:
  - 📖 Automatically generate documentation.
  - 🤔 Performs security scan.
  - ♻️ Suggests secure coding.
  - 🐛 Find problems with the code.
  - 💻 Complete the code according to the comments.
- 🚀 See the response as it is being generated **in real time**.
- 💬 Ask **follow-up questions** to the response and maintain conversation context.

## Requirements
To use codeshield, please ensure that the following requirements are met:

* Visual Studio Code version 1.73.0 or later is installed on your system.
* You have an OpenAI API key or ChatGPT access token.

## Installation

To use this extension, install it from the VSCode marketplace.

1. After the installation is complete, you will need to add your OpenAI API key to the extension settings in VSCode. To do this, open the `Settings` panel by going to the `File` menu and selecting `Preferences`, then `Settings`.
2. In the search bar, type `codeshield` to filter the settings list.
3. In the ChatGPT section, enter your API key in the top field

After completing these steps, the extension should be ready to use.

## API Modes

Currently, there are two modes for accessing the API: "ChatGPTAPI" and "ChatGPTUnofficialProxyAPI".
### ChatGPTAPI

To use this extension, you will need an `API key` from OpenAI. To obtain one, follow these steps:

1. Go to [OpenAI's website](https://platform.openai.com/account/api-keys). If you don't have an account, you will need to create one or sign up using your Google or Microsoft account.
2. Click on the `Create new secret key` button.
3. Copy the key and paste it into the `API Key` field in the extension settings.

### ChatGPTUnofficialProxyAPI

To use the ChatGPTUnofficialProxyAPI, you need an OpenAI access token from the ChatGPT web app. You can obtain the access token in either of two ways:

* Use [acheong08/OpenAIAuth](https://github.com/acheong08/OpenAIAuth), which is a Python script to automatically log in and get an access token. This method works only with email and password accounts; it does not support accounts where you authenticate via Microsoft or Google.
* Manually get an access token by logging in to the ChatGPT web app and opening https://chat.openai.com/api/auth/session, which will return a JSON object containing your access token string.

Access tokens last for approximately eight hours.

#### Commands

The following commands are available:

* codeshield: find security issues: This command will perform security scan.
* codeshield: secure refactoring: This command will help the developers for secure coding.


Because ChatGPT is a conversational AI, you can ask follow-up questions to the response. The conversation context is maintained between queries, so you can ask multiple questions in a row. 
To **reset the conversation context**, click `ctrl+shift+p` and select `ChatGPT: Reset Conversation`.

