# Initial motivation

My workflow is essentially to have notes *be* flashcards - [one of my notes](https://www.evernote.com/shard/s522/sh/672b696d-4944-4894-a641-c84529d9ce9b/230b93561681475726fa1e2188becf78) (before I discovered Obsidian). However, it got tedious to keep copy-pasting cards into Anki, so I got the idea to write a script to do it automatically.

# Version -1

Yes, the script did actually have a 'version -1'! This was me trying to make a working prototype in a private repository.

# Version 0

This was the initial release of the script - the very first version only supported the START END syntax, with custom note types, as well as a 'substitutions' feature. I've since removed this feature - it caused too many problems! Including making the config file huge.

Features slowly got added here, in this order:
- Can now edit notes and have them auto-update
- Deck and tag organisation added
- Reading markdown formatting and embedded images

# Version 1

This release was marked by improved performance of the script, as well as the option to run the script on a directory of files at a time, non-recursively.

Features in this order were added:
- FILE TAGS for a file specified
- Syntax configurable via config file
- Inline notes

# Version 2

This release was marked by the addition of Custom Regexps to the script, which I consider to be one of the main features. It's basically fully custom syntax!

Features in this order were added:
- Audio supported
- Script now has a GUI with Gooey
- CurlyCloze
- Web-hosted image support
- GUI updated, option to disable gui
- Setup file added
- IDs wrapped in HTML comments
- Recursively scanning a folder
- Script will attempt to open Anki if Anki Path and Anki Profile are supplied
- More available syntax for CurlyCloze
- Link to Obsidian file that generated the flashcard.

Gooey was notorious for causing many headaches for people trying to install the script! An issue I still haven't fixed...

## Winter Cleaning Update

I started and finished developing the script in the month before my university term started. Once I was at university, I paused all development of the script until I came back, during which time the plugin API was released! The list of bugs had increased substantially though, and this update was aimed at addressing those bugs.

# Version 3

This release is marked by the script becoming an actual Obsidian plugin! It took many days of programming to port everything over to TypeScript, which I had to learn simultaneously! TypeScript did allow me the opportunity to clean up my code base a bit - since everything compiles to one file anyway, it's easier to split functionality across multiple files.