=======================================================
           LMBOT STATUS MONITOR V1.0.0 - USER MANUAL
=======================================================
Dev by : sigasaga x doubleaitech
Support: https://buymeacoffee.com/sigasaga
=======================================================

Welcome to LMBot Status Monitor! This lightweight tool 
runs in the background to monitor your game bot and 
sends real-time alerts to your Discord server if the 
bot crashes or comes back online.

-------------------------------------------------------
1. INITIAL SETUP (FIRST TIME RUN)
-------------------------------------------------------
Step 1: Place 'LMBotStatus.exe' in a folder of your choice.
Step 2: Double-click 'LMBotStatus.exe' to run it.
Step 3: A black terminal window will appear briefly. It 
        will notify you that a 'config.txt' file has been 
        auto-generated, and then the program will close.
Step 4: Look in the same folder. You will see the newly 
        created 'config.txt' file.

-------------------------------------------------------
2. ADDING YOUR DISCORD WEBHOOK
-------------------------------------------------------
To receive alerts, you need a Discord server and channel.

If you don't have a Server or Channel yet:
1. Open Discord, click the '+' icon on the left sidebar 
   to "Add a Server", and select "Create My Own".
2. Once your server is created, hover over "Text Channels" 
   on the left and click the '+' icon to create a new 
   channel (e.g., name it 'bot-alerts').

How to get a Webhook URL:
1. Click the 'Edit Channel' (gear icon) next to your 
   newly created text channel.
2. Go to 'Integrations' and click 'Webhooks'.
3. Click 'New Webhook' (or 'Create Webhook').
4. Click the 'Copy Webhook URL' button.

How to apply it:
1. Open the 'config.txt' file.
2. Look for the line at the bottom that says: 
   Webhook=PASTE_URL_HERE
3. Replace 'PASTE_URL_HERE' with your actual Webhook URL.
4. Save the file (Ctrl + S) and close it.

*NOTE: If you manage multiple customers and want to send 
alerts to their respective Discord servers, simply add a 
new line for each customer's webhook. 
Example:
Webhook=https://discord.com/api/webhooks/111/customer1...
Webhook=https://discord.com/api/webhooks/222/customer2...

-------------------------------------------------------
3. RUNNING THE MONITOR
-------------------------------------------------------
Once your webhook is saved in 'config.txt', double-click 
'LMBotStatus.exe' again.

The window will display: "Monitoring bot... Do not close!".
Leave this window open (you can minimize it). The software 
is now actively watching your bot!

-------------------------------------------------------
4. ADVANCED SETTINGS (Optional)
-------------------------------------------------------
Inside 'config.txt', you can also change the core settings:

- ProcessName=LordsMobileBot
  (Change this if your bot's executable file has a 
  different name. Do not include the .exe extension).

- CheckInterval=10
  (This is how often the software checks the bot, in 
  seconds. The default is 10 seconds).

-------------------------------------------------------
5. IMPORTANT LIMITATIONS & DISCLAIMERS
-------------------------------------------------------
Please take note of the following limitations before using 
this software:

- Crash/Restart Only: This tool ONLY monitors if the 
  LordsMobileBot client crashes, closes, or restarts. 
- No Heartbeat Detection: It DOES NOT support "heartbeat" 
  monitoring. If the bot freezes or gets stuck but the 
  process is still running, it will not trigger an alert.
- Internet Connection Required: If your PC loses internet 
  connection, this application will NOT be able to send 
  any status updates or offline alerts to your Discord.

=======================================================