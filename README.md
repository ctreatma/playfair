# Playfair

This is a Scala implementation of the [Playfair cipher](http://en.wikipedia.org/wiki/Playfair_cipher).

## Running Playfair

You can run Playfair from the command line by executing `scala -classpath bin Playfair`.  A file chooser will pop up to allow to to select a file to encode or decode.

### File format

The first line of the file defines the action that should be performed and the keyword that should be used when performing that action.  Options are:

    encipher <keyword>
    decipher <keyword>

A Playfair cipher will be generated based on `<keyword>`, and the cipher will be applied to the remainder of the selected file.  `encipher.txt` is a sample file for encoding a message, and `decipher.txt` is a sample file for decoding an encoded message.  Enciphered messages are grouped into quintuples for output.  Deciphered messages contain no whitespace.
