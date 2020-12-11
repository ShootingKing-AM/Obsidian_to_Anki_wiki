Inspired by the Frozen Fields addon for Anki.

Anywhere in your file, you can place the following structure:

```
FROZEN - {Note type}:
{Field 1}: {Content 1}
{Field 2}: {Content 2}
...

```

As an example, if your note type was called "Question with context", and had a field called "Context", here's how you'd do it:

```
FROZEN - Question with context:
Context: What is the country's capital?

```

Then, every note of type "Question with context" will have "What is the country's capital?" automatically appended to the "Context" field.

You can do this for multiple different note types, though do not create multiple FROZEN blocks for the same note type. Also, FROZEN blocks should be separated from other content by a newline at the top and bottom to avoid errors.