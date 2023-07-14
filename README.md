# VoiceChatGPT - Converse with OpenAI ChatGPT Models 🗣️🤖

This is a Python script that allows you to have a conversation with an AI chatbot using speech input and output. The script utilizes the OpenAI API for generating AI responses and the Google Speech Recognition and gTTS libraries for speech recognition and text-to-speech conversion respectively. 

## Prerequisites

Before running the script, make sure you have the following:

- Python 3.x installed on your system ✔️
- An OpenAI API key. You can obtain it from the OpenAI website 🔑
- An active internet connection 🌐

## Setup

1. Clone the repository to your local machine.
2. Rename the provided `.env.example` file to `.env`.
3. Open the `.env` file and replace `OPENAI_API_KEY` with your actual OpenAI API key.
4. Install the required Python dependencies by running the following command: `pip install -r requirements.txt`


## Usage

1. Run the script using the following command: `python chatbot.py` ▶️
2. The chatbot will greet you with an audio message "At your service!" 🎙️
3. Start speaking to the chatbot. It will convert your speech to text using the Google Speech Recognition library and generate an AI response using the OpenAI API 🗣️🔢
4. The chatbot will respond with an audio message. You can listen to the response and continue the conversation 🎧
5. To exit the chatbot, say "exit" or "stop". The chatbot will respond with a goodbye message "It was great chatting with you!" and the script will exit 🚪

Note: The chatbot will wait for up to 3 seconds for speech input. If no speech is detected within that time, it will print a timeout message and continue listening ⌛.

## Customization

You can modify the behavior of the chatbot by making changes to the script:

- You can change the language of the speech recognition and text-to-speech conversion by modifying the `lang` parameter in the `create_audio` function.
- You can experiment with different OpenAI models by changing the `model` parameter in the `generate_response` function. For example, you can switch to the `text-davinci-003` model instead of `gpt-3.5-turbo`.
- Feel free to customize the AI prompts and responses according to your requirements.

## License

The script is released under the [MIT License](LICENSE).

## Disclaimer

This script is provided as-is without any warranty. Please use it responsibly and in accordance with the terms and conditions of the OpenAI API. Be aware of the potential limitations and ethical considerations when working with AI models. ⚠️
