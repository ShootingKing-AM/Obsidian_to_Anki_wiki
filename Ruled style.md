**[[Regex]] line:** `((?:[^\n][\n]?)+\n)-{3,}\n((?:[^\n][\n]?)+)`

**Example usage:**
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
3. Run the script, and check 'Config' to open up the config file:  
![GUI](Images/GUI_config.png)
4. Navigate to the "Custom Regexps" section
5. Change the line
<pre>
Basic =  
</pre>
to  
<pre>
Basic = ((?:[^\n][\n]?)+\n)-{3,}\n((?:[^\n][\n]?)+)
</pre>
6. Save the config file
7. Run the script on the file, with 'Regex' checked:  
![GUI](Images/GUI_regex.png)
8. You should see these cards in Anki:  
![ruled_1](/Images/Ruled_1.png)  
![ruled_2](/Images/Ruled_2.png)