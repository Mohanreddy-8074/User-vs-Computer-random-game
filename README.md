# User-vs-Computer-random-game
In the code we to play a game with user and computer if same as input from user and computer it will show like a draw...etc.By using random functions in python i have to create this project.
import random
rock='''
🪨
🪨🪨
🪨🪨🪨
🪨🪨🪨🪨'''
paper='''
🧻🧻🧻🧻🧻
🧻🧻🧻🧻🧻
🧻🧻🧻🧻🧻
'''
scissor='''
✂️✂️✂️✂️✂️
✂️✂️✂️✂️✂️
✂️✂️✂️✂️✂️
'''
game=[rock,paper,scissor]
user_input=int(input("enter your choice 0 is Rock,1 is Paper,2 is Scissor: " ))
if user_input > 2 or user_input<0:
    print("Invalid input.Try again....!")
else:
    print(game[user_input])
    computer_input=random.randint(0,2)
    print("computer Input: ")
    print(game[computer_input])
    if user_input==computer_input:
        print("It's Draw.")
    elif user_input==0 and computer_input==2:
        print("Computer Wins")
    elif user_input==2 and computer_input==0:
        print("You win.")
    elif user_input > computer_input:
        print("You Loose.")
    elif user_input < computer_input:
        print("You Win")

