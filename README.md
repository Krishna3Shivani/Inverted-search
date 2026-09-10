# Inverted-search

## project overview

A command-line based Inverted Search Engine implemented in C that creates an index of words from multiple text files and allows fast searching of words and their occurrences across files.

## Technologies Used

* C Programming
* Hash Table
* Linked Lists
* File Handling
* Pointers & Structures

## Features

* Create an inverted index from multiple text files
* Search for words across indexed files
* Display the complete database
* Save and update the database
* Track word frequency in each file

## How It Works

The program uses a **27-bucket hash table** based on the first character of each word.

Each hash-table entry points to a linked list containing the word and its file details. When a word is searched, its hash index is calculated and the corresponding list is searched instead of scanning every file.

Text Files
    ↓
Hash Table
    ↓
Word → File → Word Count
    ↓
Search / Display / Save / Update
