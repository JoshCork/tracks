# Getting Colored Output

To get colored diff output, run git config --global color.ui auto

# Setting up your workspace on a Mac

### Downloading necessary files

Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash) in your home directory with the name git-completion.bash.
Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh) in your home directory with the name git-prompt.sh.
Save bash_profile_course from the Downloadables section in your home directory with the name .bash_profile. If you use Linux, you may need to name this file .bashrc instead of .bash_profile. (If you're curious to learn more about how bash prompts work, see [this page](http://www.cyberciti.biz/tips/howto-linux-unix-bash-shell-setup-prompt.html).)

### Make sure you can start your editor from the terminal

If you use Sublime, you can do this by add the following line to your .bash_profile:

	alias subl="/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl"

### Making Git configurations

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Sublime, or if Sublime is installed in another location for you. See [this page](https://help.github.com/articles/associating-text-editors-with-git/) for the correct command for a couple of other popular text editors. For any other editor, you'll need to enter the command you use to launch that editor from the terminal.

	git config --global core.editor "subl -n -w"
	git config --global push.default upstream
	git config --global merge.conflictstyle diff3

### Restart the terminal

You'll need to close and re-open the terminal before all your changes take effect.

# Setting up your workspace on a Windows Machine

### Changing background color

If you prefer the background color of Git Bash to be something other than black, you can change it in the "Defaults" menu under the "Colors" tab. If you like the background color as-is, you don't need to make any changes.

### Downloading necessary files

Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash) in your home directory with the name git-completion.bash.
Save [this file](https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh) in your home directory with the name git-prompt.sh.
Save bash_profile_course from the Downloadables section in your home directory with the name .bash_profile. (If you're curious to learn more about how bash prompts work, see [this page](https://help.github.com/articles/associating-text-editors-with-git/).)

### Making Git configurations

Run the following Git configuration commands. The first one will need to be modified if you are using a text editor other than Sublime, or if Sublime is installed in another location for you. See [this page] for the correct command for a couple of other popular text editors. For any other editor, you'll need to enter the command you use to launch that editor from Git Bash.

	git config --global core.editor "'C:/Program Files/Sublime Text2/sublime_text.exe' -n -w"
	git config --global push.default upstream
	git config --global merge.conflictstyle diff3

### Make sure you can start your editor from Git Bash

If you use Sublime, you can do this by adding the following line to your .bash_profile:

	alias subl="C:/Program\ Files/Sublime\ Text\ 2/sublime_text.exe"
	
### Restart Git Bash

You'll need to close and re-open Git Bash before all your changes take effect.

# Set up Password Caching

Every time you send changes to GitHub via the command line, you'll need to type your password to prove that you have permission to modify the repository. This can get annoying quickly, so many people like to set up password caching, which will let you type your password once and have it auto-filled on that computer in the future. To do this, follow the instructions [here](https://help.github.com/articles/caching-your-github-password-in-git). If you're using Windows and you followed our Git installation instructions earlier, you're using msysgit, so you can follow the instructions for msysgit.

# Usefull commands / tools

- To visualize the log: git log --graph --oneline master (or presumably whatever one or two branches you want to look at)
	-  or maybe use an online diagramming tool like [gliffy](https://www.gliffy.com/) or [yUML](http://yuml.me/diagram/activity/draw). 
