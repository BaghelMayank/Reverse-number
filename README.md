# Reverse-number
using while loop
using System;
using System.Collections.Generic;
using System.Text;

namespace smallest_number_find
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter a Two digit  number or greator :");
            int n =int.Parse(Console.ReadLine());
            int reverse = 0;
            int rem;
            while(n > 0)
            {
                rem = n % 10;
                reverse = reverse * 10 + rem;
                n = n / 10;
            }
            Console.WriteLine("Reverse number is :"+reverse);

            }
    }
}
