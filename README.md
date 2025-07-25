# VOTL
[![Build status](https://github.com/FileEditor97/VOTL/actions/workflows/build.yml/badge.svg)](https://github.com/FileEditor97/VOTL/actions/workflows/build.yml)  
[![Crowdin](https://badges.crowdin.net/voice-of-the-lord/localized.svg)](https://crowdin.com/project/voice-of-the-lord)  

**Voice of the Lord** - discord bot written in Java using JDA library.  
Functions:
- Server moderation and sync blacklists;
- Custom voice channels;
- Simple verification with join roles;
- Ticketing.

Visit https://votl.fileeditor.dev/ to learn more about available commands and to view documentation.

## Contribute
- [**Help translate!**](https://crowdin.com/project/voice-of-the-lord)
- [Suggest changes to the documentation](https://github.com/FileEditor97/VOTL-docs)

## Installation
Requirements: Java JDK/JRE 21
#### From source:
1. `git clone https://github.com/FiLe-group/VOTL.git`
2. `cd VOTL`
3. `.\gradlew build`
4. Finally `.\linux-start.sh` or `windows-start.bat`

#### Prebuild jar:
Download latest Release [here](https://github.com/FileEditor97/VOTL/releases/latest).  
Or Snapshot build [here](https://github.com/FileEditor97/VOTL/actions/workflows/build.yml).

#### Docker image:
    docker pull fileeditor/votl
More at [Docker hub](https://hub.docker.com/r/fileeditor/votl).

#### Watchdog service:
Available [here](https://github.com/FiLe-group/VOTL-watchdog).

### Configuration
After first bot launch, folders `data` and `logs` will be created at .jar file location (or other specified location).  
Inside folder `data` file `config.json` must be configured with data as stated below.

#### Config file (data/config.json):
```json
{
    "bot-token": "",
    "owner-id": "owner's ID",
    "dev-servers": [
        "dev server's IDs"
    ],
    "webhook": "link to webhook, if you want to receive ERROR level logs"
}
```

## Inspiration/Credits
Thanks to Chew ([JDA-Chewtils](https://github.com/Chew/JDA-Chewtils) and Chewbotcca bot) and jagrosh (JDA-Utilities)  
[PurrBot](https://github.com/purrbot-site/PurrBot) by Andre_601 (purrbot.site)  
[AvaIre](https://github.com/avaire/avaire) by Senither  
Ryzeon & Inkception for [Discord (JDA) HTML Transcripts](https://github.com/Ryzeon/discord-html-transcripts)
