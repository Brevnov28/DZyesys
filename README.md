# Домашнее задание к лекции 4.«Tests»
1. Задача №1 unit-tests
Из курса «Python: программирование на каждый день и сверхбыстрое прототипирование» нужно написать тесты на любые 3 задания из Лекции 4. Необходимо использовать своё решение домашнего задания.

* При написании тестов не забывайте использовать параметризацию.

Рекомендации по тестам.

* Если у вас в функциях информация выводилась(print), то теперь её лучше возвращать(return) чтобы можно было протестировать.
2. Задача №2 Автотест API Яндекса

Проверим правильность работы Яндекс.Диск REST API. Написать тесты, проверяющий создание папки на Диске.
Используя библиотеку requests напишите unit-test на верный ответ и возможные отрицательные тесты на ответы с ошибкой

Пример положительных тестов:

* Код ответа соответствует 200.
* Результат создания папки - папка появилась в списке файлов.

## Примечания:

Для тестирования с функций и методов Яндекса не забудьте вставить свой токен в обозначенное место в файле test_pytest.

В unittest тестируется только первое задание. В pytest оба задания.
В unittest отдельно не проходит тестирование функция "test_find_country_2"
Ошибка - ERROR: not found: C:\Users\Степан Циглевкин\Desktop\Lessons work\22.11.22 Tests\Tests\test_unittest.py::TestFunc::test_find_country_2
(no name 'C:\\Users\\Степан Циглевкин\\Desktop\\Lessons work\\22.11.22 Tests\\Tests\\test_unittest.py::TestFunc::test_find_country_2' in any of [<Module test_unittest.py>])
общий запуск тестирование все тесты проходит, ошибок нет.

Также не проходит тестирование функция по чтению ключа из файла .ini. При этом функция отрабатывает, на Ядиске создаются папки. Не работает именно функция get_token.
Какая-то ошибка с ключом... и + ошибка, аналогичная вышеуказанной.