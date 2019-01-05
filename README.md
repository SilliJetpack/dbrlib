# dbrlib
The library for discord bot reviews

# Download 
    download the 'dbr_lib.zip' 
    
# Documentation

```javascript
const dbr = require("dbr")
const dbrbot = new dbr.dbrbot()

dbrbot.getbot("A bot's ID").then(r=> console.log(r)) // Get a bot's info

dbrbot.getuser("A user's ID").then(r=> console.log(r)) // Get user info

dbrbot.getwidget("Bot ID", "Directory where to save the image", "Type (alt or default)", "style (object)") // Get a bot's widget

dbrbot.post("Bot ID", "Token", "Server Count") // Post server count to the API
```



#  getbot() options
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
        source - the bot's source page 
        server_count - the bot's posted server count
        
# getuser() options
          id - the user's ID
        biography - the user's biography
        iscertified - returns true if user is certified
        bots - returns an array of bots the user has (including all of its information) (use bots.length if you want the number)
        background_image - the user's profile page background
        website - the user's personal website
        pulse_color - the user's avatar pulse color (if it's customized via edit page)
        certified_bots - returns array of certified bot IDs
        animation_time - the user's custom animation time
        
 # getwidget() options
   type - the widget type (default for normal one, alt for the alternate one, see API page to see what it is)
   style - the object for customization for the widget (see API page for customization)
