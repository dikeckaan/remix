# Calls Music Remix

Stream in Telegram calls using [GramTGCalls](https://github.com/tgcallsjs/gram-tgcalls).

---

## Features

-   Supports streaming audio files, voice messages, YouTube playlists and YouTube videos, even live ones!
-   Can stream in multiple chats simultaneously, with their own queues.
-   Friendly responses.
-   Doesn't create files.
-   Multilingual.

## Running

1. Copy `example.env` to `.env` and fill it with your credentials.
2. Install dependencies and build:

```bash
npm install
```

3. Start:

```bash
npm start
```

## Deploying to the cloud

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/callsmusic/CallsMusicRemix)

## Deployin with Dockerfile
- Clone the repo and go directory
- Install docker with this
```bash
 sudo apt update && sudo apt install docker.io -y
```
- Then build and run image
```bash
 docker build . -t callsmusicremix
 docker run callsmusicremix
```
## Configuring

- `BOT_TOKEN`: Telegram bot token.
- `STRING_SESSION`: A GramJS/Telethon string session. You can generate one [here](https://rojserbest.github.io/bssg).
- `API_ID`: Telegram app ID.
- `API_HASH`: Telegram app hash.
- `LOCALE`: An [available](./locales) bot language. Default: `en`.
- `MAX_PLAYLIST_SIZE`: Max YouTube playlist size. Default: `10`.

## Commands

### stream

#### _Aliases: s, p, play_

Takes an audio file, voice message or YouTube video link/ID and streams/queues it.

### playlist

#### _Aliases: pl_

Streams a YouTube playlist.

### ns

#### _Aliases: np, cs, cp_

Displays the currently streamed item.

### pause

#### _Aliases: p_

Pauses the stream.

### resume

#### _Aliases: r_

Resumes the stream.

### skip

#### _Aliases: next_

Skips the current stream.

### stop

Clears the queue and removes the userbot from the call.

## Inspiration

-   [eritislami/evobot](https://github.com/eritislami/evobot)

## License

### GNU Affero General Public License v3.0

[Read more](./LICENSE)
