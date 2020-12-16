# Usage
**[[Regex]] line:** `((?:[^\n][\n]?)+\n)-{3,}((?:\n(?:^.{1,3}$|^.{4}(?<!<!--).*))*)`

1. Create a file called `test.md`
2. Paste the following contents into the file:

<pre>
How do you use ruled style?
---
You need at least three '-' between the front and back of the card.


Are paragraphs
supported?
---------
Yes, but you need the front and back
directly before and after the ruler.
</pre>
## Obsidian Plugin users
3. In the plugin settings, paste the Regex line into the 'Custom Regexps' field associated with 'Basic'
4. Ensure that the 'Regex' option is checked
5. Click the Anki icon on the ribbon to run the plugin


## Python Script users
3. Run the script, and check 'Config' to open up the config file:  
![GUI](Images/GUI_config.png)
4. Navigate to the "Custom Regexps" section
5. Change the line
<pre>
Basic =  
</pre>
to  
<pre>
Basic = ((?:[^\n][\n]?)+\n)-{3,}((?:\n(?:^.{1,3}$|^.{4}(?&lt;!&lt;!--).*))*)
</pre>
6. Save the config file
7. Run the script on the file, with 'Regex' checked:  
![GUI](Images/GUI_regex.png)

## All users
8. You should see these cards in Anki:  
![ruled_1](/Images/Ruled_1.png)  
![ruled_2](/Images/Ruled_2.png)