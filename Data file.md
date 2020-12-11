# Added Media

The data file stores the filenames of media that the script has previously added to Anki, to avoid unnecessarily adding media again.

# File Hashes

The data file also stores a dictionary of `filename: fileHash` key-value pairs. If the script identifies a file with the same filename and fileHash as an entry in the dictionary, it will skip over the file - this means that the script only properly scans unchanged files.

For less technical users, hashing is a process that takes a file and returns a fixed-length string that acts as a 'signature' for the file. Importantly, it is an **irreversible process** - the script is not covertly storing your data!