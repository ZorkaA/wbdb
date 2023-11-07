# wbdb – War Brokers Database 
***(or as well as one can do given what's public)***

Script that pulls IDs from all squad members, and uses [POMP's API](https://wbp-wbapi.web.app/api-docs/#/player) to gather additional data on those players. Optimized for [Google Colab](colab.research.google.com) and interfaces with [Google Drive](drive.google.com). 

## Setup:

Dirt simple. Just make sure you know how to read.
- `memberpath`: Path to where you want the initial STATS SITE pull to be stored. Literally just has IDs, squad names, and player names. Doubles as a way to count squad members per squad, though [this](https://github.com/Encryp7R/WB-Squad-List-Numbers) script does the same and requires less work on your end.
- `wbdbpath`: Path to where you want the final csv to be stored. ~1000 rows (as of Nov 2023, will change over time).
- `drive.mount(blah blah blah)` Sets up write directory. **Comment out if you're NOT using Colab**, otherwise don't touch it. 


## Word of caution:
- Colab will ask for permmission to access your drive, that's normal since you'll be writing files to your drive.
- There is no built-in ratelimiting, so be careful if you're running extended versions multiple times in short succession. It's not impossible to crash stuff if you act irresponsibly. This will get Dipper and/or POMP pissed, and that's not good.

**If you abuse this I will find you in your sleep**
 
