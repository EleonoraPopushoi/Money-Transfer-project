Отчёт о тестировании системы пополнения счёта для VIP-клиента.

Краткое описание

18.08.2020 - 18.08.2020 было проведено 1.Functional testing приложения <название приложения>.
                                       2.Integration testing
                                       3.Sanity testing 
                                       4.Метод предроложения об ошибке.

На тестирование затрачено: 15 мин

В результате тестирования выявлены следующие дефекты:

https://github.com/EleonoraPopushoi/Money-Transfer-project/issues/1#issue-682782504

Описание процесса тестирования:

Необходимо протестировать системы пополнения счёта для VIP-клиента. Для тестирования работоспособности системы пополнения счёта для VIP-клиента.
 были применены методы :
  1. Функционального тестирования  
  2. Интеграционное тестирование и 
  3. Санитарное тестирование данной части функционала. 
  Было создано базовое приложение, в котором прописался код. В соответствии с ТЗ был предоставлены входные данные VIP-клиента (см. ниже). В ходе тестирования было проведен основной тест данного 
  функционала, и получен результат в виде нецелого отрицательного числа -1794967296 (ссылка на скриншот ниже). Данный результат образовался в следствии применения примитивного типа данных - int,
  при использовании которого произошел выход за максимальные границы данного типа. В данно случае, а именно финансовлй сфере работы необходимо использовать тип данных-float.
  Тестирование было произведено в IntelliJ IDEA с помощью кода, указанного выше и тестовых двнных.
 

 
 В процессе тестирования использовались следующие артефакты*: 

Входные данные:

текущий баланс счёта клиента - переменная типа int, значение - 2_000_000_000 (два миллиарда рублей)*
сумма перевода - переменная типа int, значение - 500_000_000 (пятьсот миллионов рублей)
переменная для хранения итогового значения - тип int

<название артефакта>

Примечание*: не указывайте артефакты "для галочки". Если вы сюда напишите тест-план, то мы попросим вас его показать (а если не покажете - то отправим работу на доработку). 
Пишите только то, что реально существует и требуется в задании.

В качестве тестовых данных использовались данные <указать источник, откуда брались тестовые данные>:

https://github.com/netology-code/javaqa-homeworks/tree/master/programming

Тестирование производилось в следующем окружении:

Windows 10.0 Домашний
Google Chrome 84.0.4147.105 (64 бит) version
IntelliJ IDEA Community