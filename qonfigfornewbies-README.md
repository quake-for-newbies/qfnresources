				##### QFNBot / Qonfig For Newbies #####

Available commands at the moment :
```
-bo3      Usage : !bo3 @user
  Create a bo3 set with @user, where you can pick your maps using emoji reactions. Consider storing your scores with !scores
  
-cvar     Usage : !cvar [variable] / !cvar [keyword]
  Get info about a precise Quake Live console variable or from keywords. These resources need heavy re-formatting.

-elo      Usage : !elo / !elo [@user] / !elo [steamid]
  Fetch your elo from qlstats.net, or elo for another user. Can be wrong if the user has a private profile, or if qlstats is behaving. I don't manage qlstats.net.

-help     Shows this message
  Pretty straight forward.

-ign      Usage : !ign / !ign [new ingame name]
  Set or show your current Quake Champions in game name.

-insta    Gets the link of tumer's clips channel
  Make me famous, and send me your clips. This is meant to be community-aimed.

-ip       Usage : !ip 123.456.789:27960 (proper ipv4, no domain name)
  Generate a clickable steam link to directly run Quake Live on said IP.

-lfg.qc   Usage : !lfg.qc / !lfg.qc [rank]
  Mention users matching your rank, or provided rank. For now, regions are not implemented.

-lfg.ql   Usage : !lfg.ql / !lfg.ql [elo value]
  Mention users matching your elo, or provided elo. For now, regions are not implemented.

-pingsoff Disable bot's mentions.
-pingson  Enable bot mentions (default).

-cfg.ql Gets the link of our 'basics cvars' config file.

-rank     Usage : !rank / !rank [@user] / !rank [ingame name]
  Fetch your rank from Quake Champions API, or rank for another user.

-scores   Usage (in bot's dm) !scores #gameID <your score> <opponent score>
  Send this in dm to the bot to register ranked games (from !bo3) scores.

-steamid  Usage : !steamid / !steamid [new steam id]
  Fetch or change your steamid. Steam id can be found on your qlstats profile, your steam profile, or in your quake live directory.

-top10.qc Show top 10 players in QC rank.
-top10.ql Show top 10 players in QL elo.
-top10.cap Show top 10 players below the 1100 elo cap.
-top5.qc  Show top 5 players in QC rank.
-top5.ql  Show top 5 players in QL elo.
```
Type !help command for more info on a command.


Available Admin Commands (dm the bot):

	$newcvar <query> - Update a whole Quake Live cvar.
	$cfield <query> <field> <new_value> - Update specific field in Quake Live cvar.
	$offtopic <source_channel> <destination_channel> - Suggest moving an offtopic conversation to a different channel.
	$steamid <your_steamid> - Set or update your Steam ID.
	$users.stats - Show stats for the server's members and registered users.
	$who <search_term> - Search for users by ID, Steam ID, Quake Champions name, or Quake Live Elo.

Keep in mind this is work in progress, please give feedback about errors or wanted features in DM or in #feedback (let's not spam general channels, i already did a bit too much ;))


Love y'all



**TO-DO** :
[]Fix cvar bible (infos in wrong fields, some important variables missing)

[]Split regions for !lfg.ql/lfg.qc (needs roles permissions for the bot)

[]Add try/except to handle errors (eg. message too long when !cvar a common keyword with hundreds of references, 'can't' dm member..)

[]Proper logging

[]Quit function to avoid killing process from terminal

[]Move the !bo3 output to a separate threads (issues to edit the message in there, probably my misunderstanding)

[]Handle insta api? Twitch clips?