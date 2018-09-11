# Hello 

### Double Char 
##### https://www.codewars.com/kata/56b1f01c247c01db92000076/train/python
#### Given a string, you have to return a string in which each character (case-sensitive) is repeated once. 

```python
def double_char(s):
    
    #initialize empty string to add characters to
    new_string = ""
    
    #loop through the string and add two of each character
    for char in s:
        new_string += (char*2)
        
    return new_string
```

### Sum of a Beach
##### https://www.codewars.com/kata/sum-of-a-beach/train/python 
#### Beaches are filled with sand, water, fish, and sun. Given a string, calculate how many times the words "Sand", "Water", "Fish", and "Sun" appear without overlapping (regardless of the case).

```python
def sum_of_a_beach(beach):
    
    #create list of words we are looking for
    beach_words = ['sand', 'water', 'fish', 'sun']
    
    #set a counter to count the words
    counter = 0
    
    #loop through the list of words and count the number of occurrences in the string
    for word in beach_words:
        counter += beach.lower().count(word)
        
    return counter
```

### Sum of All the Multiples of 3 or 5
##### https://www.codewars.com/kata/sum-of-all-the-multiples-of-3-or-5/train/python 
#### Your task is to write a function findSum. Up to and including n, this function will return the sum of all multiples of 3 and 5. For example: findSum(10) should return 33 (3 + 5 + 6 + 9 + 10)

```python
def find(n):
    
    #initialize list to store multiples of 3 and 5
    match = []
    
    #find which integers at and below n are multiples of 3 or 5, and append them to the list
    while n > 0:
        if n % 3 == 0 or n % 5 == 0:
            match.append(n)
        n -= 1
    print match
    
    #sum the multiples
    return sum(match)
```
