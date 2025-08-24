# Stone_paper_scissor_game
import random 
'''
1 for stone
-1 for scissor(c)
0 for paper
'''

computer = random.choice([1, -1, 0])
youstr = input("Enter your choice: ")
youDict = {"s": 1, "c": -1, "p": 0}
reverseDict = {1: "stone", -1: "scissor", 0: "paper"}

you = youDict[youstr]

print(f"You choose {reverseDict[you]}\nComputer choose {reverseDict[computer]}")

if(computer == you):
    print("Its a draw")

else:
    if(computer == -1 and you == 1):
        print("You win!")
    elif(computer == -1 and you == 0):
        print("You lose!")        
    elif(computer == 1 and you == 0):
        print("You lose!")        
    elif(computer == 1 and you == -1):
        print("You win!")        
    elif(computer == 0 and you == 1):
        print("You lose!")        
    elif(computer == 0 and you == -1):
        print("You win!")
    else:
        print("Something went wrong")
        
                      
