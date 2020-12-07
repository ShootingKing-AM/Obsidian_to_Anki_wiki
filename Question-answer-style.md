**[[Regex]] line:** `^Q: ((?:.+\n)*)\n*A: (.+(?:\n(?:^.{1,3}$|^.{4}(?<!<!--).*))*)`

**Example usage:**
1. Create a file called `test.md`
2. Paste the following contents into the file:

<pre>
Q: How do you use this style?
A: Just like this.

Q: Can the question
run over multiple lines?
A: Yes, and
So can the answer

Q: Does the answer need to be immediately after the question?


A: No, and preceding whitespace will be ignored.

Q: How is this possible?
A: The 'magic' of regular expressions!
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
Basic = ^Q: ((?:[^\n][\n]?)+)\n+A: ((?:[^\n][\n]?)+)
</pre>
6. Save the config file
7. Run the script on the file, with 'Regex' checked:  
![GUI](Images/GUI_regex.png)
8. You should see these cards in Anki:  
![question_1](Images/Question_1.png)  
![question_2](Images/Question_2.png)  
![question_3](Images/Question_3.png)  
![question_4](Images/Question_4.png)