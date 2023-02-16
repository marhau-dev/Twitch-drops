# Twitch Drops Tool

This application allows you to AFK mine timed Twitch drops, without having to worry about switching channels when the one you were watching goes offline, claiming the drops, or even receiving the stream data itself. This helps both you and Twitch save on bandwidth and hassle. Everyone wins!

### How It Works:

Every ~60 seconds, the application sends a "minute watched" event to the channel that's currently being watched - this is enough to advance the drops. Note that this completely bypasses the need to download any actual stream video and sound. To keep the status (ONLINE or OFFLINE) of the channels up-to-date, there's a websocket connection estabilished that receives events about streams going up or down, or updates regarding the current amount of viewers.
