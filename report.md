# Отчёт о тестировании KeyValidator

## Краткое описание

28.12.2020 - 28.12.2020 было проведено функциональное тестирование и тестирование установки приложения KeyValidator. Также была протестирована документация (Инструкция по установке OpenJDK11) и соместимость KeyValidator с Java 11.

На тестирование затрачено: 3 часа

В результате тестирования выявлены следующие дефекты:
* [При вводе валидного ключа из Руководства использования KeyValidator возвращается результат FAIL](https://github.com/Budenovsky/homework-KeyValidator/issues/1#issue-775364794)
* [При вводе невалидного ключа из Руководства использования KeyValidator возвращается результат OK](https://github.com/Budenovsky/homework-KeyValidator/issues/2#issue-775367753)
* [Неверный формат ключа для проверки в Руководстве использования KeyValidator](https://github.com/Budenovsky/homework-KeyValidator/issues/3#issue-775370713)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* тест-кейс

*Примечание\*: не указывайте артефакты "для галочки". Если вы сюда напишите **тест-план**, то мы попросим вас его показать (а если не покажете - то отправим работу на доработку). Пишите только то, что реально существует и требуется в задании.*

В качестве тестовых данных использовались данные Руководства использования KeyValidator:
* Result for 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998: OK
* Result for 80b427f8-92cd-3aae-ba04-3927fbe17c6: OK
* Result for b295bc63-9f03-3b4b-af80-969b39f8c262: OK
* Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: OK
* Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: OK
* Result for 18252235-78e0-44a5-8720-556f0c7da17a: FAIL
* Result for e66075b6-ddad-445e-baf6-161b3289522b: FAIL
* Result for b6d53250-f07e-4352-a293-6102ddf7f1ca: FAIL
* Result for c2bc778a-1cb9-46c6-b435-0489649d2a42: FAIL
* Result for 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1: FAIL

Тестирование производилось в следующем окружении:
* 64-разрядная операционная система Windows 10 Домашняя
* Java 11.0.9.1
