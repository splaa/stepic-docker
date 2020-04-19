# stepic-docker
Управление вычислениями https://stepik.org/course/1612


Для того чтобы посмотреть список осиротевших томов, используйте команду:

docker volume ls -qf dangling=true

Для удаления таких томов:

docker volume rm $(docker volume ls -qf dangling=true)
