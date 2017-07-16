# X
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace X
{
    class X
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());

            int h = n - 2;
            int k = 0;

            for (int i = 1; i <= (n - 1) / 2; i++)
            {
                
                Console.WriteLine("{0}x{1}x", new string(' ', k),new string(' ', h));
                h -= 2;
                k++;
            }
            Console.WriteLine("{0}x", new string(' ',n / 2));
            h += 2;
            k--;
            for (int i = 1; i <= (n - 1) / 2; i++)
            {
                Console.WriteLine("{0}x{1}x", new string(' ', k), new string(' ', h));
                h += 2;
                k--;
            }
        }
    }
}
