Here’s the same chatbot article in Markdown format:

# Build a Simple Chatbot in Python

Creating a chatbot has become much easier with modern AI libraries. In this article, we’ll build a **basic chatbot** using Hugging Face’s `transformers` library.

---

## Step 1: Install Dependencies
```bash
pip install transformers torch

Step 2: Import Required Libraries
from transformers import pipeline

Step 3: Initialize the Chatbot

We’ll use a pre-trained conversational model:

chatbot = pipeline("conversational", model="microsoft/DialoGPT-small")

Step 4: Chat with the Bot
from transformers import Conversation

# Start a conversation
conversation = Conversation("Hello, how are you?")
result = chatbot(conversation)

print(result)

# Continue chatting
conversation.add_user_input("Tell me a joke!")
result = chatbot(conversation)
print(result)

Output Example
User: Hello, how are you?
Bot: I'm doing great! How about you?

User: Tell me a joke!
Bot: Why did the computer go to therapy? It had too many bugs.

Conclusion

With just a few lines of code, you have a working chatbot. You can extend this by:

Integrating into a web app with Flask/Django.

Using larger models like DialoGPT-medium or gpt2.

Connecting to APIs for real-time data.
