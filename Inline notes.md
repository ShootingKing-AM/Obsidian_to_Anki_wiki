These are formatted as such:  
<pre>
STARTI [{Note Type}] {Note Data} ENDI
</pre>
For example  
<pre>
STARTI [Basic] This is a test. Back: Test successful! ENDI  
</pre>
Unlike regular 'block' notes, you can put inline notes anywhere on a line - for example, you could have a bulletpointed list of inline notes.  
Also, unlike regular 'block' notes, the script identifies the note type through the string in square brackets. Hence, **note types with \[ or \] in the name are not supported for inline notes.**