# Отчёт о тестировании <Money Transfer>
## Краткое описание
19.07.2021 - <Дата окончания> было проведено функциональное тестирование приложения на предмет перевода денег себе на счет VIP-клиентами организации.

На тестирование затрачено: 1 час

В результате тестирования выявлен следующий дефект:

[the total balance of the VIP client's account is displayed incorrectly](https://github.com/vergizon/Hometask-2_1-Java/issues/1) .


# Описание процесса тестирования
В процессе тестирования использовались следующие артефакты*:

Чек лист: https://github.com/netology-code/javaqa-homeworks/tree/master/programming

В качестве тестовых данных использовались данные:

- текущий баланс счёта клиента - переменная initialBalance типа int, значение - 2_000_000_000 (два миллиарда рублей) ;
- сумма перевода - переменная transfer типа int, значение - 500_000_000 (пятьсот миллионов рублей);
- переменная для хранения итогового значения баланса счета VIP-клиента currentBalance - тип int ;

'''
public class Main {

    public static void main(String[] args) {
        int initialBalance = 2_000_000_000;
        int transfer = 500_000_000;
        int currentBalance = initialBalance + transfer;
        System.out.println(currentBalance);
    }
}

Тестирование производилось в следующем окружении:

версия и разрядность ОС - Windows 10 Pro x64; 
версия Java - 11.0.11;
другое ПО, при необходимости - IntelliJ IDEA version 2021.1.2