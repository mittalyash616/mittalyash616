import random
def run(ask):
    if ask=="1":
        print("start the game now")
        print("press")
        print("1.rock")
        print("2.paper")
        print("3.scissor")
        user_input=int(input("please enter your choice: "))
        system_input=random.randint(1,3)
        if user_input==1 and system_input==2:
            print("bad luck, computer wins")
        elif user_input==2 and system_input==3: 
            print("bad luck, computer wins")
        elif user_input==3 and system_input==1: 
            print("bad luck, computer wins")
        elif user_input==1 and system_input==3: 
            print("congratulation, you wins")   
        elif user_input==2 and system_input==1: 
            print("congratulation, you wins") 
        elif user_input==3 and system_input==2: 
            print("congratulation, you wins")      
    elif ask=="2":
        print("start the game now")
        print("press")
        print("1.rock")
        print("2.paper")
        print("3.scissor")
        user_input1=int(input("please enter 1st person choice: "))
        user_input2=int(input("please enter 2nd person choice: "))
        if user_input1==1 and user_input2==2:
            print("bad luck, user2 wins")
        elif user_input1==2 and user_input2==3: 
            print("bad luck, user2 wins")
        elif user_input1==3 and user_input2==1: 
            print("bad luck, user2 wins")
        elif user_input1==1 and user_input2==3: 
            print("congratulation, user1 wins")   
        elif user_input1==2 and user_input2==1: 
            print("congratulation, user1 wins") 
        elif user_input1==3 and user_input2==2: 
            print("congratulation, user1 wins") 

#project rock paper scissor 
print("~"*60)
print("welcome guys in our python program called rock paper scissor")
print("~"*60)
print()
ask=input("hello, want to play the game (yes or no) ?  ")
if ask=="no":
    quit()
print()
while ask=="yes":
    print("press")
    print("1.single player")
    print("2.multi player")
    ask=input("please enter the number: ")
    run(ask)
    ask=input("hello, want to play the game more (yes or no) ?  ")

