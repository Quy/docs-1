PayMaster
---------

Описание
========

Онлайн способ оплаты (агрегатор платежей).

Официальный сайт: |link|

.. |link| raw:: html

   <!--noindex--><a href="http://info.paymaster.ru/" target="_blank" rel="nofollow">PayMaster</a><!--/noindex-->


Подключите PayMaster, чтобы принимать платежи на вашем сайте множеством способов.

Один договор включает множество способов оплаты на Вашем сайте: банковские карты,
интернет-банкинг, терминалы, электронные платежные системы, денежные переводы и другие.

Инструкция
==========

1.  Зарегистрируйте интернет-магазин в системе PayMaster.

    На сайте "Paymaster" необходимо установить следующие настройки на странице "Детали сайта":

    *   Разделел "Обратные вызовы": 

        -   Payment notification - POST запрос, 
        -   Success redirect - GET запрос, 
        -   Failure redirect - GET запрос, 
        -   Invoice confirmation - GET запрос 
        -   Отметить настройку "Разрешена замена URL" . 

    *   Раздел "Технические параметры"

        -   Введите секретный ключ, этот ключ необходимо будет ввести в поле "Секретный ключ" настроек способа оплаты.
        -   Тип шифрования: MD5


2.  Создайте новый способ оплаты (:doc:`Инструкция </manager/payments/index>`)

3.  Выберите процессор оплаты "Paymaster" в окне редактирования способа оплаты.

    .. fancybox:: img/payments_034.png
        :alt: PayMaster

4.  Пройдите во вкладку "Настроить" нового способа оплаты и выполните настройку.

    .. fancybox:: img/payments_035.png
        :alt: PayMaster

    Доступные настройки:

    .. list-table::
        :header-rows: 1
        :stub-columns: 1
        :widths: 10 30

        *   -   Настройка
            -   Описание

        *   -   ID аккаунта
            -   Доступен в личном кабинете PayMaster

        *   -   Секретный ключ
            -   Настраивается в личном кабинете PayMaster

        *   -   Выберите способ оплаты
            -   Вы можете выбрать способ оплаты по-умолчанию. 

                Вы можете создавать несколько способов оплаты с разными настройками, используя процессор PayMaster. Покупатель сможет сделать предварительный выбор на странице оформления заказа интернет-магазина.

                Оставьте значение "Выбор на PayMaster", чтобы покупатель выбрал удобный ему способ оплаты на сайте PayMaster.

5.  Проверьте работу создав тестовый заказ.

