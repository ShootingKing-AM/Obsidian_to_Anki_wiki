# Per-note basis

For reference, the note formatting style is:

<pre>
START
{Note Type}
{Note Fields}
Tags:
END
</pre>
Note that the Tags: line is optional - if you don't want tags, you may leave out the line.

Tags should be formatted as such:
<pre>
Tags: Tag1 Tag2 Tag3
</pre>
So, **a space between the colon and the first tag**, and a space between tags.

Hence, this syntax **would not work**:
<pre>
Tags:Tag1 Tag2 Tag3
</pre>

The above section only applies to regular notes - see [[Inline notes]] and [[Regex]] for respective information on those note types.

# Per-file basis

These tags will be added to every card in the file.

To do this:
Anywhere within the file, format the file tags as follows:
<pre>
{File Tags Line}
{Tag list}
</pre>
For example, with the default settings:
<pre>
FILE TAGS
Maths School Physics
</pre>
Like with tag-line formatting, you need a space between tags - however, do not include the "Tags: " prefix.