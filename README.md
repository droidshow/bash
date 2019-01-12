### bash
#### A git repo with collection of helper bash scripts:
- [gtd](https://github.com/droidshow/bash#gtd "Description, setup, usage") : Handle multiple git projects with common commands
- [aliases](https://github.com/droidshow/bash#aliases "Description, setup, usage") : Aliases and functions for bash environment
----------------------------------------------------------------------------------------------------------------------------
## gtd
A script to help run common git commands on multiple git repos and some custom functions. All the repos are expected to be under a common directory (they can be in subdirectories). This common top level directory is mapped/linked to a drive e.g. Z: or /z. The common directory can be locally on a computing platform on harddisk or on a USB stick for portability or both. When the repos are both local and portable, script has useful commands like 'gtd usb' or 'gtd local' to quickly map one of them to Z: for further operations. What each command actually does is defined in the platform specifict config file .gtd in the home directory.

### Config file
To keep the script portable across Ubuntu, Windows7/10, Raspbian a config file (.gtd) is expected in $HOME. To start a template file (gtd_config_template) is available in the repository with examples. Copy the template to $HOME and rename it as .gtd. Populate the .gtd file with appropriate values depending on platform.

### History
I maintain emacs org mode file as few different git projects. I use this commmon script to maintain and sync directories across Ubuntu, Raspbian, Windows (git-bash). The git projects are either cloned locally on a computing platform or on USB stick for mobility. All the gtd folders are mapped to commmon drive e.g T:/ or /t. The platform specific commands are stored in a .gtd folder in $HOME.


### Usage:
 - gtd status - Display the git status of gtd projects being tracked
 - gtd commit - Commits all the changes to all the gtd projects being tracked
 - gtd pull - Pull changes to gtd projects from origin
 - gtd push - Push changes to gtd projects from origin
 - gtd map - Show drive mapping
 - gtd unmap - Unlink the mapped drive
 - gtd usb - Map the gtd drive to usb
 - gtd local - Map the gtd drive to locally cloned project
 - gtd help - Display help


----------------------------------------------------------------------------------------------------------------------------
## aliases
A collection of aliases and functions to customize bash environment. Exports editor. Installs emacs if not found.

