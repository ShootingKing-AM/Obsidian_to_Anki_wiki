# Regular

The script can delete notes that *it has added* automatically. To do this:
1. Find the formatted note in your file:
<pre>
START
{Note Type}
{Note Data}
&lt;!--ID: {Identifier}--&gt;
END
</pre>
2. Change this to read:
<pre>
START
&lt;!--ID: {Identifier}--&gt;
END
</pre>
3. If you run the script on the file, it will interpret this as "delete the note with ID {identifier}". For convenience, it will also delete the unnecessary `START END` block from the file.

Note that if you manually delete a note in Anki, **you must remove the ID line from the text file**. Otherwise, the script will throw an error.

# Inline notes

The instructions are quite similar to deleting normal notes:
1. Find the formatted note in your file:
<pre>
STARTI [{Note Type}] {Note Data} &lt;!--ID: {Identifier}--&gt; ENDI
</pre>
2. Change this to read:
<pre>
STARTI &lt;!--ID: {Identifier}--&gt; ENDI
</pre>
3. If you run the script on the file, it will interpret this as "delete the note with ID {identifier}". For convenience, it will also delete the unnecessary `STARTI ENDI` block from the file.

Note that if you manually delete a note in Anki, **you must remove the ID line from the text file**. Otherwise, the script will throw an error.