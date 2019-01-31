# MTGA Pro Tracker
MTGA Pro Tracker is advanced Magic The Gathering Arena tracking tool designed to automatically upload collection, decks, battles, draft and inventory from your game client to our server. No manual collection input, no manual uploads. New cards, battles, drafts are added immediately after events are happening in the game.

## What can I do with MTGA Pro Tracker?
* Real Time Collection & Decks Import
* Share Progress and Wins/Losses
* Track your Wildcards, Boosters and Vault
* Deckbuild using your current collection
* Get in-game hep with matches and draft using Overlay tool

## INSTALLATION STEP-BY-STEP GUIDE
IMPORTANT! Program needs .NET 4.6.2 or higher to work. If app doesn't start on your PC (no interface shows up after you launch EXE) you should install .NET from here!

* Download MTGA Pro Tracker (currect version is v.1.5.6) from our github. Antivirus software (including Windows Defender) could be alarmed because of the app's ability to upload data to remote server and automatic update feature. So if Antivirus is alarmed, you should add this App to exceptions.
* Unpack it and launch MSI Installer.
* Get your token from widget on this page: https://mtgarena.pro/mtga-pro-tracker/ You must be registered user to get token!
* Copy this digit-letter code and paste it to input field of Tracker app.
* Right after you paste the code, your username (from MTGArena.pro website) will be displayed in the app window. Tokens are being stored, token authorization happens just once. Next time you launch the app, it will remember youyr token and username.
That's it! If  you've launched MTGA on his PC before, upload will start instantly. And when new cards will be added, those will be updated as well.

## Windows protected your PC?
When you get mesage "Windows protected your PC", you should click "More Info..." and "Run Anyway". Defender gets alarmed because application is not signed. But after several scans it will calm down and let you use Tracker. 

## TRACKER IS NOT UPDATING?
App crashes or not starting? No recent updates uploaded? Follow steps:
1. Make sure you have latest version v.1.5.6. It's updated to be compatible with latest MTGA version.
2. Be sure that you have .NET 4.6.2 or higher
3. If you are able to see app interface, just click FULL RESET button, then re-input new token.
4. Try to reboot your PC
5. Check if antiviruses or firewalls are blocking app traffic, add app to exception

## Changelog
v.1.5.6 released 31/01/2019 (In-game Overlay)
* Added in-game overlay with 3 modes: matches, decks and draft helper
* Added detailed settings for overlay
* Improved app interface
* Code signed. Now antiviruses will not get triggered with our software.
* To enable overlay just click respective button in the app interface.

v.1.5.3 released 03/01/2019 (New Year Update)
* Notifications from developers in the app. So you will not need to look for info about tracking issues on Twitter or Reddit. 
* Better update notifications. You will see update button right after update is out.
* More stable matches tracking. No opponent's cards from previous matches will get into next match. 
* Remote restart. Now tracker will restart itself when needed. So new features will be available without action required from user. 
* Protection from log overgrowing. Now if your MTGA log grows huge, app deals with it properly. 
* More stable uploads. Risk of tracker get stuck so you need manual full reset is minimal.
* In-game time counter. You will now how much time you spent on MTGA on daily basis. 

v.1.5.2 released 23/11/2018 (No initial upload)
* Fix of unwanted behaviour when app uploads old data from the log on every startup, even if that data already was uploaded.

v.1.5.1 released 21/11/2018 (Better UX)
* Data upload progress bar shows process of big logs uploads
* Buttons are being disabled when they are useless anyway or shouldn't be pressed
* Manual Reset now cleans up AppData folder, so no need to manually clean it

v.1.5.0 released 21/11/2018 (Catch-up Mode)
* NEW: introduced manual re-sync and old logs reading
* Improved data delivery on server leading to more stable data uploads
* Now tracker gets all battles from latest log even if it wasn't running
* Fixed time. Finally users will get time recorded according to their timezones
* Backlog: still no direct challenges decks detection. Will add this feature later. 

v.1.4.8 released 15/11/2018 (Hotfix)
* Fixed possible issues with collections and decks sync
* Some interface improvements and more stability

v.1.4.6 released 11/11/2018 (Hotfix)
* Hotfix: Protection of server from uploads-induced DDOS
* Hotfix: German users log parser
* Numerous tiny bugfixes

v.1.4.3 released 09/11/2018 (Better data delivery system):
* Data transmission format from client to server reworked in order to provide more stability and reduce server load

v.1.3.7 released 09/11/2018 (Hopefully final hotfix):
* Fixed error with "Client needs update" message
* Fixed date/time bugs
* Fixed globalization issues with different date/time formats
* Done some tiny improvements

v.1.3.5 released 07/11/2018 (Hotfix):
* Fixed client-side data storage system
* Added nice banner

v.1.3.4 released 07/11/2018 (Big Update!):
* Data extraction from latest log even if tracker was not running. Important: if the game was restarted for several times, only data from the latest session without tracker will survive.
* Better logs parsing system which opens the way directly to full match replay function (not implemented yet on MTGArena.pro, but client-side is fully ready)
* Upload success control and local data storage during server downtime. So no lost tracking matches because of server maintenance.
* Fixed multiple accounts: now this function is working properly.
* Stability improvements. Now app re-spawns itself if it's crashes, so no data lost because of app stopped working.
* Logging improvements. Now we will be able to monitor bugs more closely to fix them faster.
* Better integration with MTGA process.
* Fixed Windows 7 support.

v.1.3.2 released 03/10/2018 (Google Cloud):
* Server load moved on Google Cloud

v.1.3.1 released 01/10/2018 (Server Load Reduce and Stability Fixes):
* Maintenance update designed to reduce server load.
* Added MTGA player nicks recognition.
* Fixed several bugs and improved stability.

v.1.3.0 released 31/08/2018 (Multiaccount Fix & better bug tracker embeded):
* Now Multiaccount function works as it should: when you change accounts in a game, traker will switch tokens or request new token
* Better bugtracking system will help me to intercept tiny glitches in tracking process and make respective fixes.

v.1.2.9 released 17/08/2018 (MTGA v.818_646046 compatibility):
* Updated log format

v.1.2.7 released 08/08/2018 (Dynamic Monitoring):
* Now you don't need to update app in order to get new tracking tools. App loads monitoring patterns dynamically from server.
* Some bug fixes

v.1.2.6 released 06/08/2018 (Maintenance Release):
* Fixed bugs
* Resolved compatibility problems with Win7 & Win8

v.1.2.5 released 03/08/2018 (Optimization and fixes):
* Better MSI installer (no cab-files and directory selector added)
* Better string processing (thanks to u/Spongman)
* Improved log processing (app will not re-scan the whole log on startup if it isn't changed)
