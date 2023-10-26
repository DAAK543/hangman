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

##### Methods

  class Hangman: 

  1. Initialize attributes in docstring

  def __init__(self, word_list, num_lives=5):
        
       self.word_list = word_list
       self.num_lives = num_lives

  2. Select a randomly guessed word from word_list

   import random

   word_list = ['apple', 'banana', 'orange', 'pear', 'strawberry', 'watermelon']

   print(random.choice(word_list))
  
   word_guessed = 'watermelon'
 
  3. Determine the number of characters in word_guessed
     
     num_letters = len(word_guessed)

     print(num_letters)

     num_letters = 10

 4. Select a random letter from the word_guess
    
    word_guessed = 'watermelon'

     guess = 't'

     user_input = input('please guess a letter:').lower()

     while user_input == guess:   
  
     print(user_input)

      - Check if guessed letter is an alphabet

        guess = 't'

        x = guess.isalpha()

        print(x)

         if "t" == "alphabet":
          "break"
         else:

           print("Invalid letter. Please, enter a single alphabetical character.")


      - check if guessed letter is in word_guessed

         guess = "t"

         word_guessed = "watermelon"

         for char in word_guessed:
  
         if char == "t":
   
         print( "Good guess! {t} is in the word.")

         else: 
           print("Sorry, {t} is not in the word. Try again.")

    5. Deploying functions

       def check_guess(guess):
  
         if guess == "t":

         return input('please guess a letter:').lower()
  
         print(check_guess)
  
         "break" 


        print("Invalid letter. Please, enter a single alphabetical character.")
     


       def ask_for_input(guess):
  
         for guess in word_guessed:
  
         if guess == "t" and word_guessed == "watermelon":

        print("Good guess! {t} is in the word.")