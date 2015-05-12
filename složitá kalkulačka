using System;
 
namespace Kalkulacka
{
    class Program
    {
        //globalne premenne
        //a nieje inicializovana a je typu cele cislo
        private static int a;
 
        //b je inicializovana a inicializacna hodnota je 0
        private static int b = 0;
 
        //hlavna metoda/funkcia ....je volana pri spusteni programu
        static void Main(string[] args)
        {
            Console.WriteLine("Zadajte rovnicu v tvare a + b");
 
            // [] nam urcuje ze ide o jednorozmerne pole a bude typu retazec
            string[] data;
 
            //trosku zlozitejsie pre zaciatocnikov...
            //Console.Readline() precita cely riadok  Split(' ') sravi to ze cely
            //retazec rozdeli na pole retazcov tak, ze retazec  rozseka v mieste
            //kde sa nachadza znak v uvodzovkach..nas pripad je medzera
            //vysledne pole ulozi do pola data
            data = (Console.ReadLine()).Split(' ');
 
            //ekvivlaent
            //string str = Console.ReadLine();
            //string[] data = str.Split(' ');
 
            //z konzoly nam vyjde text a nevie sa automaticky previest
            //na typ cislo aby sme s nim vedeli robit matematicke operacie
            //a preto ten retazec string treba previest na cislo
            //na to nam sluzi napriklas int.Parse(string arg); funkcia
            //data[cislo] -> cislo nam urcuje poziciu v poli
            a = int.Parse(data[0]);
 
            //to iste co pri a
            b = int.Parse(data[2]);
 
            //do premennej vysledok sa vlozi sucet premennej a a premennej b
            // avsak navratovy typ Metody Scitanie(int a, int b) je "int" preto
            //treba volat este metodu ToString(); ktora prevedie int na string
            string vysledok = Scitanie(a, b).ToString();
 
            //vypise vysledok na prikazovy riadok/konzolu
            Console.WriteLine("Vysledok scitania je: {0}", vysledok);
 
            //caka na stlacenie nejakej klavesy
            Console.ReadKey();
        }
 
        //nasa vlastna metoda pre scitanie
        private static int Scitanie(int a, int b)
        {
            //vrati nam sucet premennych "a" a "b"
            return a + b;
        }
    }
}
