
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
# Added a sapce in between " " to count the spaces