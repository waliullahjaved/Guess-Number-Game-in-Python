# Guess-Number-Game-in-Python
import random
num=random.randint(1,10)
print(num)
tries=0
while True:
    guess=int(input("enter a number to guess this number"))
    if guess == num:
        print(f"You enter rght number and you try {tries} times")
        tries+=1
        break
    elif guess > num:
        print("go a little lower")
        tries+=1
    elif guess < num:
        print("go little higher")
        tries+=1
    else:
        print("you enter a wrong number")
        tries+=1
