# TwiviaBot

A trivia game bot for your Twitch chat. To get started, visit [TwiviaBot's channel](https://www.twitch.tv/twiviabot) and use the %join command in its chat. 

## Commands:

**%join - Makes TwiviaBot join your channel.**
 - Only works in [TwiviaBot's Channel](https://www.twitch.tv/twiviabot).
 - Ensure you `/mod TwiviaBot` in your channel so the bot will function properly.

**%part - Makes TwiviaBot leave your channel.**
 - Only works in [TwiviaBot's Channel](https://www.twitch.tv/twiviabot).
 - Does **not** remove points, leaderboard, or cooldown settings.

**%trivia - Starts a trivia game in the channel.**
- A trivia game may be started by any channel member.
- Answers to trivia questions must be a 90% match to be counted as correct.
- The category and difficulty of each question is random. (Coming Soon: Channel owners and moderators will be able to select categories and difficulties.)

**%points - Displays the total points of a user in the current channel.**
- Points are tracked separately in different Twitch channels.

**%leaderboard - Displays the top 5 users with the most points in the current channel.**

**%skip - Skips the current trivia game question.**
- Only the **channel owner** or a **moderator** of the channel may skip a question.
- Does **not** reset the cooldown set for the channel. 

**%cooldown - Displays/Modifies the amount of time before a new trivia game may be started.**
 - To modify a channel's cooldown, use the command `%cooldown [time]` where `[time]` is a number of seconds. ex: `%cooldown 300` (5 minute cooldown)
 - Only the **channel owner** or a **moderator** of the channel may modify the channel cooldown. For all other users, the command will simply display the total and remaining cooldown for the trivia game. 


## Resources:

Bot made using [TwitchIO](https://twitchio.dev/en/latest/index.html). 

Trivia question [database](https://opentdb.com/).

To run bot.py you will need the following environment variables:

```
TMI_TOKEN=oauth:pjwk******************
CLIENT_ID=lgs0w*******************
BOT_NICK=TwiviaBot 
```

You can get your own token, client ID, and bot with a new (or your own) twitch account.