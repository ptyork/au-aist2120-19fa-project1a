# Project 1a: English to Pig Latin Translator 

Pig Latin (aka, Ig-pay Atin-lay) is a classic "pseudo-language" that is based on a set of simple rules. Your job is to follow these rules to create a basic English to Pig Latin Translator. 

The script, `pltrans.py`, should: 

1. Ask the user for a file name 
2. Open the requested file 
3. Split the contents of the file into words 
4. Iterate over each word 
5. Translate the word to Pig Latin 
6. Output the translated word to the screen 

Follow the Pig Latin translation rules outlined here: 

[How to Speak Pig Latin](https://www.wikihow.com/Speak-Pig-Latin) 

ONLY worry about the first two rules. Treat "y" as a standard consonant. 

__THE HARD'ISH PART__: When splitting out the words, be careful to check the LAST character of the word. If it's punctuation, be sure to deal with that correctly. In other words, "well, let's go." should be "ell-way, et's-lay o-gay." NOT "ell,-way et's-lay o.-gay" 

## REQUIRED IMPLEMENTATION NOTES 

1. You MUST abstract your most useful logic by creating a function named translate that takes a word and returns the Pig Latin version (properly handling the punctuation issue outlined above). This function should be "called" as your step 5 above, which will make the main script much cleaner. So to reiterate, the following function MUST be in your code: 

``` 
      def translate(word): 
          ...
``` 

2. You MUST modify getty.txt, replacing Abraham Lincoln's name with your own.

3. You MUST then translate getty.txt and redirect the output to pig-getty.txt. In other words, you should run `python pltrans.py > pig-getty.txt` and select getty.txt when prompted. Include this translated file in your final submission. 

## LOGISTICS 

Same basic deal as with the homeworks. 

1. From your AIST2120 folder, run `git clone [URL]` to make a local copy of this assignment. 
2. DO THE WORK (create and complete any and all needed files)
3. TEST YOUR WORK A WHOLE LOT 
4. TEST IT SOME MORE LIKE YOU MEAN IT THIS TIME 
5. When done, run `git add .` 
6. Then run `git commit –m "type a clever message here"` 
7. Finally run `git push` to push your changes back up to GitHub 
8. Breathe a sigh of relief 

## OPTIONAL CHALLENGES 

1. Create a second version of the script, pltrans2.py. This version should import the translate function from pltrans (`from pltrans import translate`). Instead of asking for a file name and reading the text from the file, instead read in the text line-by-line from sys.stdin. This should allow you to run it interactively AND to pipe in text from another command (e.g., `type getty.txt | python pltrans2.py`). 

2. Ignore numbers (any "word" starting with a number).

3. Correctly implement the third rule from the How to Speak Pig Latin site.
