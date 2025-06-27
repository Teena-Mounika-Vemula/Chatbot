# 🤖 ChatBot with OpenAI, LangChain & PlayHT

This project is a voice-enabled AI chatbot built using **LangChain**, **OpenAI's GPT models**, and **PlayHT** for text-to-speech voice synthesis. The chatbot allows for conversational interaction using natural language, with spoken responses delivered through a cloned voice using PlayHT.

---

## ✨ Features

- 💬 Conversational AI powered by **OpenAI GPT (via LangChain)**
- 🧠 Maintains memory across conversation turns
- 🗣️ Converts text responses into **speech using PlayHT voice cloning**
- 🧪 Interactive frontend via **Gradio UI**
- 🔐 Supports secure integration of API keys

---

## 🧰 Tech Stack

| Tool/Service       | Purpose                                      |
|--------------------|----------------------------------------------|
| `LangChain`        | Framework to build LLM-powered applications |
| `OpenAI GPT`       | Natural language processing engine           |
| `PlayHT`           | Voice cloning and text-to-speech conversion |
| `Gradio`           | Lightweight UI for chatbot interaction      |
| `Python`           | Core programming language                    |
| `Jupyter Notebook` | Development and testing interface            |

---

## 🚀 How It Works

1. **User sends a message** via Gradio chat interface.
2. Message is passed to OpenAI's GPT model using LangChain.
3. LangChain maintains the conversation context with memory.
4. The generated text response is sent to PlayHT API.
5. PlayHT synthesizes the response into voice using a **custom cloned voice**.
6. The voice/audio is played back to the user via Gradio.

---

## 🛠️ Installation and Setup

### 🔧 Install Dependencies

In a Jupyter Notebook or terminal:

```bash
pip install langchain
pip install openai
pip install gradio
pip install huggingface_hub
```

### 🔐 API Keys Configuration

#### Get OpenAI API Key
1. Go to: https://platform.openai.com/account/api-keys
2. Click "Create new secret key"
3. Copy the key

#### Get PlayHT API Key and User ID
1. Go to: https://play.ht/
2. Navigate to: https://play.ht/studio/api-access
3. Copy your User ID and generate a Secret API Key

#### Get PlayHT Voice Clone ID
1. Go to: https://docs.play.ht/reference/api-list-cloned-voices
2. Use the "Try It" feature with your Auth Token and User ID
3. Copy a cloned voice ID from the response

### 🧪 Running the Notebook

1. Open the file `ChatBotWithOpenAILangChainAndPlayHT.ipynb` in Jupyter Notebook or VS Code.
2. Replace the following placeholders in the code with your actual keys:

```python
OPENAI_API_KEY = "your_openai_api_key"
PLAY_HT_API_KEY = "your_playht_api_key"
PLAY_HT_USER_ID = "your_playht_user_id"
voice_id = "your_voice_clone_id"
```

3. Run all the cells.
4. The Gradio interface will launch for chat and voice playback.

---

## 🎯 Example Use Cases

- Virtual assistant with real-time voice output
- Language learning bots
- Storytelling or entertainment applications
- Customer service demo bots

---

## 🧑‍💻 Author

**Teena Mounika Vemula**

---

## 📝 License

This project is open source and available under the MIT License.
