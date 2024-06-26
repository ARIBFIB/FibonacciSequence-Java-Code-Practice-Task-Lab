# FibonacciSequence-Java-Code-Practice-Task-Lab
![How it works (4)](https://github.com/ARIBFIB/FibonacciSequence-Java-Code-Practice-Task-Lab/assets/125716994/e3f94231-9946-4b85-a914-9883ac613661)

### YouTube Tutorial

Check out the video tutorial on [YouTube](https://youtu.be/uwlSE_TJweA) for more information.

YouTube Link : https://youtu.be/uwlSE_TJweA
# Implement a function that returns the nth number in the Fibonacci sequence using recursion. The Fibonacci sequence starts  with 0 and 1, and each subsequent number is the sum of the two preceding ones (0, 1, 1, 2, 3, 5, 8, ...). 

![image](https://github.com/ARIBFIB/FibonacciSequence-Java-Code-Practice-Task-Lab/assets/125716994/be7bfd33-cac1-4091-8878-088e95c2dc8f)
![image](https://github.com/ARIBFIB/FibonacciSequence-Java-Code-Practice-Task-Lab/assets/125716994/38621dbd-daf9-4c58-99df-8e7f79d57704)

# Sample Code 01
```
public class FibonacciSequence{
    public static long Fibonacci(int n){
//        if number of n is 0 or 1 then just return n
        if(n <= 1){
            return n;
        }else{
//         now if number is anyother number then  return add both (n-1) + (n-2)
            return Fibonacci(n-1) + Fibonacci(n-2);
        }
    }
    public static void main(String[] args) {
        System.out.println("The Fibnonacci of 10 is " +  Fibonacci(10));
    }
}
```
# Output
![image](https://github.com/ARIBFIB/FibonacciSequence-Java-Code-Practice-Task-Lab/assets/125716994/8b627acb-3bf7-4ea0-a794-d69ce8d6344c)


Sure, here's a recursive implementation of the Fibonacci sequence in Java:
# Sample Code 02
```java
public class FibonacciSequence {
    public static long fibonacci(int n) {
        if (n <= 1) {
            return n;
        } else {
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
    }

    public static void main(String[] args) {
        int n = 10;
        long result = fibonacci(n);
        System.out.println("The " + n + "th Fibonacci number is: " + result);
    }
}
```

The `fibonacci()` function takes an integer `n` as input and returns the `nth` number in the Fibonacci sequence.

Here's how the function works:

1. If `n` is 0 or 1, the function simply returns `n`, as the first two Fibonacci numbers are 0 and 1, respectively.
2. For all other values of `n`, the function recursively calls itself with `n - 1` and `n - 2` as arguments, and returns the sum of the two results.

In the `main()` function, we call the `fibonacci()` function with `n = 10`, which should print the 10th Fibonacci number, which is 55.

Here's how the call stack would look like for this example:

```
                      fibonacci(10)
                         |
                         v
                      fibonacci(9)
                         |
                         v
                      fibonacci(8)
                         |
                         v
                      fibonacci(7)
                         |
                         v
                      fibonacci(6)
                         |
                         v
                      fibonacci(5)
                         |
                         v
                      fibonacci(4)
                         |
                         v
                      fibonacci(3)
                         |
                         v
                      fibonacci(2)
                         |
                         v
                      fibonacci(1)
                         |
                         v
                         1
                         |
                         v
                      fibonacci(0)
                         |
                         v
                         0
```

The final result is calculated by adding the last two Fibonacci numbers (`34 + 21 = 55`).
Sure, here's an example of how you can use Markdown to include some icons and images in a GitHub README file:

# Fibonacci Sequence

![Fibonacci Sequence][]

## Implement a function that returns the nth number in the Fibonacci sequence using recursion.

The Fibonacci sequence starts with 0 and 1, and each subsequent number is the sum of the two preceding ones (0, 1, 1, 2, 3, 5, 8, ...).

### Sample Code 01```java
public class FibonacciSequence {
    public static long Fibonacci(int n) {
        if (n <= 1) {
            return n;
        } else {
            return Fibonacci(n - 1) + Fibonacci(n - 2);
        }
    }

    public static void main(String[] args) {
        System.out.println("The Fibonacci of 10 is " + Fibonacci(10));
    }
}```

### Output![Fibonacci Output][]



## Contributing

If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## Built With

- [Java](https://www.java.com/)

## Developer

- **[Abdul Rehman Irfan]**

## License

This project is licensed under the [MIT License](LICENSE).

In this example, I've included:

1. A main image for the Fibonacci Sequence
2. A code sample with syntax highlighting
3. An output image
4. A link to the YouTube tutorial video
5. Some standard sections for a README file, like Contributing, Built With, Authors, and License.

You can customize these elements further by using different images, icons, and formatting to suit your specific project needs.
