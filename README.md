# Виктоина ЛНР
## Обзор
Этот проект на Unity представляет собой приложение-викторину, разработанное для выставки ВДНХ-Россия 2024, в котором пользователи отвечают на вопросы и видят правильные ответы. Если счет пользователя входит в топ-10, он может ввести свое имя и попасть в таблицу лидеров. Вопросы загружаются из JSON файла.

## Видео с демонстрацией работы на рабочем стенде
https://drive.google.com/file/d/1kKHv32x3xxq90Gdhn1wx9n7a-9tJxX3m/view?usp=sharing

## Особенности
- Два типа викторин: викторина с вопросами ВОВ и викторина "Угадай сказку"
- Отображение правильных ответов после каждого вопроса
- Таблица лидеров для топ-10 пользователей
- Загрузка вопросов из JSON файла
- !_В данной версии проекта все вопросы заменены одинаковой заглушкой_!

## Требования
- Unity 2021.3 или более поздняя версия
- Newtonsoft.Json для парсинга JSON (установить через Unity Package Manager)

## Начало работы

### Клонирование репозитория
Клонируйте этот репозиторий на свой компьютер с помощью команды:
```sh
git clone https://github.com/Ts0ym/Quiz_LNR.git
```

## Открытие в Unity
Откройте Unity Hub.
Нажмите на Открыть, найдите склонированную папку репозитория и выберите её.
Дождитесь загрузки проекта и разрешения зависимостей в Unity.

## Запуск билда на Windows без установки Unity
1. Перейдите в папку Builds
2. Запустите файл VDNH_Quiz_LNR.exe

## Использование
1. Запустите приложение на вашем устройстве.
2. Выберите между WOW Quiz и Pictures Quiz.
3. Отвечайте на вопросы, отображаемые на экране.
4. Просмотрите свой счет и узнайте, попали ли вы в таблицу лидеров.
5. Если ваш счет входит в топ-10, введите свое имя, чтобы попасть в таблицу лидеров.

## Изменение вопросов
- Вопросы для викторины "Угадай сказку" расположены в файле Assets/StreamingAssets/picturesQuestions.json
- Вопрося для викторины ВОВ расположены в файле Assets/StreamingAssets/wowQuestions.json

### Структура объектов вопросов
{
		"questionImagePath": "НазваниеИзображенияВопроса",
		"decorationImagePath": "НазваниеИзображенияДекоратораВопроса",
		"answerIndex": 0 #Номер правильного ответа
}
