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


 5.      Deploying functions

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


  6.     class definition
          class Hangman:
  
        def __init__(self, word_list, num_lives):
        self.word_list = word_list
        self.num_lives = num_lives

       # Select a randomly guessed word from word_list

        import random

        word_list = ['apple', 'banana', 'orange', 'pear', 'strawberry', 'watermelon']

        print(random.choice(word_list))


      # selected random word from word_list is word_guessed

        word_guessed = 'orange'

        word_guessed = ['o', 'r', 'a', 'n', 'g', 'e',]


       # Determine the number of letters in word_guessed
     
       num_letters = len(word_guessed)

       word_guessed = ['o', 'r', 'a', 'n', 'g', 'e']

      print(num_letters)

      num_letters = 6


     # The number of lives the player has at the start of the game 'num_lives'

      num_lives = 5


     # Define a method called check_guess and pass guess a parameter.

      check_guess = input('guess:').lower()

      print(check_guess)


      # checking of guess_letter is in word_guessed

     guess = "r"

      word_guessed = ['o', 'r', 'a', 'n', 'g', 'e']

      for char in word_guessed:
  
       if char == "r":
   
      print("Good guess!{r}is in the word.")

      guess = "r"

      
      # Replacing the underscore in word_guessed with r

       wordrguessed = ['o', 'r', 'a', 'n', 'g', 'e']

       for char in wordrguessed:
  
        if char == "r":
        
        for r in wordrguessed:

       print (r)

        if r == 'orange':  
         break
  
         print(r)


      # letter not in word

      guess ='P'
       word_guessed = ['o', 'r', 'a', 'n', 'g', 'e']

      f or letter != word reduce num_lives by 1:

       print("Sorry, {'p'} is not in the word.")
      else:
       print( "You have {4} lives left.")


    # ask_for_input method
  
     while True:  
     
     guess = input('choose a single letter:')

     x = guess.isalpha()

     if guess != "a single alphabet char":

      print("invalid letter")

      list_of_guesses = ['b', 'y', 'm', 'j', 'k']

      # appending list_of_guesses with user-guess

       user_guess = 'r'
       list_of_guesses = ['b', 'y', 'm', 'j', 'k']
       list_of_guesses.append("r")

        print(list_of_guesses)

         ##### Class definition
         # class definition
class Hangman:
  
  def __init__(self, word_list, num_lives):
     self.word_list = word_list
     self.num_lives = num_lives

#Select a randomly guessed word from word_list

import random

word_list = ['apple', 'banana', 'orange', 'pear', 'strawberry', 'watermelon']

print(random.choice(word_list))

# selected random word from word_list is word_guessed

word_guessed = 'orange'

word_guessed = ['o', 'r', 'a', 'n', 'g', 'e',]

# Determine the number of letters in word_guessed
     
num_letters = len(word_guessed)

word_guessed = ['o', 'r', 'a', 'n', 'g', 'e']

print(num_letters)

num_letters = 6

# The number of lives the player has at the start of the game 'num_lives'

num_lives = 5

# Define a method called check_guess and pass guess a parameter.

check_guess = input('guess:').lower()

print(check_guess)


# checking if guess_letter is in word_guessed

guess = "r"

wordrguessed = ['o', 'r', 'a', 'n', 'g', 'e']

for char in word_guessed:
  
 if char == "r":
   
  print("Good guess!{r}is in the word.")

  for r in wordrguessed:
    print (r)

  if r == 'orange':  
    break
  
    print(r)

# letter not in word

guess ='P'

word_guessed = ['o', 'r', 'a', 'n', 'g', 'e']

if 'P' != word_guessed: num_lives < 1

num_lives = 4 



print("Sorry, {'p'} is not in the word.")


print('num-lives')


#  ask_for_input method
  
while True:  
     
     guess = input('choose a single letter:')

     x = guess.isalpha()

     if guess != "a single alphabet char":

      print("invalid letter")


    # The number of lives the player has at the start of the game 'num_lives'

     num_lives = 5  

###### Game

     class Hangman():
       
       def __init__(self, word_list, num_lives=5):
        
        self.word_list = word_list
        self.num_lives = num_lives


        class Hangman():
       
       def __init__(self, word_list, num_lives=5):
        
        self.word_list = word_list
        self.num_lives = num_lives


        def Hangman(game):
          return game
        print(Hangman)

        def word_guessed(word_list):
         return word_list
        print(word_guessed)

        word_list = ['apple', 'banana', 'orange', 'pear', 'strawberry', 'watermelon']

        word_guessed = ['o', 'r', 'a', 'n', 'g', 'e'] 

        num_letter = len(word_guessed)
        print(num_letter)
        
        

        for guess in word_guessed, "num_lives"  > 0:

         def game(guess, num_lives):
           
           return num_lives and guess
         
        print(game)

        while True:
             
             if num_lives == 0:

              print('you lost!')

             if num_lives != 0 and "num_letter" <= 0:
               
               print('Congratulations. You won the game!')

           
             num_lives.guess = game


             guess = list_of_guesses.pop(0) 
             

             game(num_lives, guess)
            
             list_of_guesses = ['b', 'y', 'm', 'j', 'k']

             guess_1 = list_of_guesses.pop(0)
             print(guess_1)
             print(list_of_guesses)

             num_lives = 5-1 
             print(num_lives)

             num_letter = 6-1

             list_of_guesses = ['y', 'm', 'j', 'k']
             guess_2 = list_of_guesses.pop(0)
             print(guess_2)
             print(list_of_guesses)
                        
             num_lives = 5-2 
             print(num_lives)

             num_letter = 6-2
             print(num_letter)

             list_of_guesses = ['m', 'j', 'k']
             guess_3 = list_of_guesses.pop(0)
             print(guess_3)
             print(list_of_guesses)
             
             num_lives = 5-3 
             print(num_lives)

             num_letter = 6-3
             print(num_letter)
             
             list_of_guesses = ['j', 'k']
             guess_4 = list_of_guesses.pop(0)
             print(guess_4)
             print(list_of_guesses)

             
             num_lives = 5-4 
             print(num_lives)

             num_letter = 6-4
             print(num_letter)

             list_of_guesses = ['j', 'k']
             guess_5 = list_of_guesses.pop(0)
             print(guess_5)
             print(list_of_guesses)

             num_lives = 5-5 
             print(num_lives)
             num_letter = 6-5

             
             if num_lives == 0:

              print('you lost!')

             if num_lives != 0 and "num_letter" <= 0:
               
              print('Congratulations. You won the game!')