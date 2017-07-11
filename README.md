# Back-in-30-Minutes
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Back_in_30_Minutes
{
    class Program
    {
        static void Main(string[] args)
        {
            int hours = int.Parse(Console.ReadLine());
            int minets = int.Parse(Console.ReadLine());

            minets += 30;

            if (minets < 60)
            {
                Console.WriteLine($"{hours}:{minets:d2}");
            }
            else 
            {
                minets -= 60;
                hours++;

                if (hours < 24)
                {
                    Console.WriteLine($"{hours}:{minets:d2}");
                }
                else
                {
                    hours -= 24;

                    Console.WriteLine($"{hours}:{minets:d2}");
                }
            }
        }
    }
}
