[README.md](https://github.com/user-attachments/files/32539783/README.md)
# Практическая работа №2 
## Выполнил студент группы П25-2.1. Кврпенко Артём Ярославович

### Блок 3.1. Арифметические операторы
---
№ 1. Вычислите результат выражения int x = 17 / 5; int y = 17 % 5;. Ответ: x = 3, y = 2.
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int x = 17 / 5;
            int y = 17 % 5;
            Console.WriteLine("x = " + x);   
            Console.WriteLine("y = " + y);
        }
    }
}
```
---
№ 2. Каково значение res после выполнения int a = 5; int res = ++a * 2;? Ответ: res = 12 (префиксный инкремент увеличивает a до 6, затем умножение)
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = 5;
            int res = ++a * 2;

            Console.WriteLine($"a = {a}");
            Console.WriteLine($"res = {res}");
        }
    }
}


```

---
№ 3.Каково значение res после выполнения int a = 5; int res = a++ * 2;? Ответ: res = 10 (постфиксный инкремент использует исходное значение 5, затем a становится 6).
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = 5;
            int res = a++ * 2;

            Console.WriteLine($"a = {a}");
            Console.WriteLine($"Результат = {res}");
        }
    }
}
```

----
№ 4. Чему равен результат 7 / 2 и 7.0 / 2? Ответ: 3 (целочисленное деление) и 3.5 (деление с плавающей точкой).

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = 7 / 2;
            double res = 7.0 / 2 ;

            Console.WriteLine($"a = {a}");
            Console.WriteLine($"Результат = {res}");
        }
    }
}
```

---
№ 5. Каков результат выражения -15 % 4 в C#? Ответ: -3 (знак остатка совпадает со знаком делимого).

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = -15 % 4;
            Console.WriteLine($"a = {a}"); 
        }
    }
}
```

---
№6. Что выведет выражение int x = 10; x = x++ + ++x;?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int x = 10;
            int b = x++ + ++x;
            Console.WriteLine($"x = { b}");
            
        }
    }
}
```

---
№7. Что произойдет при выполнении int max = int.MaxValue; int res = checked(max + 1);?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int max = int.MaxValue;
            int res = checked(max + 1);

            Console.WriteLine(res);
        }
    }
}
```

---
№8. Что произойдет при int max = int.MaxValue; int res = unchecked(max + 1);?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int max = int.MaxValue;
            int res = unchecked(max + 1);

            Console.WriteLine(res);
            
        }
    }
}
```

---
№ 9. Чему равен результат деления 1.0 / 0.0 и 0.0 / 0.0?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        { 
            double result1 = 1.0 / 0.0;
            double result2 = 0.0 / 0.0;
            Console.WriteLine(result1);
            Console.WriteLine(result2);
        }
    }
}
```

---
№ 10. Вычислите: int a = 8; int b = 3; int c = a - b * 2 + a / b;
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = 8;
            int b = 3;

            int c = a - b * 2 + a / b;
            Console.WriteLine(c);
            
        }
    }
}
```

Блок 3.2. Операторы сравнения
---
№ 11. Каков результат 5 > 3 и 5 >= 5 ? Ответ : true, true

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool first = 5 > 3; 
            bool second = 5 >= 5;

            Console.WriteLine(first); 
            Console.WriteLine(second)
            
        }
    }
}
```

---
№ 12. Чему равно "hello" == "hello" в C# и почему?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string x1 = "hello";
            string x2 = "hello";

            bool result = x1 == x2;

            Console.WriteLine(result);
            
        }
    }
}
```

---
№ 13. Чему равно выражение double.NaN == double.NaN?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double x1 = double.NaN;
            double x2 = double.NaN;

            bool result = double.NaN == double.NaN;
            Console.WriteLine(result);

        }
    }
}
```
---
№ 14. Каков результат выражения object a = new int[] { 1 };

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            object b = new int[] { 1 }; bool r = a == b;?

            object a = new int[] {1};
            object b = new int[] {1};
            bool r = a == b;

            bool result = r;
            Console.WriteLine(result);
            
        }
    }
}
```

---
№ 15. Чему равно 10 != 10.0?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool result = 10 != 10.0;
            Console.WriteLine(result);
            
        }
    }
}
```

---
№ 16. Что вернет null == null?
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(null == null);
            
        }
    }
}
```

