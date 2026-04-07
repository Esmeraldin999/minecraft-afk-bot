<h1><p align="center">🤖 Minecraft AFK Bot</p></h1>
This is the ultimate Minecraft Java AFK Bot powered by https://github.com/PrismarineJS/mineflayer. It connects to a Java server, performs basic movements to avoid AFK detection, to mantain the server online and can be customized via a simple configuration file.

---

## ⚠️ Warning Before You Begin

- Before starting the bot, please make sure that the Offline Mode (Pirated/Not Original) option in the settings section of your Aternos server is active.

- Secure the bot to protect it from monsters in the game.

- Aternos may ban you if it detects that you are using a bot, use this carefully.

---

## ✨ Features

* Connect to Minecraft Java servers (IP + port)
* Customize bot username
* Control chunk loading and memory usage
* Periodic chunk pruning to reduce resource usage
* Auto-movement behavior: step forward/backward, jump, sneak, loop
* Easy configuration via `config.json`

---

## ⚡ Installation

### 1. Clone the repository

```bash
git clone https://github.com/nuekkis/Minecraft-AFK-Bot.git
cd Minecraft-AFK-Bot
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure `config.json (exemple)`

```json
{
  "serverHost": "yourserver.aternos.me",
  "serverPort": 25565,
  "botUsername": "MyBotName",
  "botChunk": 4
}
```

> ⚠️ Make sure the server is in offline mode if you're not using premium accounts.

---

## 🤖 Starting the Bot

```bash
node bot.js
```

On successful connection:

* You'll see `✅ BotName is Ready!` in the console
* After 5 seconds, all loaded chunks are cleared
* Every 20 seconds, any chunks beyond a 6-chunk radius will be removed

---

## ⚙️ Configuration Options (`config.json`)

| Key            | Description                                |
| -------------- | ------------------------------------------ |
| `serverHost`         | IP or domain of your Minecraft server      |
| `serverPort`         | Server port (If the ip is test.aternos.me:**15179**, use 15179)              |
| `botUsername`     | The bot's visible name in-game             |
| `botChunk` | Radius of loaded chunks (recommended: 1–6) |

---

## ⚠️ Notes

* **Skins**: Skins might not appear properly if the server is in offline mode.
* **Sneak Movement**: The bot uses `setControlState('sneak', true)`, but some servers may block or ignore this action.
* **AFK Prevention**: The bot periodically moves, sneaks, and jumps to prevent disconnection due to inactivity.

---

## 📚 Resources & Contributions

* [Mineflayer Docs](https://mineflayer.prismarine.js.org/)
* [PrismarineJS GitHub](https://github.com/PrismarineJS/)

Feel free to contribute by opening a pull request or submitting an issue.

---

## ☁️ Free Cloud Hosting

You may prefer to not run this bot on your own device, in wich case you could run this project in the cloud without downloading anything using the **Github Codespaces** for free or any other cloud hosting service like google cloud shell or Apify.

## 📄 License

This project is licensed under the MIT License.

## 📧 **Contact**

Have questions or feedback? Feel free to open an issue or reach out on [GitHub](https://github.com/esmeraldin999).

Do you want to request a service? Contact us via our [Website](https://esmeraldin.base44.app)

