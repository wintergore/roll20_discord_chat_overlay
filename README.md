# roll20_discord_chat_overlay
Attempting to create a roll20 chat overlay that works with discord, when players speak their character image lights up, optionally replaces the ingame camera/pictures.

edit test

Follow this guide for initial setup.

Create a browser extension, or a 

li.voice-state > img:not([data-reactid*="11838"]) // use this for selecting all other users.
li.voice-state:first-of-type {
    margin-right: 40px;
}


-- CORS policy prevents iframe injection so can't use the easy route...

-- Browser extentions (get a boilerplate)
- uses an API key for discord (not mine).
- accept array of [userID, non speaking image, speaking image, non speaking brightness]
- start and stop talking event for each user.
- mimics the streamkit 'show who's talking' setup
- extension injects iframe src into the page. --start here??