Для проекта https://github.com/anestesia001/dos-29-diplomas-projects/tree/iutkov
1) Развернуть с помощью terraform и ansible инфраструктуру, состоящую из 2 машин: proxy-server, application server и бакета S3
2) Написать CI/CD пайплайны:
    - для разворачивания инфраструктуры:
        - запуск линтера для кода terraform
        - сканирование на уязвимости
        - terraform plan
        - terraform apply
    - для разворачивания приложения
        - сборка docker image
        - скан уязвимостей
        - деплой
        - проверка успешности деплоя
3) Написать скрипт для очистки старых образов и поставить его выполняться по расписанию раз в неделю на машинах jenkins и application server
 
