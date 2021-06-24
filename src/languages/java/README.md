# Sum of positive

## Description
You get an array of numbers, return the sum of all of the positives ones.
Note: if there is nothing to sum, the sum is default to 0

## Examples
```
    Input: [1, -4, 7, 12]
    Output:  20

    Explanation:  1 + 7 + 12 (without the -4)
```

## Solution
```java
public class Positive {
    public static int sum(int[] numbers) {
        int sum = 0;
        for(int number : numbers) {
            if(number > 0) sum += number;
        }
        return sum;
    }
}
```

## Breaking down the solution
Java is an object oriented programming language, in this example we are defining a static function called sum. It is a good approach to use **static** in this case because to run the solution there is no need to create an instance of the class Positive. The name of the variables are self explanatory and we are using a simple if statement to conditional verify if the number inside the array is positive. Also note that the for loop (used for iterative instructions) is use to go through each element in the array. 

## Try it!
Click [here](https://www.jdoodle.com/online-java-compiler/) to copy paste the code in a Java environment, just copy the code and  hit the **Execute** button on the bottom. In this Example you would be using an array of `1,-3, 6, 7, -9, 100` numbers, feel free to change the numbers and check the result.

```java
public class Positive {
    
    public static void main(String[] args) {
        int[] numbersExample = new int[]{1,-3, 6, 7, -9, 100};
        System.out.println(sum(numbersExample));
    }


    public static int sum(int[] numbers) {
        int sum = 0;
        for(int number : numbers) {
            if(number > 0) sum += number;
        }
        return sum;
    }
}
```
