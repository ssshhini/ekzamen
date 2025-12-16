# Примеры для билетов

# Билет номер 1
# Вопрос номер 2

# Инкапсуляция
```C#
class User {
    private string password;
    public void SetPassword(string pwd) {
        password = pwd;
    }
}
# Наследование 
```C#
class Animal
{
    public string Name { get; set; }

    public void Eat()
    {
        Console.WriteLine($"{Name} ест");
    }
}
# Полиморфизм
```C#
Animal a = new Dog();
a.Sound();

# Абстракция
```C#
abstract class Shape
{
    public abstract double GetArea();
}
