<h1>Задание 1. Мили - модернизация (обязательное к выполнению)</h1>
Вы уже научились создавать классы и методы. Поэтому вам необходимо модернизировать приложение для рассчёта миль. Теперь сама логика рассчёта будет находиться в специально выделенном классе сервиса, а в Main мы будем лишь создавать объект этого сервиса и вызывать его метод, передавая аргументами все необходимые данные для рассчёта. Получив от вызова метода рассчитанный результат, мы выведем его на экран.


<h2>Этапы выполения</h2>

1. Создайте класс `BonusMilesService` (`File` -> `New` -> `Java Class`, вводите название и нажимаете `Enter`)
2. Определите в нём метод `calculate`, который:
a)Принимает на вход один параметр: `cost` типа `int`
b)Анализируя значение переданного параметра, возвращает рассчитанное количество миль (тип - `int`)


Разместите следующий код в классе `Main`:

```css

public class Main {
    public static void main(String[] args) {
        BonusMilesService service = new BonusMilesService();
        int price = 10_000;
        int miles = service.calculate(price);
        System.out.println(miles);
    }
}
```

Убедитесь, что выводимое в консоль значение соответствует результатам предыдущей версии приложения.
