# v6.0.0

* Fixed 'l1' alias so that it lists dotfiles (minus . and ..).
* Switched to using sub-shells when traversing sub-directories for all functions.
* Switched from the pry-debugger to pry-byebug gem in irbrc.
* Switched from RDoc to Markdown for documentation.
* Updated the "gall" alias to use the --all option.
* Updated the "gcap" function to use long form Git options for better readability.
* Updated the "rew" function so that flags and local/remote options are easier to understand.
* Updated README to match GitHub project description.
* Updated "rew" local options to point to "Projects" path instead of the "Ruby" path.
* Updated the sc, ss, sg, and sdb functions to support Rails 2.x.x, 3.x.x, and 4.x.x.
* Added the "bertt" function which allows for easier testing of a specific Test::Unit test file.
* Added the "berts" alias for getting a summary of failing (if any) test files (including line numbers).
* Added the "bertv" alias for enabling Test::Unit to run tests in verbose mode.
* Added the "gus" alias (i.e. git reset HEAD).
* Added the "ggc" alias for validating and fixing dangling objects, freeing up disk space, improving performance, etc.
* Added the "gvca" function which validates and cleans all Git projects for current diretory.
* Added the "gail" alias for easily displaying/changing current global email address used for commits.
* Added the "gemuc" alias for gem update and clean of entire system.
* Added the 'w' Pry alias for "whereami".
* Added the "md" alias for opening Markdown files within the Marked app.
* Added a Versioning section to the README.
* Added tsl (list-sessions), tsa (attach-session), tsk (kill-session), and tsr (rename-session) aliases for tmux.
* Added vi as the default visual editor.
* Added the "rua" function for upgrading all projects in current directory to a new ruby version.
* Added Travis CI bash completion support.
* Added missing CHANGELOG, LICENSE, and README files.
* Added NPM to PATH.

# v5.2.0

* Force default Git editor to wait for files to be closed before returning.
* Updated shell script documentation.
* Fixed z.sh warnings when sourcing bashrc.
* Updated bash functions to use read line instead of tweaking the IFS variable for parsing directories with spaces.
* Modified gsta function to display branch status and unpushed changes in addition to uncommitted changes.
* Collapsed while/do statements to a single line.
* Added save to 'gash' alias so that git stashes can optionally be saved with a description.
* Added pretty print formatting to 'gashl' alias for git stash lists.
* Moved git grep (gg) next to git search git log search (gls).
* Dropped the glc alias in favor of the guthors alias (uses the author summary originally provided by the glc alias).

# v5.1.0

