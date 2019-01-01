This is the current command list for Arcoxia. The bolded ones with the _larger than normal size_ are commands unique to Arcoxia.

Important Stuff You Should Know:
--------------------------------

1. Arcoxia primarily uses the command character `.`.
2. `[ ]` text enclosed in brackets means that it is a necessary argument/option, and must be specified **always**.
3. `( )` text enclosed in parenthesis means that it is optional, and the command would work regardless it was specified or not, albeit in a different manner, to be more specific, it'd resort to the _default_ options.
4. All of the commands mentioned below are to be **preceded by `.`**, for Arcoxia to recognize them as commands.

Tour Commands
=============

These are the commands with tour related functionality. 

- `1v1 (doubles)` - A 1v1 tour is created. (Requires **+** or above)
- `runtour [minutes]` - The tour is automatically started after _n_ minutes. (Requires **+** or above). 

Image Commands
==============

Commands for displaying images.

- `showimg [link]`- Broadcasts the image, if user is (**@** or above), else queues it for approval.
- `showimg [approve/reject]` - Approves or Rejects an image queued.
- `showavatar [avatar number]`- Broadcasts the trainer sprite for the avatar number specified. (Requires **%** or above)
- `imgsearch [pokemon]`- Broadcasts sprites from RGB-BW. (Requires **%** or above)

Anime Commands
==============

Commands for fetching anime details and airing time.

- `a.anime [title]` - Broadcasts the information regarding the title, fetched from AniList. (Requires **+** or above)
- `a.manga [title]` - Broadcasts the information regarding the title, fetched from AniList. (Requires **+** or above)
- `a.airing [title]` - Sends the time left till airing of the next episode of the title. (Requires **%** or above)

Basic Commands
==============

Basic features and some information about the bot.

 - `about` - Basic bot info, with the link to this repo.
 - `git` - Link to this repo
 - `version` - Bot version
 - `help` - Get a link to this guide
 - `time` - Current time for Bot
 - `uptime` - Time since the last bot restart
 - `seen [user]` - Latest data from an user
 - `alts [user]` - List of known alts of an user (Alts detedted from namechanges)
 - `say [text]` - Force to say something

Chat Plugins
============

Misc commands for multiple features:

 - `pick [option1], [option2], [...]` - Choose between multiple options
 - `randomanswer` - Get a random answer
 - `joke` - Get a random joke from the local database
 - `quote` - Get a random quote from the local database
 - `regdate (username)` - Get the register date of a Pokemon Showdown account
 - `regtime (username)` - Get the age of a Pokemon Showdown account, useful for check if an account is autoconfirmed

Commands for getting pokemon info:

 - `translate [move/item/ability/nature], (source lang), (target lang)` - Command for translating pokemon stuff
 - `poke` or `randompokemon` - Get a random pokemon
 - `gen [poke]` - Get pokemon, item, etc generation
 - `viablemoves [poke]` - Get viable moves from a Pokemon
 - `heavyslam [poke], [poke]` - Get heavyslam base power
 - `priority [poke]` - Get priority moves
 - `boosting [poke]` - Get boosting moves
 - `recovery [poke]` - Get recovery moves
 - `hazards [poke]` - Get hazards moves
 
Smogon-related commands:

 - `usagelink` - Get a link to Smogon official usage stats
 - `usage [pokemon], (tier)` - Get usage stats of a pokemon
 - `usagedata [pokemon], [moves / items / abilities / spreads / teammates], (tier)` - Get usage data (common moves, items, spreads, etc) of a pokemon
 - `suspect (tier)` - Get information about a suspect test
 - `setsuspect [tier], [pokemon being suspected, ...], [link to Smogon]` - Set suspect information
 - `deftier [tier]` - Set default tier for `usage` and `suspect` commands

Commands for managing the local database of jokes and quotes:

 - `addquote [id], [text]` - Add a new quote
 - `delquote [id]` - Delete an existing quote
 - `listquotes` - Upload quotes to hastebin
 - `addjoke [id], [text]` - Add a new joke
 - `deljoke [id]` - Delete an existing joke
 - `listjokes` - Upload jokes to hastebin

