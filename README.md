```
@@@@@@@    @@@@@@   @@@   @@@@@@    @@@@@@   @@@  @@@
@@@@@@@@  @@@@@@@@  @@@  @@@@@@@   @@@@@@@@  @@@@ @@@
@@!  @@@  @@!  @@@  @@!  !@@       @@!  @@@  @@!@!@@@
!@!  @!@  !@!  @!@  !@!  !@!       !@!  @!@  !@!!@!@!
@!@@!@!   @!@  !@!  !!@  !!@@!!    @!@  !@!  @!@ !!@!
!!@!!!    !@!  !!!  !!!   !!@!!!   !@!  !!!  !@!  !!!
!!:       !!:  !!!  !!:       !:!  !!:  !!!  !!:  !!!
:!:       :!:  !:!  :!:      !:!   :!:  !:!  :!:  !:!
 ::       ::::: ::   ::  :::: ::   ::::: ::   ::   ::
 :         : :  :   :    :: : :     : :  :   ::    :

A Firefox theme with Pywal and macOS in mind. 
Firefox Vibrancy, Transparency, for macOS
ver. 0.1
By: Brandon Shockley
Original Source Material: "https://github.com/manilarome/blurredfox/"
```
# Screenshots

# Why? 
  Unfortunately becuase of design capability differences between Firefox for Linux and macOS, 
Manilarome's beautiful theme doesn't render properly on macOS. This edit of their theme tries 
to find work arounds for what doesn't work, as well as tweak some settings to my liking. This 
theme is intended to be used with Pywalfox (https://github.com/Frewacom/pywalfox). I am also 
not a professional CSS developer. My theme might be crude, and there are likely to be 
overlapping rules and bugs. Please feel free to propose fixes and raise issues on Github. 

# Dependencies

# Installation

# TODO:
- [ ] Integrate this better into Pywalfox
   -  [ ] Context menu highlighting
   -  [ ] Text highlighting 
   -  [ ] Context Menu Background
   -  [ ] Check if there are variables set I can use or link wals cached .css file. Restarts
            would be required if simply linking cached css. 
        - [ ] If Linking to .css from .cache/wal create a template to add alphachannels
-  [ ] Clean up rules and make them more concise. 
-  [ ] Find a better solution to show and hide the macOS Titlebar buttons [ (x) (-) (+) ]
-  [ ] Change Right Click Menu Seperators and Right Click Hover Color
-  [ ] Keep Menu Selected When Hovering over the Titlebar Buttons [ (x) (-) (+) ]
-  [ ] Keep URL Bar open when scrolling through overflow dropdowns
-  [ ] Make sure URL Bar and Tab Bar are the same height
-  [ ] Add pywal variable to --chrome-content-separator-color. 
-  [ ] Integrate Pywal Colors into Find Bar
-  [ ] Find Bar Seach Box Should be White
-  [ ] Side Bar Vibrancy
    -  [ ] Side bar header drop down
-  [ ] Dropdowns, right click, and context menus should match
-  [ ] Do the Customize Window 
-  [ ] Look at pywalfox's userChrome.css to see if there's anything I can integrate
-  [ ] Implement Other layout conifurations eg: Auto Hide Side Bar w/ Tabbar and OG
        auto hide url bar with tab bar on the bottom. 
-  [ ] Theme the Dropdown under the back and probably forward buttons
-  [ ] Add wallpaper or pywall'd picture / logos to interface
-  [ ] Look into icon replacements
-  [ ] Can I import sass files eg: userChrome.scss 

# Bugs:
* Find Bar Near the search box appears to flash in sync with the cursor after typing try to 
replcate.
    - Mostly Fixed by setting .findbar-closebutton to vibrancy. Still occurs once everytime 
    you click the search box. Bug is also caused by other behavior

* Opening Findbar while side panel is open messes up the lower half of the background of the
sidepanel.  
    - Set the findbar opacity to .9 appears to resolve this for the most part, findbar flashes
    when exiting

* colors.css is not completely matching pywalfox pallet. They might be off, but pywalfox has 
more colors. 19 vs 15. Some colors in colors.css appear to be dupes. Check colors.css.

* If you move your cursor above the header text in the side panel the tabs bar drops down. It
would be nice if that didnt happen. 
