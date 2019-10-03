[Click here for English version](README_en.md)

<!-- [Добавить подписку](abp:subscribe?location=https%3A//raw.githubusercontent.com/mtxadmin/ublock/master/it) -->

<!-- Click the following: [Add Web Annoyances Ultralist to Custom uBlock Origin Filters](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/yourduskquibbles/webannoyances/master/ultralist.txt&title=Web%20Annoyances%20Ultralist).  -->

<!-- [Добавить подписку](ubo://subscribe?location=https%3A//raw.githubusercontent.com/mtxadmin/ublock/master/it) -->

<!-- https://github.com/github/markup/issues/933 -->

#### Yet another small uBlock filter list

Постоянно обновляемый и пополняемый список фильтров для uBlock Origin. Удаляет рекламу и следящие модули. А также убирает всякие отвлекающие [финтифлюшки](docs/policy_ru.md) с интернет-страниц. Сделаем сайты чище и просмотр удобнее!

Также есть дочерний проект - [Yet another small hosts file](docs/hosts_file_ru.md) 

## Как это работает?

### Пример сайта *ДО* установки этого списка:

![scrolling_video_newsletter_header_share_icons highlighted](https://user-images.githubusercontent.com/22258847/51348578-16f08980-1a71-11e9-80b8-0f2ad5379bcd.png)

Несмотря на то, что вы проставили все галочки в uBlock Origin (то есть, установили списки по умолчанию), вы всё равно видите какие-то раздражающие элементы. 


### Вид того же сайта *ПОСЛЕ* установки списка:

![afterinstall](https://user-images.githubusercontent.com/22258847/51348138-e8be7a00-1a6f-11e9-9b0c-5fac61a83f8f.png)


(Пример взят с дружественного проекта, вдохновившего на развитие идеи.)


## Как установить этот список?

Во-первых, если вы еще не установили [uBlock Origin](https://github.com/gorhill/uBlock) (вариант: [Nano Adblocker](https://github.com/NanoAdblocker/NanoCore)), сделайте это прямо сейчас. На сегодняшний день это лучшая баннерорезка из существующих. Подумайте об этом так: десятки крутых и квалифицированных людей по всему миру будут стараться, чтобы вы увидели как можно *меньше* рекламы. :-)

[Зачем мне вообще баннерорезка?](docs/page_example_ru.md)


#### На компьютере
- [uBlock Origin для Google Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)
- [uBlock Origin для Mozilla FireFox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)
- [Nano Adblocker для Microsoft Edge](https://www.microsoft.com/en-us/p/nano-adblocker/9nsxdx2tdb3v/)
- [uBlock Origin для Apple Safari](https://github.com/el1t/uBlock-Safari#installation)
- [uBlock Origin для Opera](https://addons.opera.com/extensions/details/ublock/)

#### На телефоне
- [uBlock Origin для Mozilla FireFox на Android](https://addons.mozilla.org/EN-US/android/addon/ublock-origin/) 

## Установка списка

После установки, нажмите на [эту ссылку](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/mtxadmin/ublock/master/it). В предложении установки списка нажимаете Ok и всё, готово.

Иногда этот метод может не работать. Пойдём длинным путём.

1. Откройте окно uBlock Origin, нажав на кнопку ![](https://user-images.githubusercontent.com/22258847/39936895-7ca7a8fc-553d-11e8-9496-45a96b623614.png).
2. Перейдите в раздел настройки ![](https://user-images.githubusercontent.com/22258847/39938114-5dc5cf00-5541-11e8-996d-5d583611f76f.png)
3. Выберите вкладку Списки 

![](https://user-images.githubusercontent.com/22258847/39937403-1da7b8b8-553f-11e8-865a-73a3f2fa4bb8.PNG). 

4. Пролистайте в самый низ и добавьте следующий адрес:

> ```
``https://raw.githubusercontent.com/mtxadmin/ublock/master/it``
> ```
5. Нажмите на появившейся кнопке "Применить" 

Я заметил, что иногда список не добавляется с первой попытки. Да, бывает, честно говоря, не знаю, с чем это связано. Попробуйте еще раз. Как вариант, можно добавить 0 в конце:
> ```

``https://raw.githubusercontent.com/mtxadmin/ublock/master/it0``

> ```


После успешной установки вы увидите надпись "Yet another small uBlock filter list". Значит, у вас получилось.

Автор [дружественного проекта](https://github.com/yourduskquibbles/webannoyances/) сделал небольшую демонстрацию добавления списка. Примерно вот так выглядит процесс:

![](https://user-images.githubusercontent.com/22258847/39935902-25add6be-553a-11e8-82b0-badc73f44ed3.gif)

Что-то не работает? Чего-то не хватает? Напишите об этом здесь:
https://github.com/mtxadmin/ublock/issues/new
