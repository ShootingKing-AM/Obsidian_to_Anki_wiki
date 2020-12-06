Apart from the first field, each field must have a prefix to indicate to the program when to move on to the next field. For example:

<pre>
START
Basic
This is a test.
Back: Test successful!
END
</pre>

Note that you must start new fields on a new line for non-inline notes.  
When the script successfully adds a note, it will append an ID to the Note Data. This allows you to *update existing notes by running the script again*.

Example output:
<pre>
START
Basic
This is a test.
Back: Test successful!
&lt;!--ID: 1566052191670--&gt;
END
</pre>