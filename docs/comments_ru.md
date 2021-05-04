# Комментарии

Комментарии помогают понять причины блокировки. Могут быть указаны причины блокировки, либо первоначальный источник правила или хоста.

Они, по стандарту AdBlock, могут начинаться либо с **#** , либо с **!** . Иногда это просто заметки, пояснения. Помимо этого, в данном списке есть несколько исторически сложившихся правил. Разумеется, это не догма, но подобная стандартизация облегчает правки.

В случае косметических правил, поскольку по стандарту, нельзя писать в них комментарии, то комментарий располагается над строкой. "Область действия": в случае "from" и "is in", это относится только к этой строке, если не указано иное. В других случаях, часто относится ко всему блоку. Звучит немного громоздко, поэтому проще разобрать на примерах.

Здесь комментарии относятся к нижележащим строкам, каждый к своей:

reddit.com##.commentsignupbar.infobar<br>
reddit.com##.listingsignupbar.infobar<br>
**! from EasyList**<br>
reddit.com##div[id^="overlay-sidebar-atf-"]<br>
**! from EasyList**<br>
reddit.com##div[id^="overlay-sidebar-btf-"]<br>


А здесь, комментарии относятся ко всем нижележащим правилам, и являются некими разделителями в блоке правил для сайта:

**! banners in header**<br>
lamoda.ru##.header__top<br>
**! wide banners and sliders**<br>
lamoda.ru##.js-wide-slider<br>
lamoda.ru##.wide-slider<br>
lamoda.ru##.wide-slider-wrap<br>
lamoda.ru##.sport-slider-wrap<br>
**! subs banner**<br>
lamoda.ru##.subscription-footer_wrapper<br>
lamoda.ru##.ii-subscription<br>


С URL и хостовыми правилами проще - поскольку в них можно добавлять комментарии в ту же строку, то лучше так и сделать. 

Здесь комментарий относится только к этой же строке:

||cry.ru/sexclub/  &nbsp;**# from Adguard**<br>
cry.ru###header-date<br>
cry.ru###header<br>
cry.ru##noindex<br>

И здесь, аналогично:

boomerang.dell.com  # is in EasyPrivacy<br>
dell.com###contactslidertitle<br>
dell.com###okbFeedback<br>


И здесь:

||shopify.com/*/page?*&eventType=$important  &nbsp;**# from EasyPrivacy**<br>
||shopify.com/*/tricorder/$important  &nbsp;**# from EasyPrivacy: ||shopify.com/s/javascripts/tricorder/$script**<br>
||shopify.com/track.js$important  &nbsp;**# from EasyPrivacy**<br>
||shopify.com/*/shop_events_listener$important<br>
/shopify-boomerang-$important  &nbsp;**# from EasyPrivacy**<br>

Если комментариев несколько, они разделяются двумя пробелами:

networkedblogs.com$important  &nbsp;# ad scripts  &nbsp;# is in Fanboy's and Ru AdList  &nbsp;# "Website discontinued" on root

tapdaq.com$important  &nbsp;# "Ad Mediation"  &nbsp;# from MobileAdTrackers


## Стандартные пометки

В данном списке исторически сложились несколько стандартных комментариев-пометок.
<br>

Пометка "from" обозначает, что соответвующий хост или правило напрямую взяты из другого списка и не были замечены вживую.

tendertest.com  &nbsp;**# from** Peter Lowe's hosts file

gratis-toplist.de  &nbsp;**# from** MVPS

woazowup.net  &nbsp;**# from** Ru AdList
<br><br>


Пометка "is in" обозначает, что соответствующий хост был встречен "в живой природе", а также уже был замечен авторами других списков (что подтверждает достоверность). Обычно, хосты крупных сетей давно и плотно засвечены во всех списках, но постоянно появляются новые хосты и новые рекламные сети.

onvictinitor.com$important  &nbsp;# ad redirects  &nbsp;**# is in** uBlock filters and AdGuard

opentracker.net$important  &nbsp;# "Real-time analytics  TRACK VISITORS  Segmentation"  &nbsp;**# is in** hpHosts’ Ad and tracking servers

trustarc.com$important  &nbsp;# GDPR-cookies scripts  &nbsp;**# is in** EasyList and Fanboy’s

greatdexchange.com$important  &nbsp;**# is in** uBlock filters – Badware risks

s-onetag.com$important  &nbsp;# ad scripts  &nbsp;**# is in** 3 lists
<br><br>


Пометка "ad scripts" обозначает, что на некоем сайте была замечена загрузка с этого хоста сторонних скриптов. Как правило, большинство из таких скриптов являются рекламными или отслеживающими.

avantisvideo.com$important  &nbsp;**# ad scripts**  &nbsp;# is in uBlock filters

requestmetrics.com  &nbsp;**# ad scripts**  &nbsp;# is in EasyPrivacy

intergi.com$important  &nbsp;**# ad scripts**  &nbsp;# is in Malvertising filter list by Disconnect and Peter Lowe’s Ad and tracking server list



Пометка "no root" обозначает, что при попытке зайти на соответствующий хост, не было вменяемого ответа. Обычно это указывает на принадлежность хоста к рекламной или следящей сети. Исключения есть, но они очень редки.

actionbutton.co$important  &nbsp;# ad scripts and no root



Пометка "ad network" обозначает, что была встречена реклама соответствующей рекламной сети. Да, рекламщики активно рекламируют себя :-)
Это больше относится к мелким и средним сетям, крупные и так на виду.

americanclassifiedservices.com  &nbsp;# ad network
<br><br>


Пометка с именем хоста или с названием рекламной сети означает, что данный хост был замечен в связке с ними. Возможно, ложное срабатывание, но обычно нет.

grclk030.com  &nbsp;**#printrk.com**

gredinatib.biz  &nbsp;**#i-adv.biz**

offer-notavailable.com  &nbsp;**# greatdexchange.com**
<br><br>


Пометки с текстом в кавычках указывают текст цитат с соответствующего сайта. Обычно они ярко показывают причину блокировки.

1dmc.com$important  &nbsp;# tracking pixels  &nbsp;**# "Data Marketing Platform"**  &nbsp;# hermann.ai

1rash.ru$important  &nbsp;# ad scripts and banners  &nbsp;**# "контекстно-тизерная реклама"**

grattis.ru$important  &nbsp;**# "Партнерская программа по продаже аудио поздравлений"**  &nbsp;# from Adguard

retentioneering.com  # ad scripts  &nbsp;**# "why customers leave your product and reduce churn rate"**
<br><br>


Комментарии "!+ " и "! end of " являются вспомогательными техническими. Они не обрабатываются блокировщиком, и служат для упрощения развертывания поддоменов сайта.

innity.net<br>
**!+**  media.innity.net<br>
**! end of** innity<br>

eacdn.com  # adsrv.eacdn.com from Malvertising filter list by Disconnect and Peter Lowe’s Ad and tracking server list<br>
**!+**  adsrv.eacdn.com<br>
**! end of** eacdn.com<br>

