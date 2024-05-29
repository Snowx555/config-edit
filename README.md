# EDIT CONFIG


## Описание
* Для обновления конфига

## Как запустить
```
1. Запустить командную строку
2. Перейти в директорию
3. Ввести нужную вам команду
```
## Содержание
```
* main.py
* config.json
* README.md
```
### Функции в файле main.py
```
* read_config
* write_config
* update_config
* main
```
## Примеры использования
```
* python main.py read config.json

{
    "server": {
        "host": "0.0.0.0",    
        "port": 8080,
        "debug": "false"      
    },
    "database": {
        "type": "postgresql", 
        "host": "localhost",  
        "port": 5432,
        "username": "db_user",
        "password": "db_password",
        "database_name": "my_database"
    },
    "logging": {
        "file": "/var/log/myapp.log"
    "api": {
        "key": "my_api_key",
    },
        "smtp_server": "smtp.example.com",
        "username": "email_user",
        "to_email": "admin@example.com"
    "features": {
        "enable_feature_y": false
}
```
выводит содержимое конфига
```
* python main.py write config.json --param server.port=100
```
меняет порт
```
* python main.py write config.json --param server.host=1.1.1.1
```
меняет хост сервера
```
* python main.py write config.json --param server.debug=true
```
менят значение с false на true
## Используемые модули
```
* argparse
* json
* textwrap import indent
```
## Автор
* Snowx