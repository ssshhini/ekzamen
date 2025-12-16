# Примеры для билетов

# Билет номер 1
# Вопрос номер 2

# Инкапсуляция
class User {
    private string password;
    public void SetPassword(string pwd) {
        password = pwd;
    }
}
# Наследование 

class Animal
{
    public string Name { get; set; }

    public void Eat()
    {
        Console.WriteLine($"{Name} ест");
    }
}
# Полиморфизм
Animal a = new Dog();
a.Sound();

# Абстракция

abstract class Shape
{
    public abstract double GetArea();
}
