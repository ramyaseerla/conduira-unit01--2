# conduira-unit01--2
c # program to display the characters and frequency of character from a given string in LINQ query
using System;
using System.Linq;
using System.Collections.Generic;
 
class LinqExercise5
{
    static void Main(string[] args)
    {
      string str; 

            Console.Write("\nLINQ : Displays the characters and the frequency of character from giving string : "); 
            Console.Write("\nInput the string : ");
            str= Console.ReadLine();
            Console.Write("\n");
        
            var FreQ = from x in str  
                    group x by x into y  
                    select y;  
                Console.Write("The frequency of characters are :\n");
                foreach(var ArrEle in FreQ)  
                    {  
                    Console.WriteLine("Character "+ArrEle.Key + ": " + ArrEle.Count()+" times");  
                    }  
    }
}![Screenshot (99)](https://user-images.githubusercontent.com/83413515/151586609-195686ef-4dca-4d7b-a99e-ba494706eaf3.png)
