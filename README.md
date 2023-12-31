# ✨ Basic Discord Bot

## Includes Command & Event Handler

## ⚙️ Features

- Supports slash commands only
- Support for custom event listeners
- Auto update slash commands for even the slighest changes (down to choice changes within options)
- Automatic name and category generation based on file structure
- Pre existing help command with category + usage information for single commands (command options are automatically generated)
- Automatically updating help command based on new commands
- Delete indivual commands
- Deletion of all commands from Discord at once
- Support for custom command validations `(src/handlers/commandHandler.js)`
- Flexible in case you want to scale (not recommended without TypeScript)
- Easy to understand as logic is split to its own files

## 🪜 Steps to get your bot up and running.

- Clone this repo
- Add your bot token in `.env`
- Change the settings in `config.json` to your likings (you can leave out the guildId if you want to register your commands globally - this can take up to an hour)
- Run `npm install` or `yarn` to install all the packages
- Run using `node src/index.js`

## 🧾 Commands + Events information

To get more information on how a command/event is created/structured, open the respective folder and check its README.md file.

## 🗑 Delete all your commands from Discord

I created the `src/exec` directory to add any files that should be ran individually for special use cases. I've encountered during developments you may want to delete all the commands that your bot currently has registered.
To delete all your commands run `node src/exec/delete-all-commands.js`
**This file will only run if you have all the dependencies installed + have a clientId and testServer in your `config.json`**

## 🤔 Help

If you need any help I'll be happy to help. Contact me on Discord: notsikey

_I don't plan on updating this repository as I started this project to get the basics of Discord.js down._
