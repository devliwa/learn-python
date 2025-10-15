# hangman

- [learn-links1](https://hangmanwordgame.com/?fca=1&success=0#/)
- [Python Lists](https://developers.google.com/edu/python/lists#for-and-in)
- [Python import Statement](https://www.askpython.com/python/python-import-statement)

  ```python
  import random
   word_list = ["aardvark", "baboon", "camel"]

  chosen_word = random.choice(word_list)
  print(chosen_word)

  guess = input("Guess a letter: ").lower()

  for letter in chosen_word:
    if letter == guess:
        print("Right")
    else:
        print("Wrong")


