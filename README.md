# Hangman

## Introduction

Hangman is a classic game in which a player thinks of a word and the other player tries to guess that word within a certain amount of attempts.

### Usage

This is an implementation of the Hangman game, where the computer thinks of a word and the user tries to guess it. 

#### Documentation

A Hangman Game that asks the user for a letter and checks if it is in the word. It starts with a default number of lives and a random word from the word_list.

word_list = ['apple', 'banana', 'orange', 'pear', 'strawberry', 'watermelon']

 num_live = 5

- Parameters

  1. word_list: list
    The list of words to be used in the game

  2. num_lives: int
    The number of lives the player has

- Attributes 

   1.  word: str
        The word to be guessed picked randomly from the word_list

   2.  word_guessed: list
        A list of the letters of the word, with '_' for each letter not yet guessed
        For example, if the word is 'apple', the word_guessed list would be ['_', '_', '_', '_', '_']
        If the player guesses 'a', the list would be ['a', '_', '_', '_', '_']

    3. num_letters: int
        The number of UNIQUE letters in the word that have not been guessed yet

    4. num_lives: int
        The number of lives the player has

    5. list_letters: list
       A list of the letters that have already been tried

