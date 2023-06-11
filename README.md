# FizzBuzz(Java)

<h1 align="left">Question</h1>

###

<h3 align="left">Given an integer n, return a string array answer (1-indexed) where:<br><br>answer[i] == "FizzBuzz" if i is divisible by 3 and 5.<br>answer[i] == "Fizz" if i is divisible by 3.<br>answer[i] == "Buzz" if i is divisible by 5.<br>answer[i] == i (as a string) if none of the above conditions are true.</h3>

###

<h1 align="left">Approach:</h1>

###

<h3 align="left">The approach to solve the FizzBuzz problem is simple. We need to loop through numbers from 1 to n and check if the number is divisible by 3, 5, or both. If the number is divisible by 3, we add "Fizz" to the output list. If the number is divisible by 5, we add "Buzz" to the output list. If the number is divisible by both 3 and 5, we add "FizzBuzz" to the output list. If the number is not divisible by either 3 or 5, we add the number itself to the output list.</h3>

###

<h1 align="left">Complexity:</h1>

###

<h3 align="left">Time complexity:<br>O(n), as we need to iterate through n numbers from 1 to n.<br><br>Space complexity:<br>O(n), as we need to store n elements in the output list.</h3>

###

<h1 align="left">Code:</h1>

###

<h3 align="left">class Solution {
    public List<String> fizzBuzz(int n) {
        List<String> result = new ArrayList<>();
        
        for (int i = 1; i <= n; i++){
            if (i % 3 == 0 && i % 5 == 0) {
                result.add("FizzBuzz");
            } else if (i % 3 == 0) {
                result.add("Fizz");
            } else if (i % 5 == 0) {
                result.add("Buzz");
            } else {
                result.add(String.valueOf(i));
            }
        }
        
        return result;
    }
}</h3>

###
