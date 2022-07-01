# Hermeris: The Manual
The official documentation for Hermeris: *The Sapient Discord Bot* from AureateHalo. Visit https://aureatehalo.com for more information.

<img src="https://aureatehalo.com/Hermeris-4.gif" alt="Hermeris_Logo">

## Note
As of version 5.0.0-beta, Hermeris has an additional `/cmd` feature as an alternative to prefix commands for certain simpler features. A list of those text-based commands are at the end of this document.

## Preface
Thank you for selecting Hermeris as your bot. Hermeris provides special commands for educational and computational purposes, such as solving mathematical equations, providing stock market information, encryption and decryption, and other such functions. As mentioned before, Hermeris is powered by the powerful Wolfram|Alpha API besides the NASA Open API and countless other powerful APIs which provide the backend for most of its commands. The Wolfram|Alpha API provides most services that offer the perfect replacement for innumerable other possible commands.
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
### `/manual`
#### Usage:
   `/botinfo`
#### Purpose: 
   Provides a link to the Hermeris website, with this manual.
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
<hr>

### `/postalcode`
#### Usage:
   `/postalcode <postalcode> <countrycode>`
#### Compulsory Parameters:
   * `int` postalcode - The postal code with which to search.
   * `string` countrycode - The valid two-character country code for the postal code.
#### Purpose:
   Returns locations of post offices worldwide using a valid postal code. This command will fail if there is an issue with the STANDS4 API, or if the postal code and/or the country code is/are invalid. The list below contains all the supported country codes:
```
["AD","AR","AS", "AT", "AU", "AX", "AZ", "BD", "BE", "BG", "BM", "BR", "BY", "CA", "CH", "CL", "CO", "CR", "CZ", "DE", "DK", "DO", "DZ", "EE", "ES", "FI", "FM", "FO", "FR", "GB", "GF", "GG", "GL", "GP", "GT", "GU", "HR", "HU", "IE", "IM", "IN", "IS", "IT", "JE", "JP", "KR", "LI", "LK", "LT", "LU", "LV", "MC", "MD", "MH", "MK", "MP", "MQ", "MT", "MW", "MX", "MY", "NC", "NL", "NO", "NZ", "PH", "PK", "PL", "PM", "PR", "PT", "PW", "RE", "RO", "RS", "RU", "SE", "SG", "SI", "SJ", "SK", "SM", "TH", "TR", "UA", "US", "UY", "VA", "VI", "WF", "YT", "ZA"]
```
<hr>

### `/apod`
#### Usage:
   `/apod`
#### Purpose:
   Returns NASA's Astronomy Picture of the Day". This command will fail if there is an issue with the NASA Open APIs, or if the returned media is neither an image nor a video.
<hr>

### `/neows`
#### Usage:
   `/neows [<count>]`
#### Optional Parameters:
   * `int` count - The number of results. (Set to 5 by default)
#### Purpose:
   Returns results from the NeoWs near-earth asteroid feed. This command will fail if there is an issue with the NASA Open APIs, or if the returned data is too large to fit inside an embed message.
<hr>

### /rover
#### Usage:
   `/rover <rover> <sol> [<camera>]`
#### Compulsory Parameters:
   * `string` rover - The name of the rover whose images are to be retrieved (Spirit/ Opportunity/Curiosity)
   * `string` sol - The sol date for the picture
#### Compulsory Parameters:
   * `string` camera - The rover camera whose image is to be retrieved. See the next page for the list of valid names (refer to the abbreviations).
#### Purpose: 
   Get images captured by the Spirit, Opportunity, and Curiosity Mars Rovers. The table given below contains all the supported camera names for the Mars rover imagery commands:
   
<table>
   <tr>
      <th>Abbreviation</th>
      <th>Camera</th>
      <th>Curiosity</th>
      <th>Opportunity</th>
      <th>Spirit</th>
   </tr>
   <tr>
      <td>FHAZ</td>
      <td>Front Hazard Avoidance Camera</td>
      <td>✔</td>
      <td>✔</td>
      <td>✔</td>
   </tr>
   <tr>
      <td>RHAZ</td>
      <td>Rear Hazard Avoidance Camera</td>
      <td>✔</td>
      <td>✔</td>
      <td>✔</td>
   </tr>
   <tr>
      <td>MAST</td>
      <td>Mast Camera</td>
      <td>✔</td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>CHEMCAM</td>
      <td>Chemistry and Camera Complex</td>
      <td>✔</td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>MAHLI</td>
      <td>Mars Hand Lens Imager</td>
      <td>✔</td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>MARDI</td>
      <td>Mars Descent Imager</td>
      <td>✔</td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>NAVCAM</td>
      <td>Navigation Camera</td>
      <td>✔</td>
      <td>✔</td>
      <td>✔</td>
   </tr>
   <tr>
      <td>PANCAM</td>
      <td>Panoramic Camera</td>
      <td></td>
      <td>✔</td>
      <td>✔</td>
   </tr>
   <tr>
      <td>MINITES</td>
      <td>Miniature Thermal Emission Spectrometer (Mini-TES)</td>
      <td></td>
      <td>✔</td>
      <td>✔</td>
   </tr>
</table>
<hr>

*The majority of the following commands are from SerpApi and API Ninjas (mentioned in the footer of the embeds when executed).*

### `/exercise`
#### Usage:
   `/exercise <muscle>`
#### Compulsory Parameters:
   * `string` muscle - The muscle to search for
#### Purpose:
   Provides workouts for a certain muscle
<hr>
   
### `/facts`
#### Usage:
   `/facts <count>`
#### Compulsory Parameters:
   * `int` count - The number of random facts to return (1-30)
#### Purpose:
   Provides upto 30 random facts.
<hr>

### `/recipes`
#### Usage:
   `/recipes <query>`
#### Compulsory Parameters:
   * `string` query - The search query
#### Purpose:
   Provides recipes
<hr>

### `/ip_lookup`
#### Usage:
   `/ip_lookup <ip_address>`
#### Compulsory Parameters:
   * `string` ip_address - The IP address to locate
#### Purpose:
   Get the location of an IP address
<hr>

### `/invite`
#### Usage:
   `/invite`
#### Purpose:
   Get a Hermeris invite link.
<hr>

### `/status`
#### Usage:
   `/status`
#### Purpose:
   Provides the current status of the Hermeris bot (latency, number of servers, and version)
<hr>

### `/poll`
#### Usage:
   `/poll <title> <options>`
#### Compulsory Parameters:
   * `string` title - The title of the poll
   * `string` options - The options for the poll (1-10)
#### Purpose:
   Creates a simple poll
<hr>

### `/cat`
#### Usage:
   `/cat`
#### Purpose:
   Provides a random cat picture.
<hr>
