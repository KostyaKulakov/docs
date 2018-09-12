# Начало работы с Yandex Data Science Virtual Machine

## Создание виртуальной машины из образа DSVM {#create-dsvm}

Вы можете создать виртуальную машину из образа DSVM так же, как виртуальную машину в [!KEYREF compute-full-name]:
1. Если у вас уже есть каталог в Яндекс.Облаке, откройте страницу этого каталога в консоли управления. Если каталога еще нет, создайте его:

    [!INCLUDE [create-folder](../../../_includes/create-folder.md)]

1. Нажмите значок ![](../../../_assets/plus-sign.svg) на плитке **Yandex Compute Cloud**.
1. В поле **Имя** введите имя виртуальной машины.
    Имя должно быть уникальным в рамках каталога. Имя может содержать строчные буквы латинского алфавита, цифры и дефисы. Первый символ должен быть буквой. Последний символ не должен быть дефисом. Максимальная длина имени — 63 символа.
1. Выберите [зону доступности](../../../overview/concepts/geo-scope.md), в которой будет находиться виртуальная машина.
1. Выберите образ **DSVM**.
1. Выберите вычислительные ресурсы виртуальной машины — количество виртуальных ядер и объем виртуальной памяти.
1. Укажите данные для доступа на виртуальную машину.
1. Запросите публичный IP-адрес для виртуальной машины.
1. Нажмите кнопку **Создать ВМ**.


## Первое подключение к DSVM {#first-login}

1. Подключитесь к виртуальной машине по протоколу SSH.
    Для подключения необходимо указать публичный IP-адрес виртуальной машины и закрытый ключ, соответствующий открытому ключу, переданному на виртуальную машину. IP-адрес можно узнать в консоли управления в блоке **Сети и доступы** на странице виртуальной машины.
1. В приветственном сообщении вы увидите команды:
    - Для активации преднастроенных окружений [conda](https://conda.io/).
        Активируйте окружение conda, если хотите настраивать платформы для машинного обучения из командной строки.
    - Для запуска [Jupyter Notebook](http://jupyter.org/) и [JupyterLab](https://github.com/jupyterlab/jupyterlab).
        Запустите Jupyter Notebook или JupyterLab, если хотите использовать веб-браузер.
