# Сервис для работы c заметками

## Инфраструктура 🛸

+ [☄️ Репозиторий](https://github.com/dan-il-g/2)
+ [📝 Документация](http://localhost:5000/docs)


# Старт проекта

## Локально (python3):

```bash
docker-compose up -d
```


# Инструменты

Всё написано на python3, работает под шустрым fastapi и простой БД SQLlite, для демонстрации работы
Нет шаблонов проектирования, но есть дробление на файлы, чтобы кусок логики стал простым и понятным
Весь контроллер находится во view.py.

Почему FASTAPI?
Потому что быстрое написание на ассинхронном фраемворке не даст заскучать серверу от притока пользователей
Работате бысрее чем Django а пишется гораздо быстрое

На всякий случай, засунул всё в докер, чтобы на вашем компьютере всё заработало хорошо и без косяков

Используется библиотека позволяющая расширить возможности роутинга, для того, чтобы выносить контроллер в 
отдельное место, как это у меня и сделано. Код не очень красивый, но рабочий,
нужно рефакторить и перенести в паттерны юзкейсов и репозитория, чтобы было всем проще менять зависимые куски проекта