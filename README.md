<!-- ### *Do NOT download directly from this page but from the releases on the right* ➡ -->

# OBSCord-Snap
**A SAMMI Extension that makes it possible to directly make screenshots from OBS and put them online in Discord.**

**Note: This is a fork of the original version made by Silverlink to work with OBS Websocket V5 and SAMMI (The successor to LioranBoard).**

## IMPORTANT INSTALLATION INSTRUCTIONS
As of time of writing, the SAMMI Bridge has not been updated for OBS Websocket V5. You need to remove the references to the old OBS Websocket library from the bottom of your bridge.html. Easiest way is to just delete the line that looks like this (It's near the very bottom):
```
<script src="https://cdn.jsdelivr.net/npm/obs-websocket-js@4.0.2/dist/obs-websocket.js"></script>
```

Once this is done, install the extension normally (SAMMI Bridge Menu -> Install Extension)

For it to work you need to have set up a webhook in your discord.  
Discord link: https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks

<!-- The Extension includes an example deck with 2 buttons. Practically it's ready to use.  
One button has a chat trigger and the other button has a channel points redemption trigger.  
  
![Example deck screenshot](https://github.com/XSilverlink/LB-OBSCord-Snap/blob/main/Screenshots/LioranBoard_Receiver_1.png) -->

<!-- Included examples:
```
Chat command: !obscordsnap
Channel Point Name: OBSCord Snap
```
Both of these can of course be changed to your liking.

Almost all the commands within these two buttons are commented and should be self-explanatory.  
I made it so you can fill in the variables on each row but you can of course put in the variables directly into the extension. -->

### Prerequisites
* [OBS Studio Version 28 or higher (includes OBS Websocket V5 or higher)](https://obsproject.com/)
* [SAMMI](https://sammi.solutions/)

### Variables
Variable Name | Explanation | Extra Information
------------ | ------------- | -------------
webhookURL* | Discord Web hook URL | [How to create one](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks)
obswsURL | OBS Websocket URL. | Default is localhost:4455
obswsPass | OBS Websocket Password.
sourceName* | The source you want to take a screen off. | This can be a source, scene or group
filePath | The filepath location.  | This needs to be the absolute path ending with the file extension png ex: C:\screenshot.png
optionalText | Add a text to the post that will be created on discord. | This can be auto filled from chat or a channel point redeem.

**Variables marked with a * are REQUIRED variables and need to filled in!**

<!-- Shameless plug: https://twitch.tv/Silverlink -->
