Скрипт **python3** для скачивания Вашей и не Вашей музыки из вконтакта.  
Тестировал на **python 3.6.9**, под **Linux Mint 19.3**.   

**Если перестало работать, пишите.**

19.05.2022 Обновление:
+ Распараллеливание скачивания.
+ Новый параметр запуска, скачать музыку с id без повторного ввода.
```bash
./src/main.py -n -i 3289301
```

08.12.2021 Обновление:
+ Скачивание музыки по **m3u8** ссылке.

18.11.2020 Обновление:
+ Обновлены зависимости библиотек
+ Параметры запуска программы, **./main.py -n** не выводит заново запрос на авторизацию (используется после успешной авторизации).

10.10.2019 Обновление:
+ Добавлено скачивание музыки из альбомов.

### Как использовать:

```bash
apt-get install ffmpeg
pip3 install -r requirements.txt
./src/main.py
```
При 1-ом запуске скрипт попросит Вас авторизоваться:
```bash
Авторизоваться заново? yes/no
> yes
```
Далее попросит ввести логин под которым мы будем авторизироваться:
```bash
Введите логин
> my_login 
```
Далее введите пароль:
```bash
Введите пароль
> 
```
Далее необходимо ввести id пользователя/группы музыку которого мы хотим скачать:
```bash
Введите id профиля
> 
```
Узнать id по имени можно например [здесь](http://regvk.com/id/)

Или:
 - войти в свой аккаунт ВКонтакте;
 - открыть меню, которое находится в правом верхнем углу, и войти в «Настройки»;
 - найти строку «Адрес страницы» и нажать на ссылку «Изменить», которая находится рядом с ней;
 - теперь в строке номер страницы вы сможете увидеть ваш ID.

Если все было сделано успешно, то Вы увидите примерно следующее:
```bash
Вы успешно авторизовались.
Подготовка к скачиванию...
Будет скачано: 113 аудиозаписей.
Скачивание началось...

1 Уже скачен: Ленинград - i_$uss.mp3.
2 Уже скачен: Chamdo - Tibetan Gorshay Dance.mp3.
...
113 аудиозаписей скачано за: 6.139557838439941 сек.

```
