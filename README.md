# Hello-World
# My first dabbling
"""I made a hangman python game while following a tutorial that used a word guessing game as an example.
The hangman game makes players guess a letter at a time given a phrase."""
secret_word = "Elephant"
one_letter_at_a_time = ""
word_guess = ""
def Guess_a_Letter_at_a_Time_again():
    i = 0
    letter_guess = ""
    while i < len(secret_word):
        letter_guess = input("Input a letter:")
        print(letter_guess)
        print(secret_word[i])
        if letter_guess == secret_word[i]:
            k = i + 1
            print("Good guess. You have: ", secret_word[:k])
            i += 1
        else:
            print("Try again.")
    print("The secret word is: ",secret_word)
Guess_a_Letter_at_a_Time_again()
