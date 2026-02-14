# To restore the image, you need to reverse these steps.

First, read the file contents as text and shift every character backward by 3 positions. Conceptually, this can be done by converting each character to its numeric code, subtracting 3, and converting it back to a character. For example, in Python, the core transformation looks like this:

`result = "".join(chr((ord(c) - shift) % 256) for c in data)`

the resulting text is a standard textual encoding commonly used to represent binary files safely inside text-based systems

Second, take the text you get after reversing the shift, determine what textual encoding format it is, and convert it back into a binary image file, saving the output as a .png.
