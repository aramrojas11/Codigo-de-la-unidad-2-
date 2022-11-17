using System;
using System.Collections.Generic;
using System.Linq;
using System.Runtime.CompilerServices;
using System.Security.Cryptography;
using System.Text;
using System.Threading.Tasks;

namespace CODIFICAR

{
    static class ArrayExtensions
    {
        public static int IndexOf<t>(this t[] array, t value)
        {
            return Array.IndexOf(array, value);
        }
    }

    class program
    {
        public static int[] ConvertNumber(string frase)
        {
            char[] charFrase = frase.ToCharArray();
            int[] numbers = new int[charFrase.Length];
            for (int i = 0; i < charFrase.Length; i++)
            {
                numbers[i] = numberTo(charFrase[i]);
            }

            return numbers;
        }
        public static int numberTo(char letter)
        {
            char[] alfabeto = { ' ', 'a', 'b', 'c', 'd', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'ñ', 'o', 'p', 'q', 'r', 's', 't', 't', 'u', 'v', 'w', 'x', 'y', 'z', '.' };
            int index = alfabeto.IndexOf(letter);
            return index;
        }


        static void Main(string[] args)
        {
            Console.WriteLine("Codofica tu frase a numero presinando 1");
            Console.WriteLine("Codifica de numero a frase presiona 2");
            float op = float.Parse(Console.ReadLine());
            switch (op)
            {
                case 1:
                    Console.WriteLine("Has seleccionado codificar una frase a numero");
                    int[,] clave = { { 1, 2, 1 }, { 0, -1, 3 }, { 2, 1, 0 } };
                    Console.WriteLine("Escribe tu frase");
                    string frase = Console.ReadLine();
                    int[] numeros = ConvertNumber(frase);

                    for (int i = 0; i < numeros.Length; i++)
                    {
                        {
                            Console.WriteLine(numeros[i] + " ");
                        }
                        Console.ReadKey();
                    }
                    break;

                case 2:


                    break;
                default:
                    Console.WriteLine("Seleccion incorrecta");
                    Console.ReadKey();
                    break;



            }

        }
    }
}

-------------------------------------------------------------------------------------------------------------------------------------------------------------

using System;
using System.Collections.Generic;
using System.Linq;
using System.Runtime.CompilerServices;
using System.Security.Cryptography;
using System.Text;
using System.Threading.Tasks;

namespace ENCRIP

{
    static class ArrayExtensions
    {
        public static int IndexOf<t>(this t[] array, t value)
        {
            return Array.IndexOf(array, value);
        }
    }

    class program
    {
        public static int[] ConvertNumber(string frase)
        {
            char[] charFrase = frase.ToCharArray();
            int[] numbers = new int[charFrase.Length];
            for (int i = 0; i < charFrase.Length; i++)
            {
                numbers[i] = numberTo(charFrase[i]);
            }

            return numbers;
        }
        public static int numberTo(char letter)
        {
            char[] alfabeto = { ' ', 'a', 'b', 'c', 'd', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'ñ', 'o', 'p', 'q', 'r', 's', 't', 't', 'u', 'v', 'w', 'x', 'y', 'z', '.' };
            int index = alfabeto.IndexOf(letter);
            return index;
        }


        static void Main(string[] arg)
        {
            Console.WriteLine("Codofica tu frase a numero presinando 1");
            Console.WriteLine("Codifica de numero a frase presiona 2");
            float op = float.Parse(Console.ReadLine());
            switch (op)
            {
                case 1:
                    Console.WriteLine("Has seleccionado codificar una frase a numero");
                    int[,] clave = { { 1, 2, 1 }, { 0, -1, 3 }, { 2, 1, 0 } };
                    Console.WriteLine("Escribe tu frase");
                    string frase = Console.ReadLine();
                    int[] numeros = ConvertNumber(frase);

                    for (int i = 0; i < numeros.Length; i++)
                    {
                        {
                            Console.WriteLine(numeros[i] + " ");
                        }
                        Console.ReadKey();
                    }
                    break;

                case 2:
                    
                     static string[] numberTo(string[,] oracion)
                   {   
                    
                    char[] valorN = { '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'k', 'l', 'm', 'n', 'ñ', 'o', 'p', 'q', 'r', 's', 't', 't', 'u', 'v', 'w', 'x', 'y', 'z', '.' };
                    int index  = valorN.IndexOf(oracion);
                    return index;
                    }

            Console.WriteLine("Has seleccionado desencriptar un mensaje");
                    int[,] ints = { {-3/11, 1/11,7/11 }, {6/11, -2/11, -3/11 }, {2/11, 3/11, -1/11 } };
                    Console.WriteLine("Digita los numeros");
                    string number = Console.ReadLine();
                    int[] valorN = ConvertNumber (number);

                    for (int i = 0; i< number.Length; i++)
                    {
                        {
                            Console.WriteLine(number[i] + " ");
                        }
                        Console.ReadKey();
                    }


                    break;
                default:
                    Console.WriteLine("Seleccion incorrecta");
                    Console.ReadKey();
                    break;



            }

        }
    }
}
