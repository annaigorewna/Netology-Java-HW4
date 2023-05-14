## Задание 1. Мили — модернизация

Необходимо модернизировать расчет миль по [заданию 1](https://github.com/annaigorewna/Home-work-Java-Netology/blob/1fd58c84772d512e5c3fd070d1fd27d8ffca2cb2/src/README.md) в приложении [src/FirstWork.java](https://github.com/annaigorewna/Home-work-Java-Netology/blob/1fd58c84772d512e5c3fd070d1fd27d8ffca2cb2/src/FirstWork.java) . Теперь сама логика расчёта будет находиться в специально выделенном классе сервиса, а в Main мы будем лишь создавать объект этого сервиса и вызывать его метод, передавая аргументами все необходимые данные для расчёта. Получив от вызова метода рассчитанный результат, мы выведем его на экран.

### Этапы выполнения
1. Создайте класс `BonusMilesService` (`File -> New -> Java Class`, вводите название и нажимаете `Enter`).
1. Определите в нём метод `calculate`, который:
    1. принимает на вход один параметр: `cost` типа `int`;
    1. анализируя значение переданного параметра, возвращает рассчитанное количество миль (тип — `int`).
    
Разместите следующий код в классе `Main`:

```java
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