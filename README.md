# Примеры для билетов

# Билет 1 вопрос 2
```C#
Инкапсуляция

class User {
    private string password;
    public void SetPassword(string pwd) {
        password = pwd;
    }
}
```
Наследование 
```C#
class Animal
{
    public string Name { get; set; }

    public void Eat()
    {
        Console.WriteLine($"{Name} ест");
    }
}
```
Полиморфизм
```C#
Animal a = new Dog();
a.Sound();
```
Абстракция
```C#
abstract class Shape
{
    public abstract double GetArea();
}
```
#Билет 2 вопрос 1
```C#
class Logger {
    private static Logger instance;
    private Logger(){}
    public static Logger GetInstance() {
        return instance ??= new Logger();
    }
}
```

#Билет 2 вопрос 3

Исключения 
```C#
try {
    int x = int.Parse("abc");
} catch (FormatException e) {
    Console.WriteLine("Ошибка формата");
} finally {
    Console.WriteLine("Завершено");
}
```

#Билет 4 вопрос 3
```C#
lock(obj) {
    counter++;
}
```

#Билет 6 вопрос 2
```C#
class User {
    public int Id { get; set; }
    public string Name { get; set; }
}
```

#Билет 8 вопрос 2
```C#
class OrderService {
    private readonly IRepository repo;
    public OrderService(IRepository repo) {
        this.repo = repo;
    }
}
```

#Билет 9 вопрос 1
```C#
async Task LoadData() {
    var data = await httpClient.GetStringAsync(url);
}
```

#Билет 9 вопрос 2
```C#
lock(obj) {
    counter++;
}
```

#Билет 9 вопрос 3
```C#
Task.Run(() => DoWork());
Parallel.For(0, 10, i => Process(i));
```

#Билет 10 вопрос 2
```C#
try {
    Save();
} catch (IOException ex) {
    logger.LogError(ex.Message);
}
```

#Билет 13 вопрос 2
```C#
Type t = typeof(User);
var methods = t.GetMethods();
```
#Билет 14 вопрос 2
```C#
JsonSerializer.Serialize(obj);
```

#Билет 16 вопрос 2
```C#
numbers.AsParallel().Sum();
```
#Билет 17 вопрос 1

```SQL

SELECT * FROM Orders
JOIN Users ON Orders.UserId = Users.Id;
```

#Билет 23 вопрос 2
```C#

try {
    await SomeAsyncMethod();
} catch(Exception ex) {
    Console.WriteLine(ex.Message);
}
```
