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
<hr>

### `/info`
#### Usage:
   `/info`
#### Purpose:
   Provides elementary information about the bot.
<hr>
   
### `/ping`
#### Usage:
   `/ping`
#### Purpose: 
   Returns the bot’s latency.
<hr>

### `/unicode_info`
#### Usage:
   `/unicode_info <char>`
#### Compulsory Parameters:
   * `string` char - A valid Unicode character. In the case of multiple characters, the first will be taken
#### Purpose:
  Retrieves a Unicode character's name, codepoint, and hexadecimal value.
<hr>

### `/unicode_search`
#### Usage: 
   `/unicode_search <name>`
#### Compulsory Parameters:
   * `string` name - A valid Unicode character name.

#### Purpose:
   Retrieves a Unicode character along with its codepoint and hexadecimal value. Searches by name.
   
## Academic and "HermeriX" Commands
### `/nato`
#### Usage:
   `/nato`
#### Purpose: 
   Returns a chart of the NATO Phonetic Alphabet.
<hr>

### `/semaphore`
#### Usage: 
   `/nato`
#### Purpose: 
   Returns a chart of the Semaphore Alphabet.
<hr>

### `/pigpen`
#### Usage:
   `/nato`
#### Purpose:
   Returns a chart of the Pigpen Alphabet.
<hr>

### `/qr`
#### Usage: 
   `/qr <data> <res>`
#### Compulsory Parameters:
   * `string` data - Data of valid size to store in the QR code. int res - The resolution of the QR code.
#### Purpose:
   Generates a QR code containing custom data
<hr>

### `/code`
#### Usage:
   `/code <language> <link> [<version>] [<stdin>]`
#### Compulsory Parameters:
   * `string` language - Language of the source code
   * `boolean` link - Set this value to `True` if you intend to provide a link to the source code, or `False` if you will be writing the code directly.
   * `int` version - Version of the language
   * `string` stdin - Inputs required by the code (if any), separated by "||"
#### Purpose:
   Runs simple code online using the JDOODLE API. This command will fail if the output is too long, or if Hermeris exceeds the daily compilation limit.                        Consider donating to raise the limit. Click here for a list of supported languages
<hr>

### `/random`
#### Usage: 
   `/code <min> <max> <getint>`
#### Compulsory Parameters:
   * `float` min - The lower limit of the pseudorandom number
   * `float` max - Upper limit of the pseudorandom number
   * `boolean` getint - Set this value to `True` to get a random integer, otherwise enter `False`
### Purpose:
   Returns a pseudorandom number within a range
<hr>

### `/coin_flip`
#### Usage:
   `/coin_flip`
#### Purpose:
   Flips a virtual coin
<hr>

### `/calc`
#### Usage:
   `/calc <expression> [<variables>]`
#### Compulsory Parameters:
   * `string` expression - The expression to evaluate Optional Parameters:
   * `string` variables - The list of variables to use in evaluating the expression
#### Purpose:
   Evaluates a mathematical expression.
<hr>

*The following web-based commands can fail if the API does not return a valid response or if the entered parameters are irrelevant and/or invalid. 
If such a problem persists, please contact AureateHalo.*

### `/search`
#### Usage:
   `/search <query>`
#### Compulsory Parameters:
   * `string` query - The search query Purpose: Performs a DuckDuckGo Instant Search.
<hr>

### `/image_search`
#### Usage:
   `/image_search <query>`
#### Compulsory Parameters:
   * `string` query - The search query Purpose: Performs a Google Image Search.
<hr>

### `/wolfram`
#### Usage:
   `/search <query>`
#### Compulsory Parameters:
   * `string` query - The search query
#### Purpose:
Performs a Wolfram|Alpha computational search. The API makes presumptions based on the query and provides results accordingly (in a series of embeds).
<hr>

### `/web_screenshot`
#### Usage:
   `/web_screenshot <url> <width> <height>`
#### Compulsory Parameters:
   * `string` url - The webpage whose screenshot is to be returned int width - The width of the screenshot in pixels
   * `int` height - The height of the screenshot in pixels
