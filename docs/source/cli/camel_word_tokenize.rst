camel_word_tokenize
===================

About
-----

The ``camel_word_tokenize`` tool splits words from punctuation while collapsing
contiguous segments of spaces into a single whitespace character. 
It is also language agnostic and splits all characters marked as punctuation or
symbols in the Unicode specification.

For example the following sentence:

.. code-block:: none

   Hello,     world!!!!
   مرحبا يا عالم!!!

becomes:

.. code-block:: none

   Hello , world ! ! ! !
   مرحبا يا عالم ! ! !


Usage
-----

Below is the usage information that can be generated by running
``camel_word_tokenize --help``.

.. code-block:: none

   Usage:
       camel_word_tokenize [-o OUTPUT | --output=OUTPUT] [FILE]
       camel_word_tokenize (-v | --version)
       camel_word_tokenize (-h | --help)

   Options:
     -o OUTPUT --output=OUTPUT
           Output file. If not specified, output will be printed to stdout.
     -h --help
           Show this screen.
     -v --version
           Show version.
