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


## Дополнительные настройки

После установки uBlock Origin проверьте настройки:

1. Откройте окно uBlock Origin, нажав на кнопку ![](https://user-images.githubusercontent.com/22258847/39936895-7ca7a8fc-553d-11e8-9496-45a96b623614.png).
2. Перейдите в раздел настройки ![](https://user-images.githubusercontent.com/22258847/39938114-5dc5cf00-5541-11e8-996d-5d583611f76f.png)
3. Выберите вкладку Списки 
4. Убедитесь, что на вкладке Списки включены две верхних галки и НЕ включена третья:
- Автообновление списков фильтров
- Парсить и применять косметические фильтры
- Игнорировать общие косметические фильтры

Третья галка иногда сама ставится при установке на телефоне. Нужно её отжать, иначе значительная часть правил просто не будет работать. Вот так выглядит правильный вид этих настроек:

![](https://raw.githubusercontent.com/mtxadmin/ublock/master/docs/images/ublock_settings_general_ru.png)


## Установка списка

Далее, добавляем список. Для этого, нажмите на [эту ссылку](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/mtxadmin/ublock/master/it). В предложении установки списка нажимаете Ok и всё, готово.

<details>
    <summary>
        Иногда этот метод может не работать. Пойдём длинным путём. (Нажмите на эту строку, чтобы развернуть описание)
    </summary>
    
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

Автор [дружественного проекта](https://github.com/yourduskquibbles/webannoyances/) сделал небольшую демонстрацию добавления списка. Примерно вот так выглядит процесс (c поправкой на адрес списка, конечно):

![](https://user-images.githubusercontent.com/22258847/39935902-25add6be-553a-11e8-82b0-badc73f44ed3.gif)
</details>

### Установка других списков

Как вы могли заметить в предыдущем пункте, на вкладке Списки есть много всяких списков. Это те списки, что идут к блокировщику "из коробки" - наиболее старые и известные.

Я при настройке обычно прохожусь по всем разделам и включаю максимум из них. Ну, разве что, из региональных пропускаю все, кроме RUS и CHN. Второе - это китайские списки, могут быть полезны из-за Алиэкспресса и всего такого.

Также, можно добавить следующие списки:

- AdGuard Russian filter<br>
Один из двух ведущих русскоязычных списков. До 2019 года входил в стандартную поставку uBlock Origin.
Для его установки, нажмите на [эту ссылку](https://subscribe.adblockplus.org/?location=https://filters.adtidy.org/extension/ublock/filters/1.txt).
Если не добавляется, смотрите выше, как добавить вручную. Адрес списка:
https://filters.adtidy.org/extension/ublock/filters/1.txt

- NoCoin Filter List<br>
Хороший список блокировки майнинговых скриптов. Многие перечисленные в нём сервера добавлены и в другие списки, но автор постоянно находит что-то новое. Для установки, нажмите на [эту ссылку](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt). Адрес списка:
https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt

- RU AdList: Counters<br>
Небольшой вспомогательный список в дополнение к основному русскоязычному RU AdList - авторы решили выделить счетчики и прочее отдельно. Для установки, нажмите на [эту ссылку](https://easylist-downloads.adblockplus.org/cntblock.txt). Адрес списка:
https://easylist-downloads.adblockplus.org/cntblock.txt

- RU AdList: BitBlock<br>
Тоже вспомогательный список RU AdList - убирает линеечки, мерцающие картиночки, кнопочки и прочий мусор. Для установки, нажмите на [эту ссылку](https://easylist-downloads.adblockplus.org/bitblock.txt). Адрес списка:
https://easylist-downloads.adblockplus.org/bitblock.txt

<details>
    <summary>
        А есть еще?
    </summary>
    Еще пару сотен подписок можно найти на сайте https://filterlists.com . Но многие из них, к сожалению, давно заброшены - смотрите даты последнего изменения.
</details>


## Улучшения и исправления

Что-то не работает? Чего-то не хватает? Пожалуйста, напишите об этом здесь:

https://github.com/mtxadmin/ublock/issues/new

(нужен будет аккаунт. Если у вас его еще нет, создайте, там несложно - и он ещё пригодится. GitHub - полезная штука, платформа для совместной работы над проектами)
