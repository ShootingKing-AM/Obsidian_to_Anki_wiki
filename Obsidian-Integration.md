# All users
## Add file link

This will automatically append a link to the file that generated the flashcard, on the first field.

# Obsidian Plugin Users

## Add file link

Using the plugin settings, you can choose which field to append the link to!

## Link support

The plugin fully supports both normal markdown links and Obsidian style wikilinks.

## Embed support

The plugin supports obsidian-style image and audio embeds.

## Context

Using the plugin settings, you can choose which field to append 'context' to! This is the path of the file the note was generated from, as well as the position of the note in the heading tree (if any) of the file.

For example, if the file was called "test.md", and we had a note in this position:

<pre>

# Overall point

## Subheading 1

## Subheading 2

START
Basic
This is a test
Back: Test successful!
END

</pre>

Then, the context for the note would be the string "test.md > Overall point > Subheading 2"