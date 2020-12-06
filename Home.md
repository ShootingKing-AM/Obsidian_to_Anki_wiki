# Current features
* **[[Note formatting|Custom Note Types]]** - You're not limited to the 6 built-in note types of Anki.
* **Updating notes from file** - When running the script on a file again, it'll automatically update existing notes in Anki, preserving scheduling information.
* **[[Tag formatting|Tags]]**.
* **Adding to user-specified [[Deck formatting|Decks]],** on a *per-file* basis.
* **[[Markdown formatting]]**.
* **[[Math formatting]]**.
* **[[Image formatting|Images]]**.
* **[[Audio formatting|Audio]]**
* **[[Deleting notes|Auto-deleting notes]] from the file**.
* **Reading from all files in a directory automatically** - recursively too!
* **[[Inline notes]]** - Shorter syntax for typing out notes on a single line.
* **[[Cloze formatting|Easy Cloze formatting]]** - A more compact syntax to do Cloze text.
* **[[Obsidian Integration]]** - Currently, this only includes a link to the file that made the flashcard, appended to the first field of your card.
* **[[Regex|Custom Syntax]]** - Using **regular expressions**, add custom syntax to generate **notes that make sense for you.** Some examples:
  * [RemNote single-line style](regex.md#remnote-single-line-style). `This is how to use::Remnote single-line style`  
  ![Remnote 1](Images/Remnote_1.png)
  * [Header paragraph style](regex.md#header-paragraph-style).
  <pre>
  # Style
  This style is suitable for having the header as the front, and the answer as the back
  </pre>  
  ![Header 1](Images/Header_1.png)
  * [Question answer style](regex.md#question-answer-style).
  <pre>
  Q: How do you use this style?
  A: Just like this.
  </pre>  
  ![Question 1](Images/Question_1.png)
  * [Neuracache #flashcard style](regex.md#neuracache-flashcard-style).  
  <pre>
  In Neuracache style, to make a flashcard you do #flashcard
  The next lines then become the back of the flashcard
  </pre>  
  ![Neuracache 1](Images/Neuracache_1.png)
  * [Ruled style](regex.md#ruled-style)  
  <pre>
  How do you use ruled style?
  ---
  You need at least three '-' between the front and back of the card.
  </pre>  
  ![Ruled 1](Images/Ruled_1.png)
  * [Markdown table style](regex.md#markdown-table-style)  
  <pre>
  | Why might this style be useful? |
  | ------ |
  | It looks nice when rendered as HTML in a markdown editor. |
  </pre>
  ![Table 2](Images/Table_2.png)
  * [Cloze paragraph style](regex.md#cloze-paragraph-style)  
  <pre>
  The idea of {cloze paragraph style} is to be able to recognise any paragraphs that contain {cloze deletions}.
  </pre>
  ![Cloze 1](Images/Cloze_1.png)

Note that **all custom syntax is off by default**, and must be programmed into the script via the config file - see [Custom syntax](regex.md) for instructions.

[[History of script development]]

However, you don't need to have your notes be files of flashcards to use this script! You just need to be fine with visibly embedding flashcards in your notes, and keeping them there for future reference/editing. The script will ignore anything it doesn't think is a flashcard, so you're free to add context/information not needed for Anki to your notes.

[[Setup]]

[[Usage]]

[[Steps for new users]]

[[Deck formatting]]

[[Note formatting]]

[[Deleting notes]]

[[Inline notes]]

[[Cloze formatting]]

By default, the script adds to the current profile in Anki.  

[[Troubleshooting]]

[[Technical]]