# TMP Chat Bot

A simple chat bot for **TruckersMP** (ETS2 / ATS).  
This bot reads your chat log file and can respond with useful commands.  
It also connects to **OpenWeatherMap** for live weather and to **Groq API (LLaMA model)** for AI answers.

---

## ✨ Features
- `!weather <city>` → shows current weather (temperature, feels like, pressure, clouds, wind, sunrise, sunset).  
- `!gpt <text>` → ask AI (LLaMA model via Groq API). The bot will answer in the same language as the question.  
- Works inside the TruckersMP chat (reads the log file).  
- Lightweight and easy to use.  

---

## 🛠️ Setup for Developers

### 1. Clone repository
```bash
git clone https://github.com/GitPolyakoff/chatbot-truckersmp.git
```
## 2. Configure API keys

- Open `Program.cs`
Find this line:
```bash
private const string OPENWEATHERMAP_API_KEY = "YOUR_OPENWEATHERMAP_API_KEY";
```

Get your key here 👉 [OpenWeatherMap](https://openweathermap.org/api)

- Open `secrets.json`
(Right click on the `common/config` project → **Manage User Secrets**)
Insert your Groq key:
```bash
{
  "GROQ_API_KEY": "YOUR_GROQ_API_KEY"
}
```


Get your key here 👉 [Groq Console](https://console.groq.com/keys)

## 3. Build & Run

Compile the project and start the bot:
```bash
\tmp-bot\tmp-bot\bin\Debug\net8.0\tmp-bot.exe
```
---

**🚀 Usage**

- Run the game with TruckersMP.

- Run the bot.

- In chat, type commands:

- `!weather Paris` → shows weather in Paris.

- `!gpt hello` → ask AI.

---

## 🔹 Bot Commands (examples)
`!help`
```bash
User: !help
Bot: 🤖 Hello! I am PolyakoffBot v2, ready to assist you. Commands: !help, !weather <city>, !gpt <question>, !serverinfo, !players, !version, !socials, !events.
```

`!weather <city>`
```bash
User: !weather London
Bot: 🌍 London: Light rain 🌧️ | 🌡️ 14.3°C (feels 12.7°C) | 💧 82% | 🌬️ 5.1 m/s | 📊 1015 hPa
```

`!gpt <your message>`
```bash
User: !gpt who is best driver in truckersmp?
Bot: 🤖 GPT: Hard to say! Many players are skilled, but everyone has their own style. 🚛
```

`!serverinfo`
```bash
User: !serverinfo
Bot: 🖥️ Server: Simulation 1 | 145.239.0.11:443 | Players: 2500/3500 | Queue: 35
```

`!players`
```bash
User: !players
Bot: 👥 Total players online (all servers): 5421
```

`!version`
```bash
User: !version
Bot: 📦 Supported ETS2 version: 1.52.1 | Supported ATS: 1.52.1
```

`!socials`
```bash
User: !socials
Bot: 🔗 My Discord Nickname: polyakoff | Github: github.com/GitPolyakoff |
```

`!events`
```bash
User: !events
Bot: 📅 Events now/soon: Real Operations at 2025-09-20 | Convoy Community Event at 2025-09-25
```

---

## 👥 Credits

**Developers:**
- **polyakoff** - Main developer & project creator
- **lrnsxgod** - Contributor

**GitHub Profiles:**
- [GitPolyakoff](https://github.com/GitPolyakoff)
- [lrnsxdev](https://github.com/lrnsxdev)

**Discord:**
- polyakoff & lrnsxgod

---

## 📌 Notes

- Answers from GPT are short (1–2 sentences), because game chat has limited space.

- The bot only works while the log file is updating (so you must be in TruckersMP).

---
