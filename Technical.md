The script doesn't need to be in the same folder as your notes - you can put it in a Scripts folder if you have the means to run it remotely. Just ensure that the config file ends up in the same folder as the script.

You may also want to prepend the following shebang to the start of the file:

`#!/usr/bin/env python`

For more information, see [this pull request](https://github.com/Pseudonium/Obsidian_to_Anki/pull/13).

New in v2.7.0 - the script can now automatically open Anki if Anki Path and Anki Profile are supplied. This would allow you to schedule the script to run at a certain time without needing to worry about whether Anki was open at that time.

Note that the script will never close Anki by itself, so you may find Anki open when you return to your computer!

For those having issues installing on Ubuntu, check out [#99](https://github.com/Pseudonium/Obsidian_to_Anki/issues/99).

# Scheduling

On Windows, check out [Task Scheduler](https://www.windowscentral.com/how-create-automated-task-using-task-scheduler-windows-10).

On macOS/Linux, check out Corey Schafer's excellent tutorial on [cron](https://www.youtube.com/watch?v=QZJ1drMQz1A).

As an example, you could schedule the script to run recursively over your top-level notes folder, at midnight every day.

## Obsidian plugin

As of v3.2.0, the plugin offers inbuilt scheduling! However, this only works when Obsidian is running.