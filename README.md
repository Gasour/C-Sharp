using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace Znamky
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Spočítám ti průměr známek. Kolik známek zadáš?");
            int pocet = int.Parse(Console.ReadLine());
            int[] cisla = new int[pocet];
            for (int i = 0; i < pocet; i++)
            {
                Console.Write("Zadejte {0}. číslo: ", i + 1);

                if (cisla>5)
                {
                    Console.WriteLine("Zadávejte čísla jen od 1 do 5");
                    i--;
                }
                else
                {

                    cisla[i] = int.Parse(Console.ReadLine());   
                }

                
            }
            Console.WriteLine("Průměr tvých známek je: {0}", cisla.Average());
            Console.ReadKey();
        }
    }
}