Moderation
==========

**Mod Settings:** Use `mod (room - optional), [moderation], [on/off]` to enable or disable moderations.

**Moderation Exception:** Use `modex [rank/all]` to change moderation exception for a room.

**Autoban**
 - `ab [user1], [user2], [...]` - Add users to blacklist
 - `unab [user1], [user2], [...]` - Remove users from blacklist
 - `rab [regex]` - Regex ban
 - `unrab [regex]` - Remove a regex ban
 - `vab` - View blacklist

**Zero Tolerance**
 - `0tol [user]` - Checks if an user is in the zero tolerance list
 - `0tol add, [user1]:[level1], [user2]:[level2], [...]` - Add users to zero tolerance list
 - `0tol delete, [user1], [user2], [...]` - Removeusers from zero tolerance list
 - `vzt` - Upload zero tolerance list to hastebin

**Banwords and InapropiateWords:** Saying this words means automute. InapropiateWords requires that words are separated.
 - `banword [phrase]` - Add a banword
 - `unbanword [phrase]` - Remove a banword
 - `vbw` - View banword list
 - `inapword [phrase]` - Add an inappropriate word
 - `uninapword [phrase]` - Remove an inappropriate word
 - `viw` - View inapropiate words list

**Joinphrases:** Configure what phrase Bot says when certain user joins a room. This can be spammable, much caution!
 - `joinphrase [enable/disable]` - Enable or disable joinphrases for a room
 - `joinphrase set, [user], [phrase]` - Set a joinphrase
 - `joinphrase delete, [user]` - Remove a joinphrase
 - `vjf` - View joinphrases list
 
**Note:** Excepted users can use moderation commands in format `command [roomid]Arguments` to set moderation through PM or other room. Example: `ab [lobby]spammer1, spammer2`

Battle
======

Commands for battle feature

**Developing**
 - `evalbattle` - Execute arbitrary JavaScript in a battle context
 - `reloadteams` - Hotpatch teams
 - `reloadbattle` - Hotpatch battle modules
 - `move` - Force a custom move

**Challeges**
 - `blockchallenges` - Block Challenges
 - `unblockchallenges` - Stop blocking challenges
 - `chall [user], [format]` - Send a challenge
 - `challme [format]` - Send a challenge to yourself

**Tournaments Joining**
 - `jointours [on/off]` - Enable or disable tour joining
 - `jointour` - Join a tournament
 - `leavetour` - Leave a tournament
 - `checktour` - Check the tournament (If the bot does not challenge or something)

**Ladder**
 - `searchbattle [format]` - Search a battle and returns the link
 - `ladderstart [format]` - Start laddering (checks every 10 seconds)
 - `ladderstop` - Stop laddering

**Teams**
 - `team add, [name], [format], [http://hastebin.com/raw/example]` - Add a team to Bot teams list
 - `team delete, [name]` - Remove a team from Bot teams list
 - `team get, [id]` - Get a team in exportable format
 - `team check, [id], (user)` - Challenge with a specific team
 - `teamslist` - Upload teams list to Hastebin to view it.

Tournaments
===========

Commands for Tournaments feature

 - `tour` - Start a tournament
 - `tour tier=example, timer=30, users=64, dq=1.5, type=elimination` - Start a tournament with custom and optional parameters
  - **tier**: Tournament format / tier
  - **timer**: Max time (in seconds) before starting the tournament
  - **users**: Max number of users (for singups)
  - **dq**: Minutes for autodq
  - **type**: elimination or roundrobin
  - **scout**: set `scout=off` for enabling scout protection
 - `tourhelp` - Help for `tour command`
 - `tourstart` - Force start a tornament
 - `tourend` - Force end a tornament

