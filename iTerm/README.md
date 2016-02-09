iTerm2
------

Since we're going to be spending a lot of time in the command-line, let's
install a better terminal than the default one. Download and install
[iTerm2][1].

[1]: <http://www.iterm2.com/>

In **Finder**, drag and drop the **iTerm** Application file into the
**Applications** folder.

You can now launch iTerm, through the **Launchpad** for instance.

Let's just quickly change some preferences.

### Colors and Font Settings

-   Set hotkey to open and close the terminal to `command + option + i`

-   Go to profiles -\> Default -\> Check silence bell

-   Download the [Solarized dark iterm colors][2] from here. And then set these
    to your default profile colors.

    [2]: <https://github.com/altercation/solarized/tree/master/iterm2-colors-solarized>

-   Change the cursor text and cursor color to yellow make it more visible

-   Change the font to 14pt Source Code Pro Lite. Source Code Pro can be
    downloaded from [here][3].

    [3]: <https://github.com/adobe/source-code-pro/downloads>

 

 

### Showing/Hiding Hidden Files

1.  Open Terminal found in Finder \> Applications \> Utilities 

2.  In Terminal, paste the following: `sudo nano ~/.bash_profile`

3.  Enter your Mac’s administration password if required, then hit return

4.  At the bottom of the open .bash\_profile file, paste the following: `alias
    showfiles='defaults write com.apple.finder AppleShowAllFiles YES; killall
    Finder /System/Library/CoreServices/Finder.app'`

5.  Below that, paste the following: `alias hidefiles='defaults write
    com.apple.finder AppleShowAllFiles NO; killall Finder
    /System/Library/CoreServices/Finder.app'`

6.  Press ctrl + O and hit return to save the file

7.  Press ctrl + X to exit the file and return to the command line

8.  In Terminal, paste the following: `source ~/.bash_profile` to refresh your
    profile and make the aliases available

![](<http://ianlunn.co.uk/wp-content/uploads/Screen-Shot-2014-01-06-at-15.46.22.png>)

~   Adding aliases to .bash\_profile via Terminal

Adding aliases to .bash\_profile via Terminal

Now when you want to show hidden files, all you need type in Terminal
is `showfiles`, then `hidefiles` when you want to hide them.

### Source

-   <http://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/>
