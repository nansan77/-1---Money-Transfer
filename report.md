Отчёт о тестировании 

 Приложения Money Transfer

* Было создано базовое приложение «Money Transfer» в IntelliJ IDEA с переменной типа int и протестировано цифрами входящие в границы переменной типа int. 

 * При суммировании двух чисел произошёл выход за границу типа int.
 int Целочисленный ТИП граница до 2 147 483 647

* При тестировании с переменной типа Long результат стал положительным.
Long Целочисленный ТИП граница до 9 223 372 036 854 775 807

Описание тестов 

     * Были проведены Два негативных и нефункциональных теста:
1 тест: прибавления двух переменных типа int, с итогом суммы переменной типа int, С выходом за границу типа int. (негативное тестирование типа int+ типа int= типа int за границу типа int), (нефункциональное тестирование оператор (+) не работает )

2 тест: прибавления двух переменных типа int, с итогом суммы переменной типа Long (негативное тестирование типа int+ типа int= типа Long), (нефункциональное тестирование оператор (+) не работает)

       * Был проведен один позитивный и функциональный тест:

 1 тест: прибавления двух переменных типа Long, с итогом суммы переменной типа Long
(позитивное тестирование типа Long + типа Long = типа Long), (функциональное тестирование оператор (+) работает)

 Результаты

* 33,33% Успешных тестов
* 66,66% не успешных тестов

* [Баг репорт: Приложение Денежный Перевод (Money Transfer) при пополнении счёта, не верно сложил два числа 2_000_000_000 + 500_000_000 #1](https://github.com/nansan77/-1---Money-Transfer/issues/1)

* [Баг репорт: Приложение Денежный Перевод (Money Transfer) при пополнении счёта, не верно сложил два числа 2_000_000_000 + 500_000_000 #2](https://github.com/nansan77/-1---Money-Transfer/issues/2)

Общие рекомендации

Заменить переменная типа int на переменную типа Long
