Clacks
======

This is intended to be a system that converts characters into the clacks semaphore system, and back again.

Clacks Formation
----------------
The literature suggests that the clacks system consisted of 8 shutters[1], although there are clacks interpretations that use 6 shutters, most notably the release of the Clacks board game. The board game Clacks is very limited in that it defines only the letters A-Z, a space, and the END character. I may base my clacks interpretations on this, adding to the symbol list to define extra characters, punctuation, numerals, and so on.

I'm still debating whether to use ASCII conversions of the 8 bit value directly, with each "lamp" representing a bit, or to use the Unified 8-dot Braille system, which also consists of 8 "bits", but doesn't seem to conform to the ASCII system.
For the 6-shutter version of Clacks, it may be easier to use the English Braille system which also uses 6 dots. However, the system used in the Clacks boardgame doesn't conform to 6-dot braille, unfortunately.[2]
It seems that the similarity between Braille and the Clacks board game is that they are case insensitive. I intend to include a case sensitive option for this software, but it will be guaranteed that the clacks glyphs for uppercase letters used in the insensitive version will correspond with those for the lower case letters used in the sensitive version.

In fact I'll probably end up using the binary ASCII system anyway, as having access to all the unprintable characters between 0 and 31 (inclusive) means I can use them as control characters (much like they're used on computers anyways).

Also, is it cruel to create a light-shutter based semaphore system which requires vision and base it on a reading system designed for visually impaired people?

https://en.wikipedia.org/wiki/Braille_Patterns
http://www.roubaixinteractive.com/PlayGround/Binary_Conversion/The_Characters.asp

Software Options
----------------

I intend to create a computer based clacks implementation that supports case (in)sensitivity, and both 6/8 shutter versions of the clacks semaphore. I'll also be implementing the control characters, such as G (Send message on), N (Do not log message), U (At the end of the line, send it back again). This means I'll need to figure out some way of identifying incoming clacks signals as overhead or not. I also need to figure out how to send both plaintext and encrypted clacks signals. I'll be starting out with plain text, and branching off into signals at a later date.

References/Citations
--------------------

[1] The Fifth Elephant, Page 24: "Lord Vetinari stood at his window watching the semaphore tower on the other side of the river. All eight of the big shutters facing him were blinking furiously - black, white, white, black, white..."

[2] As illustrated here: on the left is the letter "a" in English 6-dot Braille. On the right, is the letter "a" in Clacks board game semaphore, which interestingly corresponds to either the value "en", or "?" in English 6-dot Braille.

![a-braille](https://upload.wikimedia.org/wikipedia/commons/2/2c/Braille_A1.svg "a in Braille") ![a-clacks](https://upload.wikimedia.org/wikipedia/commons/9/97/Braille_QuestionMark.svg "A in Clacks game.")
