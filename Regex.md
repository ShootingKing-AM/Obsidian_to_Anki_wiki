# Table of contents
This page lists templates for custom syntax. In each case, copy-paste the regex line into the desired note type in the config file to use the template.

* [[RemNote single-line style]]
* [[Header paragraph style]]
* [[Question answer style]]
* [[Neuracache flashcard style]]
* [[Ruled style]]
* [[Markdown table style]]
* [[Cloze Paragraph style]]


## Custom styles
The above styles are but a few examples of the endless possible styles you can make using regular expressions.
If you want to make your own style, however, you should know these things:
* The script automatically compiles the regular expression with a 'multiline' flag, so you can use the `^` character to signal the beginning of a line
* You need to have as many capture groups in your regexp as there are fields in the note type - the 1st capture group becomes the 1st field, the 2nd becomes the 2nd field etc
* If making a 'paragraph' regex, consider using this group to match lines at the end - `(?:^.{1,3}$|^.{4}(?<!<!--).*))`. It ensures that you don't accidentally match the `<!--` at the start of an ID comment!

If you'd like for your style to be added to this page, make a style-request issue and I'll consider it. 

## Tagging notes
Cards made using this format support tags - simply append a "Tags: {tag_list}" to the end of your block. The guidance is to use same line for single-line regexps, and the following line for paragraph regexps. If you're having problems, do consider whether FILE TAGS or tags from the folder (see [[Folder settings]]) would be easier!

### Obsidian plugin users

## Deleting notes
To delete notes made using this format, remove the content before the ID and make it look like:
<pre>
{Delete Regex Note Line}  
&lt;!--ID: 129840142123--&gt;  
</pre>
With the default settings:
<pre>
DELETE  
&lt;!--ID: 129414201900--&gt;  
</pre>

Note that if you manually delete a note in Anki, you should remove the ID line from Obsidian/the file too. The script will print a message if a note is identified with an ID that doesn't exist in Anki.

## Conflicts?
Try to make sure your regex matches don't overlap with each other. The script is designed, however, to not recognise a match inside another match (for different note types).

For example, if you're using the default syntax of the script for the 'Cloze' note type:
<pre>
START
Cloze
This is a {{c1::test}}
END
</pre>

, you don't have to worry about a RemNote single-line match being picked up.