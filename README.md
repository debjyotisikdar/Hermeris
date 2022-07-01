# Hermeris
The official documentation for the Hermeris Bot

## Preface
Thank you for selecting Hermeris as your bot. Hermeris is a “sapient Discord bot”, meaning that it provides special commands for educational and computational purposes, such as solving mathematical equations, providing stock market information, encryption and decryption, and other such functions. As mentioned before, Hermeris is powered by the powerful Wolfram|Alpha API besides the NASA Open API and countless other powerful APIs which provide the backend for most of its commands. The Wolfram|Alpha API provides most services that offer the perfect replacement for innumerable other possible commands.
Hermeris uses the py-enigma library to provide a virtual Enigma Machine for text manipulation. Please refer to the manual entry on the /enigma command (page 13) for help with the syntax.

## Getting Started
***Refer to the following steps to add Hermeris to your server:***
* Go to the Hermeris Website and select the appropriate invite button to add Hermeris. 
* Alternatively, click here to add Hermeris.

*After adding Hermeris, you should receive a welcome message in the first text channel of the server.*

Hermeris will require a few minutes to reload its extensions and add the guild’s commands for use. If the above-shown embed does not appear and the bot appears offline, it could be due to the following reasons:
* Server outage (please contact AureateHalo in such a scenario)
* Downtime for debugging and upgrades (visit the AureateHalo website for updates)

Occasionally, Hermeris has to be turned off due to the above-mentioned reasons. In some cases, assuming that Hermeris was successfully added to the server, it will send an embed in the first text channel, providing vital information about the shutdown.

As Hermeris a free to use the bot and relies entirely on donations for its hosting, downtimes and performance issues may occur at times. While there is no perfect solution to this, donations always make Hermeris more powerful and robust.
Furthermore, beta versions of Hermeris are highly unstable and should not be used on large servers. They are subjected to frequent shutdowns and connection issues. Users should only use a beta version of Hermeris for testing and experimental purposes or on smaller servers. A beta version of Hermeris may leave any large servers which hinder its performance. Hermeris does not interact through Private Channels. Only `/status`, `/manual`, and `/invite` can be used in Private Channels.

## Utility Commands
### `/help`
#### Usage:
   `/botinfo`
#### Purpose: 
   Shares a copy of this manual with the channel.
   
### `/info`
#### Usage:
   /info
#### Purpose:
   Provides elementary information about the bot.
   
### `/ping`
#### Usage:
   /ping
#### Purpose: 
   Returns the bot’s latency.

### `/unicode_info`
#### Usage:
   `/unicode_info <char>`
#### Compulsory Parameters:
   * `string` char - A valid Unicode character. In the case of multiple characters, the first will be taken
#### Purpose:
  Retrieves a Unicode character's name, codepoint, and hexadecimal value.
  
### `/unicode_search`
#### Usage: 
   `/unicode_search <name>`
#### Compulsory Parameters:
   * `string` name - A valid Unicode character name.

#### Purpose:
   Retrieves a Unicode character along with its codepoint and hexadecimal value. Searches by name.