---
№ 17. Каков результат выражения (3 < 5) == (10 >= 20)?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine((3 < 5) == (10 >= 20)); 
            
        }
    }
}
```

---
№18. Вычислите bool res = 4 <= 4 && 5 > 2;

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool res = 4 <= 4 && 5 > 2;
            Console.WriteLine(res);
        }
    }
}
```

---
№ 19. Что вернет выражение char c = 'b'; bool res = c > 'a';? 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            char c = 'b';
            bool res = c > 'a';
            Console.WriteLine(res);        
            Console.WriteLine((int)'b');   
            Console.WriteLine((int)'a'); 
            
        }
    }
}
```

---
№20. Сравните результат bool r = -0.0 == 0.0;

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(-0.0 == 0.0); 

            Console.WriteLine(1.0 / 0.0);   
            Console.WriteLine(1.0 / -0.0); 
            
        }
    }
}
```

Блок 3.3. Логические операторы
-
№ 21. Чему равен результат 5 & 3 в двоичном и десятичном виде?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(!true || false && true);
            
        }
    }
}
```

---
№ 22. Будет ли вызван метод Foo() в false && Foo()?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            
            bool Foo()
            {
                Console.WriteLine("Foo вызван!");
                return true;
            }

            bool r = false && Foo();
            Console.WriteLine(r);
            
        }
    }
}
```
---
№ 23. Будет ли вызван метод Foo() в false & Foo()? 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool Foo()
            {
                Console.WriteLine("Foo вызван!");
                return true;
            }

            bool r = false & Foo();
            Console.WriteLine(r)
        }
    }
}
```

---
№ 24. Вычислите результат: true ^ false ^ true.

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(true ^ false ^ true);
            
        }
    }
}
```

---
№ 25. Что вернет выражение !(5 > 2 || 3 < 1) ?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(!(5 > 2 || 3 < 1));
            
        }
    }
}
```

---
№ 26. Дано: bool a = true, b = false;. Чему равно a && !b || b && !a ?

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool a = true, b = false;
            bool r = a && !b || b && !a;

            Console.WriteLine(r);
        }
    }
}
```

---
№ 27. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Каков результат true || (x / 0 == 1) при любом целом x? 

            int x = 5;
            bool r = true || (x / 0 == 1);
            Console.WriteLine(r);
        }
    }
}
```

---
№ 28. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
           // Каков результат false & (10 / 0 == 1) ?

            int zero = 0;

            bool r = false & (10 / zero == 1);
            
        }
    }
}
```

---
№ 29. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Чему эквивалентно выражение !(A && B) по закону де Моргана?

            bool A = true, B = false;
            bool deMorgan1 = !(A && B);
            bool deMorgan1Equivalent = !A || !B;
            Console.WriteLine($"{deMorgan1}, {deMorgan1Equivalent}");
            
        }
    }
}
```

---
№ 30. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Чем эквивалентно выражение !(A || B)по закону де Моргана? Ответ: !A && !B.
            bool A = true, B = false;
            bool deMorgan2 = !(A || B);
            bool deMorgan2Equivalent = !A && !B;
            Console.WriteLine($"{deMorgan2}, {deMorgan2Equivalent}");
            
        }
    }
}
```

Блок 3.4
---

