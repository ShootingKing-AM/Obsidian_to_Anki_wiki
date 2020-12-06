# Cloze note types
Allows you to indicate whether or not a note type should be interpreted as a 'Cloze' type. You must set this to 'True' if you wish to use the 'CurlyCloze' option with this note type - see [Cloze formatting](#cloze-formatting).

# DEFAULT section

Section for setting default parameters of the script:
* Tag - the default tag added to every card produced by this script.
* Deck - the default deck every card produced by this script goes into. Overridden by TARGET DECK (see [syntax](#syntax))
* CurlyCloze - explained in [Cloze formatting](README.md#cloze-formatting)
* GUI - allows you to enable/disable the GUI of the script. See [Command line usage](README.md#command-line-usage)
* Regex - Toggle regex mode to be on or off by default.
* ID Comments - Toggle whether or not card IDs are wrapped in a HTML comment. Wrapping IDs in a HTML comment makes them invisible on 'preview' mode, which can make notes look cleaner.
* Anki Path and Anki Profile - If you supply both the absolute path to the Anki executable, and your profile on Anki, the script will attempt to open Anki when run if it's not already running. Useful for automation - see [Technical](README.md#technical)

# Obsidian

Vault name: The name of your obsidian vault that you're adding flashcards from.  
Add file link: Whether you want to append a link to the associated obsidian file on the first field of the card.  

# Syntax

Note that START, END, TARGET DECK, FILE TAGS and DELETE all require an **exact match** on the line - you cannot have spaces afterwards.
* Begin Note - The string that signals the start of a [note](#note-formatting). Defaults to START.
* End Note - The string that signals the end of a note. Defaults to END.
* Begin Inline Note - The string that signals the start of an [inline note](#inline-note-formatting). Defaults to STARTI (Start-Inline).
* End Inline Note - The string that signals the end of an inline note. Defaults to ENDI (End-Inline).
* Target Deck Line - The string that signals "the line beneath me is the name of the target deck". Defaults to TARGET DECK.
* File Tags Line - The string that signals "the line beneath me is the set of tags that should be added to all notes from this file". Defaults to FILE TAGS.
* Delete Regex Note Line - The string that signals "the line beneath me is an id string for a regex note that should be deleted." Defaults to DELETE.