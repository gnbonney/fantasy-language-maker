Fantasy Language Maker
----------------------

Makes fantasy language glossaries based on markov chains applied to text corpuses. Comes with some sample corpuses from Project Gutenberg. (http://www.gutenberg.org/wiki/Main_Page)

Requires an installation of the Python programming language version 3
http://www.python.org

My version requires spacy https://pypi.org/project/spacy/ for nlp.

To install after python is installed:

```
pip install spacy
python -m spacy download en_core_web_sm
```

I use this to tell whether an English word is noun, verb, etc.

Note: I also tried using spacy syllables to split words, but foud it doen's always work.

To run:

on linux/mac 
From the command line, type './markov [options] <path to corpus> [path to additional corpus..]'

on windows
From the dos prompt, 'python markov [options] <path to corpus> [path to additional corpus..]'

```
Usage: markov [options]

Options:
  -h, --help            show this help message and exit
  -l LOOKBACK, --lookback=LOOKBACK
                        number of characters to look back in the chain
  -d DICTIONARY, --dictionary=DICTIONARY
                        dictionary file to use
```                        

You can get additional corpora from Project Gutenberg - download the 'utf-8' version. I recommend removing the Gutenberg headers and footers before running the program on it.