№ 31. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Чему равен результат 5 & 3 в двоичном и десятичном виде?

            Console.WriteLine(!true || false && true);
            
        }
    }
}
```

---
№ 32. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равен результат 5 | 3? 
            int x = 5 | 3;

            Console.WriteLine($"{x}");
            
        }
    }
}
```
---
№ 33. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равен результат 5 ^ 3?
            int x = 5 ^ 3;
            Console.WriteLine($"{x}");
        }
    }
}
```
---
№ 34. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Вычислите ~0тип int.
            int x = ~0;
            Console.WriteLine($"{x}");
            
        }
    }
}
```
---
№ 35. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно 1 << 4?
            int x = 1 << 4;
            Console.WriteLine($"{x}");
            
        }
    }
}
```
---
№ 36. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно 40 >> 2?
            int x = 40 >> 2;
            Console.WriteLine($"{x}");
            
        }
    }
}
```
---
№ 37. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Как с помощью побитовой операции проверить, установлено ли третье битовое число n(маска 2^3 = 8)?
            int n = 13;
            bool x = (n & 8) != 0;
            bool y = (n & (1 << 3)) != 0;
            if (x)
            {
                Console.WriteLine("3-й бит установлен");
            }
            else
            {
                Console.WriteLine("3-й бит не установлен");
            }
            
        }
    }
}
```
---
№ 38. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Как с помощью побитовой операции установить 2-й бит числа nв 1?
            int n = 8;
            n |= (1 << 2);
            Console.WriteLine(n);
        }
    }
}
```
---
№ 39. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //  Как бросить (установить в 0) 4-й бит числа n?
            int n = 20;
            n &= ~(1 << n);
            Console.WriteLine($"{n}");
            
        }
    }
}
```
---
№ 40. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Каковы результаты выражения (-16) >> 2для int?
            int x = (-16) >> 2;
            Console.WriteLine($"{x}");

            
        }
    }
}
```
Блок 3.5. Операторы присваивания
---
№ 41. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что делает оператор x += 5?
            int x = 10;
            x += 5;
            Console.WriteLine($"{x}");
            
        }
    }
}
```

---
№   42. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Какое значение aпосле выполнения: int a = 10; a *= 2 + 3;?
            int a = 10;
            a *= 2 + 3;
            Console.WriteLine($"{a}");
        }
    }
}
```

---
№ 43. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равен xпосле int x = 12; x >>= 2;?
            int x = 12;
            x >>= 2;
            Console.WriteLine($"{x}");
            
        }
    }
}
```

---
№ 44. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что делает оператор x ??= y?
            int? x = null;
            int y = 5;
            x = x ?? y;
            Console.WriteLine($"{x}");
        }
    }
}
```
---
№ 45. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему будет равна строка strпосле:
            string str = null;
            str = str ?? "default";
            str = str ?? "custom";
            Console.WriteLine($"{str}");
            
        }
    }
}
```
---
№ 46. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Допустимо ли выражение byte b = 1; b += 2;без явного приведения?
            byte b = 1;
            b += 2; 
            Console.WriteLine($"{b}");
            
        }
    }
}
```
---
№ 47. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно значение cпосле int a = 5, b = 10, c = 0; c = a = b;?
            int a = 5, b = 10, c = 0;
            c = a = b;
            Console.WriteLine($"{c}, {a}");
        }
    }
}
```
---
№ 48. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Какое значение maskпосле: int mask = 1; mask <<= 3; mask |= 2;?
            int mask = 1;
            mask <<= 3;
            mask |= 2;
            Console.WriteLine($"{mask}");
            
        }
    }
}
```
---
№ 49. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно xпосле int x = 15; x %= 4;?
            int x = 15;
            x % = 4;
            Console.WriteLine($"{x}");
            
        }
    }
}
```
---
№ 50. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно xпосле int x = 7; x ^= 7;?
            int x = 7;
            x ^= 7;
            Console.WriteLine($"{x}");
            
        }
    }
}
```
Блок 3.6
---
№ 51. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //  Вычислите int score = 75; string res = score >= 60 ? "Pass" : "Fail";.
            int score = 75;
            string res = score >= 60 ? "Pass" : "Fail";
            Console.WriteLine($"{res}");
            
        }
    }
}
```
№ 52. 

---

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно int x = 5; int y = (x > 10) ? 100 : (x > 2) ? 50 : 0;?
            int x = 5;
            int y = (x > 10) ? 100 : (x > 2) ? 50 : 0;
            Console.WriteLine($"{y}");
            
        }
    }
}
```
№ 53. 

---

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Какой тип имеет выражение результата true ? 10 : 15.5?
            double result = true ? 10 : 15.5;
            Console.WriteLine($"{result}");
        }
    }
}
```
---
№ 54. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вы произносите string s = null; Console.WriteLine(s?.Length);?
            string s = null; 
            Console.WriteLine(s?.Length);
        }
    }
}
```
---
№ 55. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Какой тип имеет результат выражения s?.Lengthдля string s?
            string s = null;
            int? length = s?.Length;
            Console.WriteLine($"Length = {length}");
        }
    }
}
```

---
№ 56. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Вычислите: string name = null; string res = name ?? "Anonymous";.
            string name = null;
            string res = name ?? "Anonymous";
            Console.WriteLine($"{res}");
        }
    }
}
```

