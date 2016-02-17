## What is a .bash_profile?

There is a hidden file in your user directory named .bash_profile. This file is loaded before Terminal loads your shell environment, and contains all the startup configuration and preferences for your command line interface. In your bash_profile you can change different settings such as your terminal prompt, adding aliases to functions you use frequently, etc.

This file is called a ‘dot file’ and it's invisible in Finder. The ‘.’ at the beginning of the name renders it invisible. You can view all invisible files in the Terminal by typing `ls -al` in any directory. You might be surprised by how many you find.

## Setting up your Learn .bash_profile

 1. type `mv ~/.bash_profile{,.bak}` to backup any files you already have
 2. run `curl "https://raw.githubusercontent.com/flatiron-school/dotfiles/master/bash_profile" -o "$HOME/.bash_profile"`
 
 ## Reverting to your old bash profile
 
 1. ```cd ~```
 2. confirm that you have .bash_profile.bak in your root directory
 3. If it is present, ```rm .bash_profile```  (This will delete the current .bash_profile)
 4. ```mv .bash_profile.bak .bash_profile``` (This will rename the backup file so it is now the .bash_profile)
 5. ```source .bash_profile``` (This will reload the new .bash_profile in the currently open terminal)
 6. If your old bash profile isn't in effect in your terminal, you may need to close all open terminal windows and then open a new terminal window
<p data-visibility='hidden'>View <a href='https://learn.co/lessons/bash_profile'>.bash_profile</a> on Learn.co and start learning to code for free.</p>
