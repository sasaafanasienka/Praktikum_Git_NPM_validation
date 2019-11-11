### sasaafanasienka.github.io

# Практическая работа №10
### Проект по темам Git и "командная строка"

Сссылка на работающую страницу:
https://sasaafanasienka.github.io/

Версия 0.15

_В проекте нужно было написать шаблон регулярного выражения для валидации то, что вводит пользователь.
Для этого я записал шаблон регулярного выражения в атрибут pattern каждого поля из 4 полей:_

* _Имя_
   1. только кириллица;
   2. первая буква заглавная;
   3. можно ввести от 2 до 20 символов — это можно задать в атрибутах minlength и maxlength;
   4. возможна запись двойных имён — например Анна-Мария.

* _E-mail_
   1. только латиница;
   2. «собака» @ — обязательный символ;
   3. Точка . — тоже обязательный символ.
   4. Цифры, подчерк, тире — разрешённые символы

* _Телефон_
   Шаблон для телефона должен находить номера в таких форматах:
   +7(925)900-90-90
   +7(925) 900-90-90
   +7 925-900-90-90
   +79259009090
   89259009090
   Пробелы также могут встречаться в номере
   *_В моей работе данное поле принимает также номера с кодом страны отличным от +7  
   Это потому что я из Беларуси (+375) :)_*

* _Сайт_
   Адрес сайта должен
   1. начинаться с http:// или https://;
   2. затем www. — это необязательная группа;
   3. IP-адрес — 255.255.255.255 или доменное имя — stasbasov.ru
   4. порт — тоже необязательная группа. Порт начинается с двоеточия, за которым идут от 2 до 5 цифр. Например: :8080;
   5. путь — последовательность из цифр, слешей и латинских букв, на конце которого может стоять решётка #