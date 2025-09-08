using System;

class Program
{
    static void Main()
    {
        // --- Exercice 1 : Afficher les premiers n nombres naturels et leur somme ---
        Console.WriteLine("=== Premiers n nombres naturels et leur somme ===");
        Console.Write("Entrez une valeur pour n : ");
        int n = int.Parse(Console.ReadLine());  // Lire n au clavier

        int somme = 0;
        Console.WriteLine("Les premiers {0} nombres naturels sont :", n);
        for (int i = 1; i <= n; i++)
        {
            Console.Write(i + " ");
            somme += i;
        }
        Console.WriteLine("\nLa somme est : " + somme);

        Console.WriteLine("\n-----------------------------------------\n");

        // --- Exercice 2 : Factorielle d'un entier ---
        Console.WriteLine("=== Factorielle d'un nombre ===");
        Console.Write("Entrez un nombre entier : ");
        int nombre = int.Parse(Console.ReadLine());  // Lire le nombre au clavier

        long factorielle = 1;
        for (int i = 1; i <= nombre; i++)
        {
            factorielle *= i;
        }
        Console.WriteLine("La factorielle de " + nombre + " est : " + factorielle);
    }
}
