If the script itself is not able to run, try running `python3 {PATH_TO_SCRIPT}`.

If you are unable to get `pip` to run, see this [user guide](https://pip.pypa.io/en/stable/user_guide/).

Some people have reported issues with installing the `Gooey` dependency. From v2.5.0 onwards, the script can run without `Gooey`, falling back to a command-line interface.

The script was written in Python 3.8.5, and it uses `os` module features from Python 3.6+ [This issue](https://github.com/Pseudonium/Obsidian_to_Anki/issues/6#issue-690905446) confirms that the script does not run on Python 2.