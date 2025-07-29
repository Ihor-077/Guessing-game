# Guessing Game 🎯

This is a simple Python word guessing game.  
You have 3 tries to guess the secret word.

## 🧠 What You Learn

- `while` loops
- `if`/`else` conditions
- User input handling
- Basic game logic

## 💻 How to Play

1. Run the program
2. Try to guess the secret word within 3 tries
3. Win or lose based on your input!

---------------------------------------------------------------

print("You have 3 tries to guess the word")
secret_word = "Gym"
guess = ""
guess_count = 0
guess_limit = 3
out_of_guesses = False

while guess != secret_word and not(out_of_guesses):
    if guess_count < guess_limit:
     guess = input("Guess a word:")
     guess_count += 1
    else:
        out_of_guesses = True
if out_of_guesses:
    print("Out of guesses! YOU LOSE!")
else:
    print("You win!!!")
