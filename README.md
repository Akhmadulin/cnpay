CFIP Connector installer

CFIP Connector installer — это инструмент для автоматической установки и настройки клиента с использованием Docker и Docker Compose.

Основные функции

Установка Docker и Docker Compose.

Генерация сертификатов.

Автоматическая установка необходимых пакетов и настройка конфигурационных файлов.

Запуск Docker с предварительно настроенными параметрами.

Установка и использование

    Запуск Docker-установки Выполните скрипт docker.sh с правами sudo или от имени root:

sudo ./docker.sh

Скрипт автоматически установит Docker и Docker Compose.

    Настройка конфигурации Откройте файл config.json и заполните следующие параметры:

{
"organization": "Название вашей организации",
"password": "Пароль для генерации сертификатов"
}

    Установка и настройка Выполните скрипт install.sh:

./install.sh

Скрипт автоматически:

Установит необходимые пакеты (unzip, telnet и curl).

Распакует файлы.

Сгенерирует сертификаты.

Заполнит конфигурационные файлы.

Запустит Docker.

Требования

Linux-сервер с поддержкой sudo или доступом к root.

Установленные зависимости:

telnet
curl
unzip
