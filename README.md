# Роль nginx-docker

Запускает и конфигурирует nginx в docker

Используемые модули: `docker`, `template`, `file`, `uri`

### Использование роли

Тег `install` запускает контейнер и выполняет действия тега `configure`

Тег `configure` создает конфигурационный файл, выполняет проверку и применяет конфигурацию

Тег `uninstall` останаваливает и удаляет контейнер

### Использование линтеров

Необходимые инструменты: `pipenv` и `lefthook`

Инициализация python-окружения

`pipenv update`

Установка git-хуков

`lefthook install`

Ручной запуск линтеров

`lefthook run pre-commit`