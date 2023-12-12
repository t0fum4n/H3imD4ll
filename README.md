# Heimdall Discord Bot

## Description
Heimdall is a sophisticated, "ChatGPT" powered, Discord bot focued on cybersecurity and designed to interact with users, manage chat history, and perform various automated tasks related to cybersecurity and threat news aggregation. It integrates Discord and OpenAI's GPT-4 model to provide intelligent and contextual responses about your SIEM alerts or threats in the news as they pertain to your org.

## Features
- **Automated Scripts Execution**: Runs various Python scripts to summarize news feeds, manage alerts, and check vulnerabilities.
- **Chat Interaction**: Responds to user messages in Discord using GPT-4, ensuring contextually relevant and intelligent responses.
- **Chat History Management**: Maintains a history of chat interactions and has the capability to manage its size.
- **Vulnerability Checks**: Executes scripts to check for vulnerabilities for specified agents.
- **Alerts Summarization**: Summarizes alerts stored in a JSON file.
- **Custom Discord Commands**: Includes several Discord commands for users to interact with the bot.

## Future Features
- **Incident Response Case Managment**: Interact with the ClickUp API to CRUD tasks.\
- **More Threat Feeds**: CISA KEV, Twitter, Reddit, etc
- **Lockdown host with chat**: Ask Heimdall to contain a host and he will lock it down from a firewall perspective and begin an analysis of the host to see if it is infected or not.
- **Executive Reporting Help**: Create automations that use Heimdall to generate automated reports for executive digestion. Get information about your stack in context to threat intel and program maturity fed to upper management in a way they can understand. 


## Setup and Installation
To set up the Heimdall Discord Bot, you will need:
- Python 3.x
- Discord and OpenAI API keys
- Required Python packages: `discord.py`, `asyncio`, `subprocess`, and others as per the requirements.

## Configuration
1. Clone the repository.
2. Install dependencies using `pip install -r requirements.txt`.
3. Configure the API keys in the `keys` module.
4. Set up the bot on Discord and obtain the bot token.
5. Run the bot using `python <bot_script>.py`.

## Usage
- **Chat with the Bot**: Mention Heimdall or include 'Heimdall' in your message in Discord.
- **Discord Commands**:
  - `/getvulns`: Check vulnerabilities for a specified agent.
  - `/sumalerts`: Summarize current alerts.
  - `/forget`: Manage chat history size.

## Contributing
Contributions to the Heimdall Discord Bot are welcome. Please follow the standard fork-and-pull request workflow.

## License
[MIT License](LICENSE.md)

---

*Note: This bot is designed for educational and informational purposes and is not intended for production use without proper security measures.*

## Screenshots

Below are some examples of Heimdall Discord Bot in action:

<p align="center">
  <strong>Questioning Heimdall about a Recent Vulnerability</strong><br>
  <img src="pics/logofail.png" alt="Asking Heimdall about a vulnerability not known at training time"><br>
  <em>Heimdall's response to a query about a recent vulnerability.</em>
</p>

<p align="center">
  <strong>Identifying Operating System Based on Vulnerabilities</strong><br>
  <img src="pics/agentosid.png" alt="Identifying Operating System with Heimdall"><br>
  <em>Heimdall identifying an operating system based on listed vulnerabilities.</em>
</p>

<p align="center">
  <strong>Alert Summarization Feature</strong><br>
  <img src="pics/alertsummary.png" alt="Summarizing an alert with Heimdall"><br>
  <em>Heimdall summarizing an alert for easy understanding.</em>
</p>
