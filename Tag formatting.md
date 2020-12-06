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

# Per-file basis

v1.1.1 now allows you to specify 'file tags' for a file - these tags will be added to every card in the file.

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