<p align="center">
  <img src="https://github.com/parnia-alipour/ai_agent/blob/master/for%20readme/g.gif?raw=true" alt="Animated GIF" width="700">
</p>

## Projects:

[Aiva](https://github.com/parnia-alipour/ai_agent/blob/master/AI_agent.json)

About Aiva:

Aiva is an amazing chatbot and friend for you, with a soft, calm, and human-like tone. I gave Aiva the ability to avoid providing unnecessary explanations unless the user specifically asks for them.

Aiva can send voice messages. If you ask her to explain something to you via voice, or send her a voice message and ask your questions through audio, she will automatically reply to you with a voice message as well!
Aiva can also search the internet for you, and if you ask for an image, she can find and send one from the internet.
She can even generate images for you. (Keep in mind that I gave her access to a basic image-generation model that is completely free. If you want a more powerful model, you can add credits to your Google Gemini account and modify the system prompt a little so that she uses Google Gemini for image generation.)
Aiva has two memory systems, and both of them are extremely powerful:

* **Qdrant Vector Store** for **long term memory**
* **Postgres Chat Memory** for **conversation memory**

Aiva will only respond to you if you provide the correct code name. If you don't provide the correct code name, she will never answer your questions.
You can change the code name.

To use Aiva, change your own name in the System Message of the AI Agent from parnia or پرنیا to your own name. After that, Aiva will be your friend.
You can also change her name if you don't like the name Aiva.

Aiva can communicate in both **Persian and English**.


---
[Data Analyst](https://github.com/parnia-alipour/ai_agent/blob/master/data_analyst.json)

This agent has the ability to analyze your data in two different ways and send the analysis to your email.

**First:** You can tell the agent to create a chart for you, select a column, and ask it to count the number of samples in that column. For example, you can select the target column and write: **“Create a diabetes vs. non-diabetes chart for the last column.”** The agent does this very well.

**Note:** Instead of actually creating a traditional chart, it will display a beautiful table showing the number of samples and their percentages in an easy-to-read format.

I had originally chosen a pie chart for this, but I changed my mind and decided to use a table format instead. It creates and presents the table very beautifully.

**Second:** The second agent can analyze each column individually. If you ask it to analyze every column and provide you with the results, it will do exactly that.

I also added a **search capability** to the agent so that it doesn't hallucinate when analyzing columns. For medical datasets, it can search for reliable reference ranges and, when appropriate, identify the normal ranges for different conditions. It can also do this for other types of data where reference ranges are relevant.

For example, with a diabetes dataset, it can tell you what glucose range is generally considered normal for a patient, so you can have accurate and useful information about the specific column you selected and better understand what the data represents.

Both agents can respond in **both Persian and English** and send the results to your email. If you speak Persian, they will analyze the data and send the response to you in Persian. If you speak English, they will do the same in English.
