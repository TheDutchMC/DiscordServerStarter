# DiscordServerStarter
By TheDutchMC

# What/why?
I have servers running 24/7, but they aren't used all the time. This means that for a couple of hours per day,
no one is using the servers and thus they are just wasting power. I don't like that.

How does this program help fix the issue? Simple, The processes that run on the server, in my case, Minecraft servers,
will check if players are using the server. If no one is online, it'll write that to a file. This is being done with a custom plugin
which I have yet to write. A script will read from those files, location is configurable. If all servers give a no players online,
the script will wait ten minutes and then shut the server down.

Of course, when someone wants to join, it has to be started back up. We do this with a discord bot, the users that want to join need
to type $wakeserver into a Discord chat, the $ can be configured to be something else. This will then send a Wake-on-LAN magic packet to
the server and wake it back up.

What will this program not do? This program will not automatically start your Minecraft server back up, you will have to write a script
for that yourself.
