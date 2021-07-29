# Python-Webinar

1. Calculator

num1 = int(input("Please enter first number : "))

num2 = int(input("Please enter second number : "))

op = input("Please select your operator- +,-,*,/ ")

if op == "+" :

    print(num1 + num2)

elif op == "-" :

    print(num1 - num2)

elif op == "*" :

    print(num1 * num2)

else:

    print(num1 / num2)


---------------------------------------------------------------------------------------------

2. Guess a number - 

import random

num = random.randint(1, 100)

guess = None


while guess != num:

    guess = input("guess a number between 1 and 100: ")

    guess = int(guess)

    if guess == num:

        print("congratulations! you won!")

        break

    elif guess > num:

        print("Nope, sorry. your number is greater than the actual number")

    else:

        print("Nope, sorry. your number is smaller than the actual number")
-------------------------------------------------------------------------------------------------------------
3. Calender

import calendar

yy = int(input("Please tell your birth year : "))

mm = int(input("Please tell me your birth month : "))

print(calendar.month(yy, mm))

print(calendar.calendar(yy))

---------------------------------------------------------------------------------------------------------

4. Stopwatch

import time

def countdown(timer):

    while timer:

        mins, secs = divmod(timer, 60)

        timeformat = '{:02d}:{:02d}'.format(mins, secs)

        print(timeformat)

        time.sleep(1)

        timer -= 1
    print("stop1")

countdown(10)

--------------------------------------------------------------------------------------------------
5. Text to Speech

import pyttsx3​

frnd  = pyttsx3.init()​

name = input (' Please enter your name ')​

msg = "hello "+ name +". Welcome to bitLabs webinar session, Have a nice day!!"​

frnd.say(msg)​

frnd.runAndWait()​

​
