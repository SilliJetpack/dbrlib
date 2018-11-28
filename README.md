# dbrlib
The library for discord bot reviews

# Download 
    download the 'dbr_lib.zip' 
    
# Documentation

```javascript
const dbr = require("dbr")
const dbrbot = new dbr.dbrbot()

dbrbot.getbot("A bot's ID").then(r=> console.log(r))

dbrbot.getuser("A user's ID").then(r=> console.log(r))

dbrbot.getwidget("Bot ID", "Directory where to save the image")
```


#  botget() options
        clientID - the bot's ID
        prefix - the bot's prefix
        invite_url - the bot's invite url (custom or default)
        support_url - the bot's support server link
        short_description - the bot's short description
        long_description - the bot's long description
        ownerID - the bot's owner ID
        ownerBIO - the bot's owner's biography
        ownerCERTIFIED - returns true if the bot owner is certified
        likes - number of likes the bot has
        dislikes - number of dislikes the bot has
        unique - returns true if bot is certified as "unique"
        veryUnique - returns true if bot is certified as "veryUnique"
        
# userget() options
          id - the user's ID
        biography - the user's biography
        iscertified - returns true if user is certified
        bots - returns an array of bots the user has (including all of its information) (use bots.length if you want the number)
