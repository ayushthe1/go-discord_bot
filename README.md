# go-gopher_discord-bot


This repo contains a simple Bot for Discord in Go, with a basic code organization.
We use:
* [KuteGo API](https://github.com/gaelleacas/kutego-api): an API that retrieve Gophers
* [DiscordGo](https://github.com/bwmarrin/discordgo): a Client that interact with Go servers

## Pre-requisites

Install Go in 1.16 version minimum.

or:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/scraly/learning-go-by-examples/tree/main/go-gopher-bot-discord)

## Build the app

`$ go build -o bin/go-gopher-cli main.go`

or

`$ task build`

## Run the app

First, you can export the token:

`$ export BOT_TOKEN=<your bot token>`

Let's run locally our Bot right now:

```
$ ./bin/gopher-bot-discord -t $BOT_TOKEN
Bot is now running.  Press CTRL-C to exit.
```

or

`$ task bot`

## Test the app

```
$ task bot
task: [bot] ./bin/gopher-bot-discord -t $BOT_TOKEN
Bot is now running.  Press CTRL-C to exit.
```

Now you can tape `!gopher`, `!gophers` and `!random` in the Discord server connected to the Bot ;-).