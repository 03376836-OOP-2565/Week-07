# การทดลองที่ 7.1

1. ให้สร้าง project เป็น console application และรันโค้ดต่อไปนี้

``` c#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Week7_Lab1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            var person1 = new Person();
            person1.Name = "Rambo";
            person1.Age = 25;
            person1.TellAge();
            person1.TellName();
        }
    }
    class Person
    { 
        // Fields
        private string name;
        private int age;

        // Properties
        public string Name
        {
            get { return name; }
            set { name = value; }
        }

        public int Age
        {
            get { return age; }
            set { age = value; }
        }

        // Methods
        public void TellAge()
        {
            Console.WriteLine($"My age is {age}");
        }
        public void TellName()
        {
            Console.WriteLine($"My name is {name}");
        }

    }
}

```


### บันทึกผล

![ภาพ](https://github.com/Sittinon-Sawatdemongkol/Week-07/assets/115066278/4262c1bd-3d7c-495f-a9c5-5a2df7bdca9c)

---

# Assignment
## 1. ให้เขียนโปรแกรมโดยใช้โปรแกรมด้านบนเป็นตัวอย่าง 

### 1.1 สร้างคลาส `Student` โดยมี members ดังต่อไปนี้


|Member type|     name   |data type|modifier | Accessor |
|:---------:|:----------:|:-------:|:-------:|:--------:|
|field      | studentID  | string  | private |          |
|field      | name       | string  | private |          |
|field      | age        | int     | private |          |
|field      | major      | string  | private |          |
|field      | university     | string  | private |          |
|field      | gpa        | float   | private |          |
|property   | StudentID  | string  | public  | getter, setter |
|property   | Name       | string  | public  | getter, setter |
|property   | Age        | int     | public  | getter, setter |
|property   | Major      | string  | public  | getter, setter |
|property   | University     | string  | public  | getter, setter |
|property   | GPA        | float   | public  | getter, setter |
|Method     | TellStudentID()     | void    | public  | |
|Method     | TellName()     | void    | public  | |
|Method     | TellAge()     | void    | public  | |
|Method     | TellMajor()     | void    | public  | |
|Method     | TellUniversity()     | void    | public  | |
|Method     | TellGPA()     | void    | public  | |


### 1.2  ทดสอบโดยเขียน Code ใน Main() ดังต่อไปนี้

```cs
static void Main(string[] args)
{
    var student1 = new Student();
    student1.Name = "ชื่อของนักศึกษาเอง";
    student1.Age = อายุ;
    // ..... เขียนให้ครบทุก properties

    // เรียกใช้งานวัตถุ
    student1.TellName();
    // ..... เรียกใช้ให้ครบทุก method
}
```

### บันทึกผล

```cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Week7_Lab1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            var student1 = new Student();
            student1.StudentID = 64030161;
            student1.Name = "Rachata Supanurak";
            student1.Age = 20;
            student1.Major = "Computer";
            student1.University = "KMITL";
            student1.GPA = 3.4;
            // ..... เขียนให้ครบทุก properties

            // เรียกใช้งานวัตถุ
            student1.TellID();
            student1.TellName();
            student1.TellAge();
            student1.TellMajor();
            student1.TellUniversity();
            student1.TellGPA();
            // ..... เรียกใช้ให้ครบทุก method
        }
    }
    class Student
    {
        // Fields
        private int studentID;
        private string name;
        private int age;
        private string major;
        private string university;
        private double gpa;

        // Properties
        public int StudentID
        {
            get { return studentID; }
            set { studentID = value; }
        }
        public string Name
        {
            get { return name; }
            set { name = value; }
        }

        public int Age
        {
            get { return age; }
            set { age = value; }
        }
        public string Major
        {
            get { return major; }
            set { major = value; }
        }
        public string University
        {
            get { return university; }
            set { university = value; }
        }
        public double GPA
        {
            get { return gpa; }
            set { gpa = value; }
        }
        // Methods
        public void TellID()
        {
            Console.WriteLine($"My Student ID is {studentID}");
        }
        public void TellName()
        {
            Console.WriteLine($"My name is {name}");
        }
        public void TellAge()
        {
            Console.WriteLine($"My age is {age}");
        }
        public void TellMajor()
        {
            Console.WriteLine($"My Major is {major}");
        }
        public void TellUniversity()
        {
            Console.WriteLine($"My University is {university}");
        }
        public void TellGPA()
        {
            Console.WriteLine($"My GPA is {gpa}");
        }
    }
}

```

![ภาพ](https://github.com/Sittinon-Sawatdemongkol/Week-07/assets/115066278/014e2e2d-4747-48c9-8157-9c801ae712ce)
