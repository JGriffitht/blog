
**Debugging is a process of identifying errors in your code called “bugs”.** The way I go at debugging is starting to look for bugs in my code and changing one thing at a time, this allows me to experiment and pinpoint my assumptions on what I have done wrong.

----------------------------------------------------------------------------------------------------

In These lines of code are meant for figuring out how many spaces are given in a string but the problem I found with it is that it wasn't counting the spaces that were in the string so using the method of the way I go at debugging I started at the top first the two variables are labeled text for string and count for each space then reading my for loop that something I was looking out for in the text was not stated in the quotations and I had to state what I wanted it to count in the text.

```python
text = "Hello, world, my name is"
count = 0

for char in text:
    if char == " ":
        count += 1

print(count)
# added a spac in between the quations to count the spaces.
```
****************************************************************************************************

in these next lines of code they meant to find if the numbers 1 through the user input of number is even or odd but when going over this I found out I was getting an error because I was asking the user for a string and not integer along with the operation sign changing it to an equal sign allowing it to take the users input and tell the user if the numbers are even are odd depending on what number was imputed.

```python
print("give me a number")
n = int(input())

for num in range(1, n):
    if num % 2 == 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")
        #checking if the number is dividable by two then made sure the input was a intenger
```

----------------------------------------------------------------------------------------------------

These lines of code is supposed to calculate the factorial number given through the input of the user but when going over the code I found out that the the number inputs I used was wrong I needed to change the numbers used to calculate the number changing the loop range to 1 plus the number and removing a negative I had.

```python
num = int(input("Enter an integer: "))

if num < 0:
    print("No negative numbers.")
else:
    result = 1
    for i in range(1, num + 1):
        result *= i

    print(f"Factorial of {num} is {result}")
    #changed the rangses and changed some numbers to find the correct ranges of the number
 ```

****************************************************************************************************

This is supposed to allow the user three attempts using a password after three attempts it will lock the user out prompting them with “Too many attempts” after debugging this code I found out that I was making it check for if the password was incorrect and not for the correct password and added a break to end the loop when the password was guessed.

```python
attempts = 0
correct_password = "secret"

while True:
    password = input("Enter your password: ")
    attempts += 1

    if password == correct_password:
        print("Correct password!")
        break
    else:
        print("Incorrect password")

    if attempts >= 3:
        print("Too many attempts")
        break
# fixed the varible that it was looking for also changed to be equal to three so the user doesnt go over the attempts given
```
