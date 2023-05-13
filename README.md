# Recursive-function

## Aim: To write a C# program to reverse a number using recursive function.

## Algorithm:
1. initialise the program 
2. using static keyword in public key to declare the function 

## Program:
~~~ C#
using System;

class Program
{
    static int reverse(int num, int rev)
    {
        if (num == 0)
        {
            return rev;
        }
        else
        {
            rev = rev * 10 + num % 10;
            return reverse(num / 10, rev);
        }
    }
    static void Main(string[] args)
    {
        int num, rev = 0;
        Console.Write("Enter a number: ");
        num = int.Parse(Console.ReadLine());

        rev = reverse(num, rev);
        Console.WriteLine("Reverse of {0} is {1}", num, rev);
    }
}
~~~

## Output:
![Screenshot 2023-05-13 091408](https://github.com/shankar-saradha/Recursive-function/assets/93978702/df671405-4c44-4958-bc7b-c5641ec29ed5)

## Result:
