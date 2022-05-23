# Подготовка страницы к разметке

Давайте дополним базовый шаблона страницы, который сгенерировали на предыдущем шаге.

1. Заголовок страницы и её краткое описание:

        <title>Пегас-трансфер: ежедневные поездки Краснодар-Пятигорск от 750 руб.</title>
        <meta name="description" content="Пегас-трансфер: Ежедневные совместные поездки из Краснодара в Пятигорск и обратно. За 5 часов. Цена от 750 рублей">

2. Добавляем favicon для страницы

        <link rel="icon" type="image/png" sizes="16x16" href="./favicon/favicon-16x16.png">
        <link rel="icon" type="image/png" sizes="32x32" href="./favicon/favicon-32x32.png">
        <link rel="apple-touch-icon" sizes="180x180" href="./favicon/apple-icon-180x180.png">
        <link rel="icon" type="image/png" sizes="192x192" href="./favicon/android-icon-192x192.png">
        <link rel="manifest" href="./favicon/manifest.json">

3. Дополнительные данные для корректной отрисовки страницы в браузере.

    - указываем стандарт кодировки текста,
    - указываем стандарты viewport и запрещаем масштабирование страницы.
    - уточняем что наша страница адаптированна под мобильные устройства (убери этот тег, если вёрстка не адаптивная).
    - запрещаем распознавание и автоматическую стилизацию адресов,телефонов
    - просим IE переключиться в последний режим
    - указываем параметры файла с данными разработчика сайта.

          <meta charset="UTF-8">
          <meta name="viewport"
              content="width=device-width, height=device-height, initial-scale=1.0, user-scalable=no, maximum-scale=1.0" />
          <meta name="HandheldFriendly" content="True" />
          <meta http-equiv="X-UA-Compatible" content="IE=edge" />
          <meta name="format-detection" content="telephone=no" />
          <meta name="format-detection" content="address=no" />
          <meta name="author" content="humans.txt">

4. Технические параметры. ОБЯЗАТЕЛЬНО удаляем перед релизом

    - запрещаем индексацию страницы поисковыми системами.
    - запрещаем кэширование страницы

          <meta http-equiv="Cache-Control" content="no-cache" />
          <meta name="robots" content="noindex, nofollow">

5. Прописываем базовый url для относительных путей на странице, а так же параметр открытия ссылок на странице (не обязательно)

        <base href="/" target="_blank">

## Теперь давайте сгенерируем фавикон, через специальный сервис

https://www.favicon-generator.org/

Обратите внимание что мы не все варианты favicon указываем в разметке.
Файл manifest.json содержит структурированный набор метаданных, описывающий наш проект.
Для перестраховки закидываем копию favicon в .ico в корень проекта.

Подготовка страницы к разметке завершена!
