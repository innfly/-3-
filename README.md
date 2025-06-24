# DEMO CA
Создание пользователя sshuser на серверах  Создаем самого пользователя:   useradd sshuser -u 1010  опция -u позволяет указать идентификатор пользователя сразу при создании    Задаем пароль:   passwd sshuser   Добавляем в группу wheel:   usermod -aG wheel sshuser   Добавляем строку в /etc/sudoers:   sshuser ALL=(ALL) NOPASSWD:ALL  Позволяет запуска
