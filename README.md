<img width="150" height="150" align="right" style="float: right; margin: 0 10px 0 0;" alt="music_disc" src="https://cdn.discordapp.com/attachments/1082982687163306058/1086906431783051314/discord-avatar-512-CDL4F.png">

# GardiMusic 

<a href="https://github.com/hmes98318/Music-Disc/releases"><img alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/hmes98318/Music-Disc?style=for-the-badge"></a> 
<a href="https://discord.js.org/"><img src="https://img.shields.io/badge/Discord.JS-v14-blue?style=for-the-badge&logo=DISCORD" /></a> 
<a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node%20Version->=16.13.0-brightgreen?style=for-the-badge&logo=Node.js"></a> 
<a href="https://github.com/hmes98318/Music-Disc/blob/main/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/hmes98318/Music-Disc?style=for-the-badge&color=brightgreen"></a>  

### Discord.js v14 Music Bot  
Supports **YouTube**, **Spotify**, **SoundCloud** streams.


### Reference version  
[**node.js  `v18.12.1`**](https://nodejs.org/en/)  
[**discord.js  `v14.7.1`**](https://www.npmjs.com/package/discord.js)  


## Deploying with node.js

### Clone the repository
```
git clone -b v1.2.6 https://github.com/hmes98318/Music-Disc.git
```
or [**click here**](https://github.com/hmes98318/Music-Disc/releases) to download 
and also this is credited to original creator of this code but i modifed the script


### Install the dependencies
auto install all dependencies on [`package.json`](./package.json)  
```
npm install
```

### Configure environment
[`.env`](./.env) 
```env
TOKEN = "your_token"
NAME = "GardiMusic"
PREFIX = "g+"
PLAYING = "g+help | GardiMusic"
COLOR = "#FFFFFF"
DEFAULT_VOLUME = 93
MAX_VOLUME = 100
AUTO_LEAVE = true
AUTO_LEAVE_COOLDOWN = 5000
DISPLAY_VOICE_STATE = true
PORT = 33333
```
**`AUTO_LEAVE`** : After the music finished, can choose whether let the bot leave voice channel automatically or not.  
**`AUTO_LEAVE_COOLDOWN`** : Timer for auto disconnect(ms).  
**`DISPLAY_VOICE_STATE`** : Show voice channel status updates.   

## Running the script 
```
npm run start
```


## Deploying with Docker Compose  
**image link** : https://hub.docker.com/r/hmes98318/music-disc  
### put your Token into [`docker-compose.yml`](./docker-compose.yml)
```yml
version: '3.8'
services:
  gardi-music:
    container_name: gardi-music
    restart: always
    environment:
      TOKEN: "your_token"
      PREFIX: "g+"
      PLAYING: "g+help | GardiMusic"
      COLOR: "#FFFFFF"
      DEFAULTVOLUME: 50
      MAXVOLUME: 100
      AUTO_LEAVE: "true"
      AUTO_LEAVE_COOLDOWN: 5000
      DISPLAY_VOICE_STATE: "true"
    ports:
      - 33333:33333
```

### Start the container  
```
docker-compose up -d
```


## join support server
https://discord.gg/2XdwkeXmzw

and i credits to hmes98318

