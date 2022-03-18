Midterm Project
Textblob Package
Ivan Ramirez

OPEN TERMINAL
pip install -U textblob
ENTER

python -m textblob.download_corpora
ENTER

pip install pyspellchecker
ENTER

python -m pip install requests
ENTER

  For my midterm project, I chose the textblob package and I chose to lookinto the spellchecker. Textblob is a python library that analyzes textual data. Textblob is able to analyze human language and is able to apply a vairety of different functions as making lists for certain words and such as the spellchecker that I used which also has multiple functions such as finding specific words that are mispelled and making a list out of them and making a auto-correct type of automization that will automatically correct the words that are mispelled and outputs the same thing except that it comes out with the correct words and rearranging the paragraph in a better alignment. 
  This was my second attempt of trying to use textblob and this time it was successful. When I first tried to install it, I was stuck for hours and could not find what I was doing wrong. I downloaded textblob successfully as well as a few additional packages in terminal, but when I ran the code through VS Code, it said that the packages were not found. This lead to me trying to find the package that was not downloaded and I just kept going in circles trying to find what was wrong for many hours. After I gave up, I went back and realized that I was not in the classenv when I was attempting to do the assignment. Once I did, I downloaded textblob in the class enviroment using pip install textblob in my machine's terminal. After this, I entered from textblob import TextBlob re to VS Code. Right after this, I entered docx= and put in a paragraph with several spelling mistakes. When this is ran, the order of the text is out of line and not uniform. To fix this, I used a regex command which was import re str=re.findall("[a-zA-Z,.]+",docx) updated_docx=(" ".join(str))print(updated_docx). Once this is ran, the paragraph that I entered was outputted in a uniform manner making it easier to read. Then, to showcase texblobs lists/spellchecking ability, I entered from spellchecker import SpellChecker spell = SpellChecker() misspelled = spell.unknown(str) print(misspelled). This made a list with every mispelled word in the paragraph that was initially entered making it easy to see what was mispelled. From here, as a final entry, I entered new_doc = TextBlob(updated_docx) result = new_doc.correct() print(result). This gave the final product with the previous functions added to it which made the pragraph uniform and changed the mispelled words into the correct spelling.
  I would like to further develop this code with the textblob package to oraganize incorrect spelling in papers or essays to spell check, properly format, and auto correct what is wrong which would allow the user to not just see what they spelled wrong, but it would also make the changes for the user which would be a lot easier. I am unsure if there is a word limit through atom or VS Code as I was unable to find that information, but if a student were to put their essay through this code it could be a lot easier to use as a spellchecker without having to sign up for any websites and would allow for more efficient papers through using this code.
