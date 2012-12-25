# L4D2 Survivor MVP Plugin
***Based on Plugin by Tabun at [L4DNation](http://www.l4dnation.com/confogl-and-other-configs/survivor-mvp-plugin/).***

## Overview
The original plugin incorrectly collected and displayed tank and witch damage unless it was previously specified to include it in the MVP calculation. What'
s more, it was incorrectly showing tank damage even when it was being collected (due to an odd event in which seemed to award 5k damage to whoever struck the final blow to the tank). This forked version of the plugin simply corrects those issues, while also implementing a range of other stats and features (mainly grabbed from the requests in the author's original thread).

A lot of the code needs to be cleaned up and refactored. I suppose after all of the new features are implemented that's what should be done, however if someone else wants to have a crack please feel free! I personally have plans to build on this plugin (though most likely I'll create a new plugin which takes advantage of the author's original natives, whilst also adding in a few of my own), that records statistics across the server, so you can see a user's history. I've been meaning to write something like that for my own server for a while, so we can implement some form of ranking algorithm and see what players aren't pulling their weight. 

##Changes:

  - Track witch and tank damage regardless of whether or not we're including it in our mvp stat.
  - Fix issue with last survivor to inflict damage on tank prior its death being awarded 5k damage. 
  - Collect and display to console more detailed statistics:
    - Number of times pinned/smoked etc.
    - Number of pills eaten
    - Total damage received
    - Kills of each zombie class
    - Boomer pops (without anyone getting boomed)
 

##TODO:
  - Tank stats (collect and output stats when tank is up so we can see who isn't pulling their weight):
    - Common/SI killed during tank
    - Number of rocks eaten
    - Number of rocks skeeted
    - Number of times pinned/smoked etc.
    - Total damage dealt to tank (if someone doesn't deal a lot of damage, doesn't clear SI/common and DOESNT get pinned, they're doing something wrong)
    - Time spent LOSing tank.
  - Misc stats
    - Track skeets (I might hold off on this for a bit as it's going to be a bit annoying)
  - Add command to print stats to console (so we can view stats mid-game, not just at the end of round)