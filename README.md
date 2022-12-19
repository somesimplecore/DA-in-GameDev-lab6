# Интеграция рекламных сервисов в интерактивное приложение
Отчет по лабораторной работе #6 выполнил(а):
- Паханов Александр Александрович
- РИ-300018

Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Cоздание интерактивного приложения с рейтинговой системой пользователя и интеграция игровых сервисов в готовое приложение.

## Задание 1
### Используя видео-материалы практических работ 1-5 повторить реализацию функционала.
### Ход работы:

- Практическая работа «Интеграция баннерной рекламы»

Для того, чтобы в нашей игре на Яндекс играх показывалась баннерная реклама, создадим RTB-блок для нашей игры. Сгенерированное название запишем в поле Banner static 1 в Player settings:

![](/Pics/z1_1.jpg)

Далее выставим следующие настройки у скрипта Info YG:

![](/Pics/z1_1.jpg)

Теперь у нас будет показываться баннерная реклама при игре на площадке.

- Практическая работа «Интеграция видеорекламы»

Напишем следующий код после смерти и во время проверки SDK:

```C#
YandexGame.RewVideoShow(0);
```

Теперь у нас будет показываться видеореклама после действий, описанных выше.

- Практическая работа «Показ видеорекламы пользователю за вознаграждение»




## Задание 2
### Описать не менее трех дополнительных функций Яндекс SDK, которые могут быть интегрированы в игру.
### Ход Работы:

- YandexGame.playerPhoto
С помощью данного метода можно получить фото пользователя. Эту картинку потом можно применять как угодно. К примеру, можно ее привязать к игровому персонажу или по другому внедрить в игровой процесс.

- YandexGame.RewVideoShow()
Через вызов этого метода можно показывать рекламу за вознаграждение. За просмотр рекламы можно давать дополнительные ресурсы, уникальное оружие или интересные скины.

- YandexGame.PromptShow()
Этот метод вызывает диалоговое окно, в котором будет предложено установить ярлык. Данная функция может увеличить посещение игры пользователями, т.к. будет легче и быстрее открыть игру.

## Задание 3
### Доработать стилистическое оформление списка лидеров и системы достижений, реализованных в задании 1.
### Ход работы:

Чтобы текст достижений было лучше видно, добавим подложку за надписи. Также добавим заголовок, иконки и разделитель. Достижения пронумеруем, чтобы игроку было легче разграничить и воспринимать достижения.  В итоге получаем следующий вид системы, который намного приятнее глазу:

![](/Pics/z3_1.jpg)

Список лидеров на платформе Яндекс Игры не имеет инструментов для редактирования его визуальной составляющей, поэтому доработать стилистическое оформление не представляется возможным

## Выводы

Мы удачно добавили множество функций YandexSDK, которые улучшат игровой опыт пользователя. Яндекс дает доступ к информации аккаунта пользователя, которую мы можем использовать в своей игре. Также есть возможность сохранения прогресса игрока на серверах Яндекс, что говорит о том, что нам не обязательно иметь собственный сервер для хранения данных. Вдобавок были добавлены таблица лидеров и система достижений. SDK от Яндекс имеет еще множество функций, которые можно использовать для удержания игрока, монетизации и развития геймплея. Также было доработано стилистическое оформление системы достижений.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
