# chpath

Helps a user manage their current PATH structure. For those who don't know, the PATH contains a list of directories to search in for any given program. Sometimes modifying the path can include restarting your terminal, and sometimes even your computer! With chpath, it force-refreshes the PATH readers for the entire terminal so you can get to using your new path right away!

You can list all current paths with `chpath list`

Adding paths is as simple as passing any number of paths to `chpath add [PATHS ...]`

Editing paths is as simple as taking the original path (can be grabbed via `chpath list | grep` or other various operations) and setting it equal to the new path via `chpath edit <path>=<newpath> [ ... ]`

Removing paths is as simple as passing all the paths to remove to `chpath remove [PATHs ...]`

The point of this script is to be simple, robust, and most of all helpful. You shouldn't ever have to use the command once your paths are setup, and other programs can run detection for chpath and utilize it directly to realtime update the path (Won't work unless base program is sourced alongside chpath)
