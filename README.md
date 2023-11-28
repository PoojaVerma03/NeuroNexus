# NeuroNexus
import random
user_choice=int(input("Enter your choice : Type 0 for Rock , 1 for Paper , 2 for Scissors. "))
if(user_choice>=3 or user_choice<0):
    print("You Entered Invalid number. You Lose .")
else:
    computer_choice= random.randint(0,2)
    print("Computer chose : ")
    print(computer_choice)
    if(computer_choice == user_choice):
        print("Its a draw.")
    elif(computer_choice == 0 and user_choice == 2):
        print("You Lose.")
    elif(computer_choice == 2 and user_choice ==2 ):
        print("You Win. ")
    elif(computer_choice > user_choice):     # 0 2 condition should be put before this one (order matters)
        print("You Lose.")
    elif(computer_choice < user_choice):
        print("You Win. ")




