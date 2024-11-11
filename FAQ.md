<p align="center">
  <b><a href="https://github.com/mzivic7/pulsar-discord">Pulsar-Discord</a></b> / <a href="https://github.com/mzivic7/pulsar-discord/blob/main/faq.md">FAQ</a>
</p>

---

# FAQ

- [Custom Playing Status](#playing-status)
- [Rich Presence Is Not Showing](#rich-presence-is-not-showing)
- [Getting debug info](#getting-debug-info)

----

# Playing Status
## Changeable Text
To change other texts like 'Editing a (name) file', follow this steps:

1. **Open i18n file**
Open file located in `(UserDirectory)/.pulsar/packages/pulsar-discord/i18n/(Currently Using Language).json`

2. **Change desired text**
Change content of the json file in order to change your desired text.

## "Playing Pulsar Editor" Text
To change the "Playing Pulsar Editor" text you will need to make a new [discord developer application](https://discordapp.com/developers/applications/), you can do this by repeating the following steps:

1. **Create a new discord developer application**
Click [Here](https://discordapp.com/developers/applications/) and create a new application.

2. **Set your app name and turn on rich presence**
Your app name will later be displayed as `Playing <app-name>`.

3. **Set Client ID to your application**
Copy your `Application ID`.  
And in pulsar-discord package settings change `Settings > Behaviour > Custom Client ID` into your Application ID.  

4. **Upload icons assets**
Download all of the programming languages icons ([available here](https://github.com/HelloWorld017/fileicons-render/tree/main/icons)) and upload them all under Rich Presence > Rich Presence Assets (if you miss one it won't work!). The asset name should be filename of the image (without the `.png`!).

5. **Upload custom image assets**
Now, under same assets, upload the custom image that will replace original Pulsar icon. Imust have asset name `pulsar`.

---

# Rich Presence is not showing
- Check if the Pulsar is added in the games tab.
- Check if the option `Display currently running game as a status message.` is turned on in Discord.
- Restart the Pulsar and Discord.
- Try installing from the source code:

Open the terminal and type the following: `pulsar -p uninstall pulsar-discord`

Then, [reinstall pulsar-discord from the source code](https://github.com/mzivic7/pulsar-discord#installing-from-source-code) and restart Pulsar and discord.

---

# Getting debug info
- Turn on Debug Mode option in package settings
- Restart Pulsar
- Open file `(UserDirectory)/.pulsar/pulsar-discord/Log.txt