#### Purpose:
   Returns a screenshot of any website (including explicit ones). This command is highly experimental and may not respond if the destination server takes too long to respond to the API.
<hr>

### `/youtube`
#### Usage: `/youtube <query>`
#### Compulsory Parameters:
   * `string` query - The search query
#### Purpose:
   Search YouTube for videos, channels, live streams, etc.
<hr>

### `/grammar`
#### Usage:
   `/grammar <text>`
#### Compulsory Parameters:
   * `string` text - The text to review
#### Purpose:
   Provides simple elementary grammatical corrections and suggestions.
<hr>

### `/abbreviations`
#### Usage:
   `/abbreviations <acronym> <reverse_lookup> [<category>]`
#### Compulsory Parameters:
   * `string` acronym - The acronym to search with
   * `boolean` reverse_lookup - Set this to True to use reverse lookup, or False otherwise
<hr>

#### Optional Parameters:
   * `string` category - Specify a category and filter the results
#### Purpose:
   Searches for full forms of acronyms.
<hr>

### `/anagram`
#### Usage:
   `/anagrams <text>` 
#### Compulsory Parameters:
   * `string` text - The text to search with Purpose: Searches for possible anagrams of a text.
<hr>

### `/poetry`
#### Usage:
   `/poetry <phrase>`
#### Compulsory Parameters:
   * `string` phrase - The phrase to search for Purpose: Find excerpts from poems containing a phrase.
<hr>

### `/text_to_base64`
#### Usage:
   `/text_to_base64`
#### Purpose:
   Converts regular text to base64 (opens a modal to enter text)
<hr>

### `/base64_to_text`
#### Usage:
   `/base64_to_text`
#### Purpose:
   Converts base64 to text (opens a modal to enter text)
<hr>

### `/text_to_caesar`
#### Usage: 
   `/text_to_caesar`
#### Purpose:
   Encodes test using the Caesar Cipher (opens a modal to enter text)
<hr>

### `/caesar_to_text`
#### Usage:
`/caesar_to_text`
#### Purpose:
   Decodes Caesar Ciphertext to regular text (opens a modal to enter text)
<hr>

### `/text_to_vignere`
#### Usage: 
   `/text_to_vignere`
#### Purpose: 
   Encodes test using the Vignere Cipher (opens a modal to enter text)
<hr>

### `/vignere_to_text`
#### Usage: 
   `/vignere_to_text`
#### Purpose:
   Decodes Vignere Ciphertext to regular text (opens a modal to enter text)
<hr>

### `/mono`
#### Usage: `/mono <op>`
#### Compulsory Parameters:
   * `string` op - The new value for each character in the form of a mathematical expression. 
#### Purpose:
   Encodes text using a simple custom monoalphabetic cipher. Accepts text using a Modal. The following predefined variables can be used in the expression op:
   * `int` - The Unicode value of the character in base 10
   * `len` - The length of the input text
   * `pos` - The conventional position of the character in the string.
<hr>

### `/enigma`
#### Usage:
   `/anagrams <rotors> <reflector> <ring_settings> <plugboard_settings> <starting_position>`
#### Compulsory Parameters:
   * `string` rotors - The rotors to use for the Enigma Machine
   * `string` reflector - The reflector to use for the Enigma Machine
   * `string` ring_settings - The ring settings for the Enigma Machine, separated by spaces
   * `string` plugboard_settings - The plugboard connections for the Enigma Machine, separated by spaces
   * `string` starting_positions - The starting position for the Enigma Machine
#### Purpose:
   Manipulates text using a virtual Enigma Machine. Accepts text using a modal. For ease of use, the following is a sample command call:

### `/postalcode`
#### Usage:
   `/postalcode <postalcode> <countrycode>`
#### Compulsory Parameters:
   * `int` postalcode - The postal code with which to search.
   * `string` countrycode - The valid two-character country code for the postal code.
#### Purpose:
   Returns locations of post offices worldwide using a valid postal code. This command will fail if there is an issue with the STANDS4 API, or if the postal code and/or the country code is/are invalid. The table given below contains all the supported country codes:
