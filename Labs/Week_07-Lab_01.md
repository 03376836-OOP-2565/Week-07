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

![ภาพ](https://user-images.githubusercontent.com/112167732/232374150-e1ef9e7d-6e97-43ce-979c-8bcce4cbce51.png)


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
![ภาพ](https://user-images.githubusercontent.com/112167732/232376567-d7b7b706-efc9-4ff0-a824-ac5457523788.png)
![ภาพ](https://user-images.githubusercontent.com/112167732/232376649-18fe2f1f-bc71-45ba-b355-37de3a5769cb.png)
![ภาพ](https://user-images.githubusercontent.com/112167732/232376707-f3a3b5ad-f375-4ef5-8d02-761102b0e0bd.png)
![ภาพ](https://user-images.githubusercontent.com/112167732/232376738-56e4f5d3-29d3-49ee-8863-ca7a3010b173.png)
![ภาพ](https://user-images.githubusercontent.com/112167732/232376760-27d3ceed-9285-49e9-9957-95c8db9ad1a7.png)
