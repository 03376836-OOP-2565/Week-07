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
![image](https://user-images.githubusercontent.com/115066298/236549655-df16f41d-ac29-40ff-9729-7fa3796428a3.png)



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
|field      | school     | string  | private |          |
|field      | gpa        | float   | private |          |
|property   | StudentID  | string  | public  | getter, setter |
|property   | Name       | string  | public  | getter, setter |
|property   | Age        | int     | public  | getter, setter |
|property   | Major      | string  | public  | getter, setter |
|property   | School     | string  | public  | getter, setter |
|property   | GPA        | float   | public  | getter, setter |
|Method     | TellStudentID()     | void    | public  | |
|Method     | TellName()     | void    | public  | |
|Method     | TellAge()     | void    | public  | |
|Method     | TellMajor()     | void    | public  | |
|Method     | TellSchool()     | void    | public  | |
|Method     | TellGPA()     | void    | public  | |


### 1.2  ทดสอบโดยเขียน Code ใน Main() ดังต่อไปนี้

```cs
using System;

namespace ConsoleApp16
{
    internal class Program
    {
        public class Student
        {
            private string studentID;
            private string name;
            private int age;
            private string major;
            private string school;
            private float gpa;

            public string StudentID
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

            public string School
            {
                get { return school; }
                set { school = value; }
            }

            public float GPA
            {
                get { return gpa; }
                set { gpa = value; }
            }

            public void TellStudentID()
            {
                Console.WriteLine("Student ID: " + studentID);
            }

            public void TellName()
            {
                Console.WriteLine("Name: " + name);
            }

            public void TellAge()
            {
                Console.WriteLine("Age: " + age);
            }

            public void TellMajor()
            {
                Console.WriteLine("Major: " + major);
            }

            public void TellSchool()
            {
                Console.WriteLine("School: " + school);
            }

            public void TellGPA()
            {
                Console.WriteLine("GPA: " + gpa);
            }
        }
        static void Main(string[] args)
        {
            var student1 = new Student();
            student1.Name = "Siracha";
            student1.Age = 20;
            student1.StudentID = "192";
            student1.Major = "Computer";
            student1.School = "KMITL";
            student1.GPA = 4.00f;

            student1.TellName();
            student1.TellAge();
            student1.TellStudentID();
            student1.TellMajor();
            student1.TellSchool();
            student1.TellGPA();
        }

    }
}
```

### บันทึกผล
![image](https://user-images.githubusercontent.com/115066298/236550428-def52f57-4728-4504-a79f-3db09274206b.png)
