using System;

namespace diziler_array
{
    class Program
    {
        static void Main(string[]args)
        {
          //sort

          int[] sayiDizisi = {23,12,4,8,48,15};
          Console.WriteLine("****sırasız****");
          foreach (var sayi in sayiDizisi)
          {
              Console.WriteLine(sayi);
          }
          Console.WriteLine("****sıralı****");
          Array.Sort(sayiDizisi);

          foreach (var sayi in sayiDizisi)
           Console.WriteLine(sayi);

           //clear
           //sayiDizisi elamanlarını kullanarak 2. index ten itibaren 2 tane elemanı 0 lar.

           Array.Clear(sayiDizisi,2,2);

           foreach (var sayi in sayiDizisi)
           {
               Console.WriteLine(sayi);

           }

           //reverse

         Console.WriteLine("****reverse****");
          Array.Reverse(sayiDizisi);

          foreach (var sayi in sayiDizisi)
           Console.WriteLine(sayi);

           //indexof

         Console.WriteLine("****indexof****");
         Console.WriteLine(Array.IndexOf(sayiDizisi,23));

         //resize
         Console.WriteLine("****resize****");
         Array.Resize<int>(ref sayiDizisi,7);
         sayiDizisi[6] = 81;

         foreach (var sayi in sayiDizisi)
         {
             Console.WriteLine(sayi);
             
         }




    
        }

    }   
}



