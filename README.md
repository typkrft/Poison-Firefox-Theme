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
ver. 0.2
By: Brandon Shockley
Original Source Material: "https://github.com/manilarome/blurredfox/"
```
![Poison](https://i.imgur.com/0Amq1Y9.png)
![Additional Screenshots](https://imgur.com/a/Sh0vzDS)

# Why? 
Unfortunately, becuase of design capability differences between Firefox for Linux and macOS, 
Manilarome's beautiful theme, ![blurredfox](https://github.com/manilarome/blurredfox) doesn't render properly on macOS. This edit of their theme tries 
to find work arounds for what doesn't work, as well as tweak some settings to my liking. This 
theme is intended to be used with, ![pywal](https://github.com/dylanaraps/pywal) and ![pywalfox](https://github.com/Frewacom/pywalfox). I am also 
not a professional CSS developer. My theme might be crude, and there are likely to be 
overlapping rules and bugs. Please feel free to propose fixes and raise issues on Github. 

# Features
- Autohide Single Tab Windows
- Autohide URL Bar
- Native macOS Vibrancy (Blur & Transparency) Effects for
 - The Side Panel
 - The URL Bar
 - The Tab Bar
 - The Bookmarks Bar
 - The Find Bar
 - The Customization Page
- Clearly Commented So you can turn Features On and Off
- Pywal & Pywalfox theming for 
 - Dropdown Menus 
 - Right click Menus
 - Tabs
 - Etc.

# Dependencies (Optional - See Notes)
- ![Pywal](https://github.com/dylanaraps/pywal)
- ![Pywalfox](https://github.com/Frewacom/pywalfox)

# Installation
- Install ![Pywal](https://github.com/dylanaraps/pywal/wiki/Installation)
  - Note: I would recommend Installing it from source if you plan on using it on its own. The last time I checked there was an issue that cuased the wallpaper to disappear when trying to set it in macOS. 
- Install ![PywalFox](https://github.com/Frewacom/pywalfox)
  - Note: There are two parts to PywalFox - 1) Firefox Extension 2) A local python daemon. Both are required for Pywalfox to function properly. In addition you may run into an issue connecting the daemon to the Firefox extension please check ![this thread for possible solutions](https://github.com/Frewacom/pywalfox/issues/34).
- Run pywal to generate a cached theme.
- Enable custom css in Firefox. More on this ![https://www.reddit.com/r/FirefoxCSS/comments/brmi8v/psa_firefox_v69_users_will_have_to_set_a_pref_to/](here_.
  - Note: There may be some additional preferences you need to change. I don't recall if it's neccessary on macOS. If you run into issues please let me know. 
- Download the userChrome.css file from this repository. 
- Edit the `@import url` line to reflect your pywal cache file. This should be found `/Users/<userName>/.cache/wal/colors.css`.
- Look through the config and edit the options to your liking. 
- Once Installed simply add the userChrome.css file in the chrome folder in your Firefox profile folder. 
  - Note: Your profile folder should be located at `/Users/<userName>/Library/Application\ Support/Firefox/Profiles/xxxxxxx.default-release/chrome/`.
- Restart Firefox.
  
# Notes: 
  - The Dependencies are optional, but if you dont use them be sure to edit the color variables and remove the pywal import line.
  - The way it is setup now the userChrome.css sources a cached pywal this means when ever you update pywal you must also restart Firefox. Pywalfox colors will update without restarting however. 
  - This could be modified for Linux. I might effectively the only thing that probably would change are the `-moz-mac-vibrancy-dark` sections. Blur would likely be set through your compisitor and not userChrome.css
  - The User should configure spacing in the URL bar between elements using the Customization page instead of tyring to set it in the userChrome.css, probably.

# TODO:
- [ ] Integrate this better into Pywalfox
   -  [ ] Context menu highlighting
   -  [ ] Text highlighting 
   -  [ ] Context Menu Background
   -  [ ] Check if there are variables set I can use or link wals cached .css file. Restarts
            would be required if simply linking cached css. 
        - [ ] If linking to .css from .cache/wal create a template to add alpha channels
-  [ ] Clean up rules and make them more concise. 
-  [ ] Find a better solution to show and hide the macOS Titlebar buttons [ (x) (-) (+) ]
-  [ ] Change Right Click Menu Seperators and Right Click Hover Color
-  [ ] Keep Menu Selected When Hovering over the Titlebar Buttons [ (x) (-) (+) ]
-  [ ] Keep URL Bar open when scrolling through overflow dropdowns
-  [ ] Make sure URL Bar and Tab Bar are the same height
-  [ ] Add pywal variable to --chrome-content-separator-color.
    -  [X] <del>Create Config Options to Show and hide.</del>
-  [ ] Integrate Pywal Colors into Find Bar</del>
-  [X] <del>Find Bar Seach Box Should be White
-  [X] <del>Side Bar Vibrancy</del>
    - [X] <del>Side bar header drop down</del>
-  [ ] Dropdowns, right click, and context menus should match
-  [X] <del>Do the Customize Window</del>
-  [ ] Look at pywalfox's userChrome.css to see if there's anything I can integrate
-  [ ] Implement Other layout conifurations eg: Auto Hide Side Bar w/ Tabbar and OG
        auto hide url bar with tab bar on the bottom. 
-  [ ] Theme the Dropdown under the back and probably forward buttons
-  [ ] Add wallpaper or pywall'd picture / logos to interface
-  [ ] Look into icon replacements
-  [ ] Can I import sass files eg: userChrome.scss 
-  [ ] Try to add blur to elements that are just transparent. Maybe a blurred picture as the background? 
-  [ ] Change the height of the URL Bar to match the icons in the bar
-  [X] <del>Center the URL Bar buttons between the Url input and the edge</del>
-  [ ] URL Bar always focused on New Tab 
-  [X] <del>Hide Tabs if only one tab</del>

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