* Fixed bug with sublime not being defined prior to loading bash_* files as a necessary dependency.
* Fixed bug with opf alias where paths with spaces would fail to open properly.
* Fixed Git-related Bash functions where directory names would be split with spaces.
* Added the -f option for exporting functions.
* Added ez alias which speeds up opening the ~/.z config in the default editor.
* Added the xrayconfig.txt file which supports the xray-rails gem.
* Added the 'f' alias for the pry-debugger finish command.
* Added pry-rescue support.
* Added Bond gem support to .irbrc and .pryrc.
* Added breakpoint aliases for Pry to .pryrc.
* Added the gdis alias (i.e. git reset --hard).
* Added the gcp alias (i.e. git cherry-pick).
* Added the gpua function which allows one to "git pull" for all git-enable directories in current folder.
* Added boa Bash function which lists outdated gems for each project in current directory.
* Added the gifize function (allows one to easily convert video into an animated GIF.
* Added the gi alias (i.e. git init).
* Refactored the scripts in the functions folder.
* Updated run.sh usage.
* Switched from pry-nav to the pry-debugger gem.
* Updated the gpd Bash function to delete local branch regardless of merge status and made remote branch specific to 'origin'.
* Added gasha function which answers the git stash size of all projects in current directory.
* Renamed instance variable 'directory' to 'project' in directory loops for Bash functions.

# v5.0.0

* Fixed the timeout comment in the pow config.
* Fixed 'Enhancements' spelling typo in irbrc file.
* Default the $EDITOR variable to Sublime Text for all environments.
* Default to 'simple' when pushing (gitconfig).
* Added the gce alias for 'git config -e'
* Added the opf alias (i.e. opens current terminal path as a tab in Path Finder).
* Added Pry aliases for continue, step, and next as c, s, and n.
* Added guardrc support and dropped the -c option from the beg alias (provided via guardrc now).
* Tweaked .pryrc to match Bash prompt settings.
* Added the .aprc file for setting Awesome Print defaults.
* Add the Dotphiles resource to the README.
* Configured Bash history to remove duplicates, keep a history size of 1000, and exclude mundane commands from being entered in history.
* Added Hirb and Awesome Print support to the Pry console.
* Updated the installer to prompt for options before executing.
* Added the install option for checking currently installed file differences.
* Added the install option for linking dotfiles to this project.
* Added the install option for showing available dotfiles for install.
* Added the install option for deleting installed dotfiles.
* Added the geady alias (i.e. git rebase -i @{u}).
* Renamed the 'guthers' alias to 'guthors'.
* Renamed install.sh to run.sh.
* Bumped IRB Eval History to 1000.
* Reduced Bash history size to 1000.

# v4.1.0

* Applied RubyGems 2.0.0 syntax upgrades.
* Added the powconfig file. Thanks Eric.
* Removed the Code Climate badge - Not really relevant for this project.
* Removed the tree alias, using the Tree app instead.
* Added Z support for Bash.
* Added the gba alias (git branch --all).
* Renamed the gpcap alias to gcap and cleaned up the associated documentation.
* Upgraded the gtaila alias to color code counts: 0-9 (white), 10-19 (yellow), 20 or greater (red).
* Fixed if statement in gtaila function color check.
* Cleaned up the gtaila function documentation.
* Added a link to the Dotify project in the README.
* Added purple color to current directory info in shell prompt.
* Added additional Bash color definitions.
* Changed the command prompt colors to the following: timestamp (grey), Git branch (purple), and current directory (cyan).
* Added Nicolas Gallagher's dotfiles to the README.
* Broke up the command prompt code into easier to read segments.
* Switched IRB prompt to match Bash shell prompt (using pipes instead of brackets).
* Added the gls alias (i.e. gl + -S for search).
* Removed Windows support of Thumbs.db in gitignore.txt.
* Removed TextMate support in gitignore.txt.
* Removed SVN support in gitignore.txt.
* Ignore CTag metadata in gitignore.txt.
* Added parameter documentation for init_github function.
* Added the gday function to report git activity across all projects for today only.
* Refactored the duplicate gsup and gday function code into the gince function.

# v4.0.0

* Removed the extra spacing before time in the 'gld' alias.
* Split Bash aliases and functions into separate files.
* Fixed bash prompt so that word wrapping works.
* Fixed diagram aliases to ensure the doc/design folder exists prior to being executed.
* Dropped the debug alias.
* Added cyan coloring for project names in gsta and gsup aliases.
* Added the gcm alias (i.e. git commit -m).
* Added the rbi alias (i.e. rbenv install).
* Cleaned up file permissions.
* Added sgh alias (i.e. script/rails helper).
* Added the gbd alias for deleting local and remote branches.
* Added gbdm alias for deleting all merged branches.
* Added the gtaila function which counts the number of commits from last tag for all projects.
* Moved bash colors into seperate file.
* Removed excess carriage return per project results.
* Added the gpcap alias which commits and pushes changes for all projects that have changes.
* Removed the debundle code.
* Added color comments.
* Added the guthers alias (lists all authers/contributors on a project).
* Added the gap alias (i.e. git add --patch).
* Expanded git alias abbreviations to improve self documentation.
* Expanded all alias abbreviations, where able, in order to be more self documenting.
* Added Adam Jahnke's dotfile project to the README.
* Added the rdd bash alias (i.e. rm -rf _doc).
* Applied Code Climate GPA badge.

# v3.0.0

* Added ipa alias.
* Added the groot alias. Thanks Eoin.
* Added the gwc Git alias.
* Added l1 alias for listing files and directories as single line output only.
* Added a Bash function for reporting Git activity across all projects for standup reports.
* Added Git URL aliases for GitHub and Heroku to gitconfig.txt
* Added the gms alias.
* Added alias for gdc.
* Added the sniff alias for monitoring TCP/IP traffic (pulled from Paul Irish's dotfiles).
* Added the bert aliase for running Test::Unit tests.
* Added the beg alias for running guard.
* Added usage printout for rew function.
* Added third option to rew function which allows for building a new rails project using local rails setup template options.
* Added the glatest git alias which answers the latest update to the project with a datestamp.
* Added the rbu alias (i.e. rbenv uninstall).
* Added support for current git branch to command prompt display.
* Added Bash Completion support.
* Added yellow color to Git branch info in command prompt.
* Added glame alias (i.e. git blame).
* Added the gsta function (i.e. git status all) which answers the status of any project with uncommitted changes.
* Added Code Climate support.
* Added the rbvars alias.
* Added the rfixes alias.
* Added the gtail alias which shows all commits since last tag.
* Added CONTRIBUTING guidelines per GitHub requirements.
* Added Ruby 1.9.x syntax.
* Added the gashl, gashs, gashp, gashd, and gashc for git stash list, show, pop, drop, and clear respectively.
* Modified the command prompt to keep the cursor at the first position.
* Modified the copy to clipboard message for the glh alias.
* Modified the gsup alias to output commits in reverse order (oldest first, newest last).
* Modified the 'ber' alias to be 'bundle exec rake'.
* Modified the rew function to make it easier to select which templates to build from when generating a new Rails app.
* Modified the rew alias so that the template choice can be supplied without always being prompted for one.
* Modified alias rbw to be rbp (i.e. rbenv which) and changed rbw to alias rbenv whence.
* Modified the PRY prompt to resemble the IRB prompt.
* Modified bash prompt colors (grey for time and cyan for git branch info).
* Modified all git logging to show full commit hash.
* Removed the cpath alias and upgraded the p alias to always copy path to clipboard.
* Removed the hard coded author name for the gsup alias - picks up git user name from .gitconfig file instead.
* Removed the Bash color codes.
* Removed Pry editor config since it defaults to sublime.
* Removed the bec alias for cucumber and repurposed it to capistrano (i.e. bundle exec cap).
* Removed the Apache aliases.
* Removed the Ruby GC exports (configured by rbenv-vars - see the OSX project for further details).
* Removed the bers alias and replaced with the bes and bess aliases for using RSpec.
* Removed the Ruby install script and added a Bash script instead.

# v2.2.0

* Fixed awesome_print requirement for .irbrc.
* Removed the .railsrc file and added the "rew" fuction to the .bashrc file with support for multi-template setup.
* Removed the Wirble gem and switched to Wirb.
* Added Pry support (see pryrc.txt).
* Added Ruby heap/memory settings.
* Added rdo alias for quickly launching generated RDoc.
* Added gpur alias for 'git pull --rebase'.
* Added glh alias for acquiring full hash of last commit and auto-copy to clipboard support.
* Added gamend alias for git comment ammending.
* Added glf alias for showing recent git changes in HEAD prior to doing a git pull.
* Added aliases for rbenv.
* Added debundler support the .irbrc file.
* Added IRB auto-completion and history support.
* Added the GitHub Dotfiles project to the README.

# v2.1.0

* Fixed checkout instructions.
* Fixed issues with IRB and Rails IRB command prompts.
* Added sdb alias for rails dbconsole.
* Added RubyMine project files to gitignore file.
* Added Espresso files to gitignore file.
* Added a resource link for bash shell colors.
* Added the rassp and rassc aliases.
* Added Capistrano aliases for stage and production deploys.
* Moved the Rails IRB logic into the irbrc file and left the railsrc file with only default settings.
* Added aliases for Sitemap Generator gem.
* Added alias for bundle outdated.
* Droped RailRoad gem support and switched to the Railroady gem.
* Updated the dmodels, dcontrollers, and dstate aliases.
* Added bcon alias for bundle console.
* Renamed all the gem alises to gem*.
* Dropped TextMate support, switched to Sublime Text 2.
* Changed EDITOR export to point to sublime.
* Changed 's' alias to 'e' to represent the default editor and dropped the dot in the alias.
* Updated the bashs alias with better cross-platform support.
* Replaced use of the tilde with $HOME variable.
* Added OSX and Ubuntu path setup for rbenv.
* Updated README with link to Mathias Bynens' dotfiles project.
* Removed the aliases for clearing rails logs since the rake:log clear tasks does this now.

# v2.0.0

* Fixed the bch and rebundle aliases.
* Added .sass-cache to .gitignore.
* Added rbenv support.
* Added an alias for Heroku+ account switching.
* Added new rails app generation defaults to the .railsrc file.
* Updated the .gitconfig documentation.
* Removed rake call for the 'res' alias.
* Removed the -w option from the Ruby opts export.
* Removed the Icon? option from gitignore.
* Removed the .rmvrc template and RVM support completely.
* Removed the binary warning flag.
* Removed the rdemo and rdemot .bashrc aliases.

# v1.2.0

* Added the glast, gres, and grev Git aliases.
* Removed the ActionView and route configurations from the railsrc.txt file.
* Upgraded to Rails 3.0.11 for Rails Template Setup alias.
* Added Apache start and stop, Gemsmith, and Ruby profile aliases.
* Added git stash alias.
* Added the additional aliases for bundler: b, bch, bi, bu, and be.
* Added references to James Edward Grey II and Gabe Berke-Williams' dotfiles projects.
* Added project-specific default settings for RVM.
* Updated the IRB copy to clipboard method and added a paste method.
* Added bolded and underlined colors as well as background colors.
* Added link for Bash colors.
* Added the gln alias for git log --name-status.
* Added the init_github method to the bashrc file.
* Renamed setup.rb to install.rb and added configuration documentation to the README.
* Added the gemrc.txt template.
* Added RVM fix for loading new Ruby environments when creating new terminal tabs.
* Updated README with new Gemsmith specs.

# v1.1.0

* Removed FileUtils requirement for setup.rb.
* Added existing file check with corresponding console notification.

# v1.0.0

* Initial version.