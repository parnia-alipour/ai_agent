<p align="center">
  <img src="https://github.com/parnia-alipour/ai_agent/blob/master/for%20readme/g.gif?raw=true" alt="Animated GIF" width="700">
</p>

## Projects:

[Aiva](https://github.com/parnia-alipour/ai_agent/blob/master/AI_agent.json)

About Aiva:

Aiva is a Telegram bot.🤖
Aiva is an amazing chatbot and friend for you, with a soft, calm, and human-like tone. I gave Aiva the ability to avoid providing unnecessary explanations unless the user specifically asks for them.

Aiva can send voice messages. If you ask her to explain something to you via voice, or send her a voice message and ask your questions through audio, she will automatically reply to you with a voice message as well!
Aiva can also search the internet for you, and if you ask for an image, she can find and send one from the internet.
She can even generate images for you. (Keep in mind that I gave her access to a basic image generation model that is completely free. If you want a more powerful model, you can add credits to your Google Gemini account and modify the system prompt a little so that she uses Google Gemini for image generation.)
Aiva has two memory systems, and both of them are extremely powerful:

* **Qdrant Vector Store** for **long term memory**
* **Postgres Chat Memory** for **conversation memory**

Aiva will only respond to you if you provide the correct code name. If you don't provide the correct code name, she will never answer your questions.
You can change the code name.

To use Aiva, change your own name in the System Message of the AI Agent from parnia or پرنیا to your own name. After that, Aiva will be your friend.
You can also change her name if you don't like the name Aiva.



Aiva can use the access you give it to Google Calendar to add events or retrieve existing dates and tell you about them. For example, you can tell Aiva the birthdays of your loved ones, and it will save them for you. Later, if you ask Aiva about a birthday, it can use its access to your Google Calendar to find the date and tell you.

To use Aiva, you need to create a chatbot through BotFather on Telegram, copy its token ID, and enter it into n8n.


Please note: if you use that Gemini model for the agent and tell it "please send me a photo of a queen (or anything)" repeatedly, and the agent doesn't respond, it's probably because it searched that site and got blocked  the site likely detected it as a bot. Come back tomorrow and request a picture on that topic from that site again.
Wikipedia and similar sites don't like slow or unusual requests. If the agent takes too long to respond, they might think it's a bot and block it. (from personal experience)
Aiva can communicate in both **Persian and English**.



Talk with Aiva...

![aiva2](https://github.com/parnia-alipour/ai_agent/blob/master/for%20readme/hello.gif?raw=true)

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


---

[Agent Doctor](https://github.com/parnia-alipour/ai_agent/blob/master/Agent_Doctor.json)


This is a medical agent focused on thalassemia, heart disease, and diabetes. I deployed the machine learning and deep learning models I had developed on a server and built an agent around them. Based on what the models have learned, the agent can assess whether a person may have thalassemia, diabetes, or heart disease.

**Please note:** You should always consult a qualified doctor regarding any medical condition. You should never rely solely on an AI agent for a medical diagnosis, as the agent may occasionally make errors in its assessment.


---

[Analyst Agent](https://github.com/parnia-alipour/ai_agent/blob/master/markets_analyst.json)

This agent is capable of generating signals for financial markets. I have equipped the agent with the ability to calculate support and resistance levels as well as pullbacks. Based on the mathematical calculations it performs in its underlying layer, the agent determines whether the market trend is bullish or bearish.

The agent can analyze cryptocurrency, stock, and forex markets across multiple timeframes:

For cryptocurrencies:

* 1h (Hourly) :Short-term
* 1d (Daily) : Medium-term
* 1w (Weekly) :Long-term
* 1M (Monthly): Multi-year trends

For U.S. stocks:

- TIME_SERIES_DAILY : Daily

- TIME_SERIES_WEEKLY: Weekly

- TIME_SERIES_MONTHLY : Monthly

For forex:

* FX_DAILY : Daily

* FX_WEEKLY : Weekly

* FX_MONTHLY : Monthly


I have also given the agent access to both technical and fundamental analysis. In addition, it can analyze market sentiment and trading volume. By combining all of these factors, the agent provides an assessment of whether the market is likely to move upward or downward. At the end of each analysis, it provides an estimated probability percentage for a bullish or bearish movement.

Important Notice:
Please do not rely solely on this agent when making buying or selling decisions. Financial markets are inherently unpredictable, and the agent's analysis should not be considered financial advice or a guarantee of future market movements. 

I used Alpha Vantage for technical analysis and Alpha Vantage Overview for fundamental analysis of U.S. stocks, so that the agent can perform very good analysis. I also added Twelve Data with the goal of using non-U.S. and international markets, but unfortunately, to access international markets, you must upgrade your Twelve Data account to Premium and make a small change to the prompt to tell the agent to use this tool. In this project, I placed it alongside Alpha Vantage for analyzing U.S. stocks.

For analyzing the forex market, I used Alpha Vantage FX this is a separate tool dedicated to currency pairs (like EUR/USD), not stocks. The agent can analyze currency pairs and provide signals based on the same support/resistance and pullback logic.

CoinGecko, Fundamental Analysis CoinGecko, and Binance Klines are used for both technical and fundamental analysis, but specifically for the cryptocurrency market (such as Bitcoin, Ethereum, etc.), and as mentioned, these tools also calculate support and resistance zones and pullbacks, just like forex.

### 🔴Any attempt to scam, misuse, exploit, or sell this agent through other channels, or to take advantage of other people's lack of knowledge or trust, will be dealt with very seriously and strictly🔴
