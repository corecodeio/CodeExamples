# Counting sheep

## Description
Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

**Example:**
```
Input: 
    [True,  True,  True,  False,
    True,  True,  True,  True ,
    True,  False, True,  False,
    True,  False, False, True ,
    True,  True,  True,  True ,
    False, False, True,  True]
    
Output: 17
```


## Solution
```python
def count_sheeps(array_of_sheep):
  count = 0
  for sheep in array_of_sheep:
      if sheep:
          count += 1 
  return count
```

## Breaking down the solution
The syntax in python language is already self explanatory, because of the intention when developing the language, but here we also can notice that the variables have names related to the problem, and that just by reading the code you can know what is doing the code. Just a simple for and a simple if.

## Try it!
Click [here](https://www.programiz.com/python-programming/online-compiler/) to copy paste the code in a Python environment, just copy the code and make the call with the array that  you want, in this example `[True, True, False, True]`, to run the code just hit the **Run** button on the right.
Remember that each `True` represents a sheep. 

```javascript
def count_sheeps(array_of_sheep):
  count = 0
  for sheep in array_of_sheep:
      if sheep:
          count += 1 
  return count
 
# Printing the result of the call
sheeps = [True, True, False, True]
print(count_sheeps(sheeps))
```
