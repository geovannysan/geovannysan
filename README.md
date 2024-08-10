## Hola 👍
```bash
using System;
using System.Collections.Generic;

namespace MyPortfolio
{
    public class SoftwareDeveloper
    {
        public string Name { get; set; }
        public string Title { get; set; }
        public string Location { get; set; }

        public SoftwareDeveloper()
        {
            Name = "Geovanny Chávez Pallaroso";
            Title = "Ing. Computación e informática";
            Location = "Ecuador, Guyaquil";
        }
    }

    public class Skills : SoftwareDeveloper
    {
        public List<string> Languages { get; set; }
        public List<string> Databases { get; set; }
        public List<string> Frameworks { get; set; }

        public Skills()
        {
            Languages = new List<string> { "JavaScript""C#",, "TypeScript", "PHP",  "..." }; 
            Databases = new List<string> { "MySQL", "MongoDB", "PostgreSQL", "SQL Server" };
            Frameworks = new List<string> { "Node js","React", "Ionic", "ASP.NET Core","Android","JQuery","...." } ;
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            SoftwareDeveloper bio = new SoftwareDeveloper();
            Skills skills = new Skills();

            Console.WriteLine("Name: " + bio.Name);
            Console.WriteLine("Title: " + bio.Title);
            Console.WriteLine("Location: " + bio.Location);
            Console.WriteLine();
            Console.WriteLine("Languages: " + string.Join(", ", skills.Languages));
            Console.WriteLine("Databases: " + string.Join(", ", skills.Databases));
            Console.WriteLine("Frameworks: " + string.Join(", ", skills.Frameworks));
        }
    }
}
```