Commands for leaderboards system

 - `rank (user)` - View users's ranking (points, wins, finals, semifinals, etc)
 - `top` - View the Top5 in the leaderboard
 - `official` - Make a tournament in progress official (to be counted, see config)
 - `unofficial` - Make a tournament in progress unofficial
 - `leaderboards table, [room]` - Upload the leaderboard table to Hastebin
 - `leaderboards reset, [room]` - Reset leaderboards data
 - `leaderboards setconfig, [room], on, [Win points], [Finalist], [SemiFinalist], [Battle win points], [official/all]` - Activate and set leaderboards configuration
 - `leaderboards setconfig, [room], off` - Disable leaderboards system.
 - `leaderboards viewconfig, [room]` - View leaderboards configuration
 - `leaderboards reset, [room]` - Reset leaderboards data

Games
-----

General commands for managing games:

 - `game [Game Name], arg1=value1, arg2=value2...` - Start a game
 - `endgame` - Force end a game
 - `reloadgames` - Alias of `reload feature, games`

**Hangman** and **Poke-Hangman**. Arguments: maxfails (max number of allowed fails, 0 or no specify this argument for infinite), lang (optional only for Poke-Hangman to change the language of the pokemon stuff). Commands:

 - `g [word/char]` - To guess words or characters
 - `view` - To view the game status
 - `end` - To force end the game

**Anagrams** and **Poke-Anagrams**. Arguments: games (max number of rounds), points (number of ponts for winning), time (time to answer in seconds), lang (optional only for Poke-Anagrams to change the language of the pokemon stuff). Commands:

 - `g [word]` - To guess the words
 - `view` - To view the game status
 - `end` - To force end the game
 
**Trivia**. Arguments: games (max number of rounds), points (number of ponts for winning), time (time to answer in seconds). Commands:

 - `ta [answer]` - To answer the questions
 - `view` - To view the game status
 - `end` - To force end the game

**BlackJack**. Arguments: time (time for each turn in seconds), maxplayers (max number of players) Commands:

 - `in` - To join the game. Use `out` to leave
 - `players` - To view the players list
 - `start` - To start the game
 - `hand` - To view your hand
 - `hit` - To get a new card to your hand
 - `stand` - To finish your turn
 - `end` - To force end the game

**Kunc**. Arguments: games (max number of rounds), points (number of ponts for winning), time (time to answer in seconds). Commands:

 - `g [pokemon]` - To guess the pokemon
 - `view` - To view the game status
 - `end` - To force end the game
 
**Rock, paper, scissors**. Single command game: `rps [rock/paper/scissors]`

**Ambush**. Arguments: roundtime (time per round). Commands:

 - `in` - To join the game. Use `out` to leave
 - `players` - To view the players list
 - `start` - To start the game
 - `fire [user]` - To kill other players
 - `end` - To force end the game

**Pass-The-Bomb**. Arguments: maxplayers (max number of players). Commands:

 - `in` - To join the game. Use `out` to leave
 - `players` - To view the players list
 - `start` - To start the game
 - `pass [user]` - To pass the bomb to another user
 - `end` - To force end the game

Youtube
=======

Commands for Youtube link recognition feature

 - `youtube [on/off]` - Enable / Disable YouTube link recognition

Auto-Invite
===========

Commands for auto-invite feature

  - `reloadroomauth [room]` - Reload roomauth if the autoinvite feature is not working well
  - `getroomauth [room]` - Upload roomauth to hastebin (dev command)

Group Chats
===========

Automated Promotion

 - `setautorank [on/off]` - Enable or disable automated promotion in a room
 - `autorank [rank/off]` - Set the autopromotion rank for all users when joining the room
 - `autorank [user], [rank/deauth]` - Set the autopromotion rank for a single user
 - `listautorank` - Upload the autopromotion list to Hastebin

Welcome private message. This can be spammable, much caution!

 - `wpm [enable / disable]` - Enable or disable this feature in a room. Only for excepted users.
 - `wpm view` - View the welcome private message set in a room
 - `setwpm [message]` - Set the welcome private message for a room
 - `delwpm` - Remove the welcome private message for a room

Developing commands for GroupChats feature

 - `ignoregroupchat [groupchat]` - temporarily ignore a groupchat (to leave a groupchat). Then you must edit the config to make it permanent
 - `unignoregroupchat [groupchat]` - unignore a groupchat
