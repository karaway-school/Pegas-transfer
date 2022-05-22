# Pegas-transfer

 Учебный проект ПЕГАС ТРАНСФЕР
 Тут буду писать полезную информацию по проекту и делиться ссылками на ресурсы :)

## Подготовка страницы к разметке

Давайте дополним базовый шаблона страницы, который сгенерировали на предыдущем шаге.

1. Заголовок страницы и её краткое описание:

        <title>Пегас-трансфер: ежедневные поездки Краснодар-Пятигорск от 750 руб.</title>
        <meta name="description" content="Пегас-трансфер: Ежедневные совместные поездки из Краснодара в Пятигорск и обратно. За 5 часов. Цена от 750 рублей">

2. Добавляем фавиконку для страницы

        <link rel="icon" type="image/png" sizes="16x16" href="./favicon/favicon-16x16.png">
        <link rel="icon" type="image/png" sizes="32x32" href="./favicon/favicon-32x32.png">
        <link rel="apple-touch-icon" sizes="180x180" href="./favicon/apple-icon-180x180.png">
        <link rel="icon" type="image/png" sizes="192x192" href="./favicon/android-icon-192x192.png">
        <link rel="manifest" href="./favicon/manifest.json">

3. Дополнительные данные для корректной отрисовки страницы в браузере. Указываем стандарт кодировки текста, второй метатег удаляем, так как не вижу в нём смысла (мы не ориентируемся на древние браузеры), указываем общепринятые стандарты viewport, а так же указываем параметры файла с авторами сайта - говорим что файл есть и он лежит в корне проекта, разрешаем индексацию страницы поисковыми системами.

        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta name="author" content="humans.txt">
        <meta name="robots" content="index, follow">

4. Прописываем базовый url для относительных путей на странице, а так же параметр открытия ссылок на странице

        <base href="/" />
        <base target="_blank" />

5. Теперь давайте сгенерируем фавикон, через специальный сервис: https://www.favicon-generator.org/
Обратите внимание что мы не все варианты фавикон указываем в разметке.
Файл manifest. json содержит структурированный набор метаданных, описывающий наш проект.
Для перестраховки закидываем копию фавиконки в .ico в корень проекта.

Подготовка страницы к разметке завершена!
