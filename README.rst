Скачиватель для webinar.ru
==========================

*Позволяет скачать запись вебинара и сохранить в виде .mp4 файла.*

Процесс скачивании автоматизирован не полность, потребуется искать
некоторые ссылки при помощи браузера.

Зависимости
-----------

Что нужно иметь для запуска приложения.

* Unix
* Python 3.6+
* ffmpeg
* requests (пакет для Питона)
* Базовые знания о работе в браузере с отладочной консолью.


Использование
-------------

1. Взять ссылку на ваш вебинар. Вида https://events.webinar.ru/event/xxx/yyy/zzz
2. Открыть в браузере.
3. Включить отладочную консоль (F12).
4. Запустить воспроизведение.
5. Отыскать ссылку с ``record-new/`` и запомнить её.
6. Отыскать ссылку, оканчивающуюся на ``chunklist.m3u8`` и запомнить её.
7. Запустить скачиватель (командой ниже) и скормить ему ссылки и двух предыдущих пунктов.

.. code-block:: bash

    $ python3 webinarru.py

Изменил
-------------
* fix некоторые кириллические имена 
* Возможность докачки
* линуксовые команды заменил на питонячьи)

