# caesar-cipher
A Python program to implement Caesar-cipher encryption

Team: 1-3 people

Challenge: Easy/Intermediate

The Caesar cipher (https://en.wikipedia.org/wiki/Caesar_cipher) is one of the simplest forms 
of encoding messages.  Mapping each letter of the alphabet to a number in sequence,

    A   B   C   D   E   ...    X    Y    Z
    |   |   |   |   |          |    |    |
    1   2   3   4   5   ...   24   25   26

convert each letter of the plaintext into its number, add a constant to that number, and then 
convert back to letters using the same map.  Thus, the plaintext "BABY" is encoded with a 
shift constant of '3' to become

BABY ->  2 1 2 25
     -> (2+3) (1+3) (2+3) (25+3)
     -> 5 4 5 2
     -> EDEB
    
(notice that we "wrap around" back to A=1 when adding the constant takes us past Z=26 so that 
25+3 goes to 2).

If you know the shift constant that was added, it's easy to reverse the encoding to recover the 
original text 'BABY'.  If you don't, however, then it's not immediately obvious to you what the 
plaintext was from reading 'EDEB'.

This program should allow the user to input a unit of text and to specify a shift factor.  It 
should return the encoded text.

Intermediate Challenge 1
Display the output of the program as an animation.  The output starts as the entered plaintext, 
and it converts to the encrypted text letter-by-letter, randomly (like when movies show codes 
being encrypted and decrypted).

Intermediate Challenge 2
Extend the program to scrape and encode a paragraph of text from Wikipedia, selected randomly 
or by whichever criteria you like.
