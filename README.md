# Go Proto Module
## Описание
Этот модуль предоставляет протокол для взаимодействия с сервисом аутентификации, сгенерированный для языка Golang в репозитории [proto-definitions](https://github.com/sandrinasava/proto-definitions). Модуль используется в проекте [cafe-services](https://github.com/sandrinasava/cafe-services) для общения между сервисом обработки заказов и сервисом аутентификации.

## Мотивы вынесения .proto-файла и сгенерированного кода из [cafe-services](https://github.com/your-username/cafe-services):

- ### Упрощение управления зависимостями:
   В микросервисах достаточно указать зависимость на go-proto-module, вместо того, чтобы хранить .proto-файлы и генерировать код непосредственно в каждом микросервисе.

- ### Упрощенная актуализация контракта:
   Достаточно изменить .proto в proto-definitions и обновить зависимости в проекте.
   В свою очередь Workflow в proto-definitions обновит информацию в go-proto-module.