---
№ 57. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Вычислите: string a = null, b = "User", c = "Admin"; string res = a ?? b ?? c;.
            string a = null, b = "User", c = "Admin";
            string res = a ?? b ?? c;
            Console.WriteLine($"{res}");
            
        }
    }
}
```

---
№ 58. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет выражение false ? (10 / 0) : 42?
            int zero = 0;
            int result = false ? (10 / zero) : 42;
            Console.WriteLine($"{result}");
        }
    }
}
```

---
№ 59. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Скомпилируется ли код var x = condition ? 10 : "text";?
            bool condition = true;
            var x = condition ? 10 : "text";

            
        }
    }
}
```

---
№ 60. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._6.Тернарный_и_null_операторы
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равно int? count = null; int res = count?.GetHashCode() ?? -1;?
            int? count = null;
            int res = count?.GetHashCode() ?? -1;
            Console.WriteLine($"{res}");  
        }
    }
}
```
---

## 3.7. Операторы типов и приведения
---
№ 61. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет выражение object obj = "Hello"; bool check = obj is string;?
            object obj = "Hello";
            bool check = obj is string;
            Console.WriteLine($"{check}");
```

---
№ 62. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет object obj = 123; string s = obj as string;?
            object obj = 123;
            string s = obj as string;
            Console.WriteLine(s ?? "null");
```
---
№ 63. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что случилось при явном приведении object obj = 123; string s = (string)obj;?
            object obj = 123;
            string s = (string)obj;
            Console.WriteLine($"{s}"); 
```
---
№ 64. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет typeof(int) == typeof(Int32)?
            bool check = typeof(int) == typeof(Int32);
            Console.WriteLine($"{check}");
```
---
№ 65. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Чему равен результат sizeof(long)в байтах?
            Console.WriteLine($"sizeof(long) = {sizeof(long)} байт");
```
---
№ 66. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет null is string?
            Console.WriteLine($"{null is string}");
```
---
№ 67. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет выражение object x = null; bool b = x is null;?
            object x = null;
            bool b = x is null;
            Console.WriteLine($"{b}");
```
---
№ 68. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Каков результат (int)3.99?
            int result = (int)3.99;
            Console.WriteLine($"{result}");
```
---
№ 69. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Каков результат сопоставления с образцом: object o = 42; if (o is int val && val > 40) { ... } Будет ли завершен блок тела?
            int res = (int)3.99;
            Console.WriteLine($"{res}");
```
---
№ 70. 
```csharp
using System;
using System.Collections.Generic;
using System.Diagnostics;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._7.Операторы_типов_и_приведения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // Что вернет выражение default(int)и default(string)?
            int i = default(int);
            string s = default(string);
            Console.WriteLine($"default(int) = {i}");
            Console.WriteLine($"default(string) = {s ?? "null"}");
```

##4. 35 сложносоставных заданий на логические выражения
---
№ 71. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //bool x = (5 > 3) && !(10 <= 2) || (4 == 5);
            //Console.WriteLine($"Задача 1: {x}");
```
---
№72. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№73. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = (10 & 6) == 2 && (10 | 6) == 14;
            Console.WriteLine($"Задача 3: {x}");
        }
    }
}
```
---
№ 74. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = (15 >> 1 == 7) && (7 << 2 == 28);
            Console.WriteLine($"Задача 4: {x}");
        }
    }
}
```
---
№ 75. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = (8 > 5) && (3 + 2 * 4 == 11) && !(false || !true);
            Console.WriteLine($"Задача 5: {x}");
        }
    }
}
```
---
№ 76. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = (true || false) && (false || true) ^ (true && !false);
            Console.WriteLine($"Задача 6: {x}");
        }
    }
}
```
---
№ 77. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = (100 / 10 == 10) && (100 % 30 == 10) && !(5 - 5 != 0);
            Console.WriteLine($"Задача 7: {x}");
        }
    }
}
```
---
№ 78. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 79. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 80. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 81. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 82. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 83. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 84. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 85. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 86. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 87. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 88. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 89. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 90. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 91. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 92. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 93. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 94. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 95. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 96. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 97. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 98. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 99. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 100. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 101. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 102. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 103. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 104. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
№ 105. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4._35_сложносоставных_заданий_на_логические_выражения
{
    internal class Program
    {
        static void Main(string[] args)
        {
            bool x = !(true && false) ^ (true || false && false);
            Console.WriteLine($"Задача 2: {x}");
        }
    }
}
```
---
