## Комментарии

Комментарии помогают понять причины блокировки. Могут быть указаны причины блокировки, либо первоначальный источник правила или хоста.
<br><br>

Пометка "from" обозначает, что соответвующий хост или правило напрямую взяты из другого списка и не были замечены вживую.

tendertest.com  &nbsp;**# from** Peter Lowe's hosts file

gratis-toplist.de  &nbsp;**# from** MVPS

woazowup.net  &nbsp;**# from** Ru AdList
<br><br>


Пометка "is in" обозначает, что соответствующий хост был встречен "в живой природе", а также уже был замечен авторами других списков (что подтверждает достоверность)

onvictinitor.com$important  &nbsp;# ad redirects  # is in uBlock filters and AdGuard

opentracker.net$important  &nbsp;# "Real-time analytics  TRACK VISITORS  Segmentation"  &nbsp;# is in hpHosts’ Ad and tracking servers

trustarc.com$important  &nbsp;# GDPR-cookies scripts  # is in EasyList and Fanboy’s

greatdexchange.com$important  &nbsp;# is in uBlock filters – Badware risks

s-onetag.com$important  &nbsp;# ad scripts  # is in 3 lists
<br><br>


Пометка "ad scripts" обозначает, что на некоем сайте была замечена загрузка с этого хоста сторонних скриптов. Как правило, большинство из таких скриптов являются рекламными или отслеживающими.

avantisvideo.com$important&nbsp;&nbsp;# ad scripts  # is in uBlock filters

requestmetrics.com  # ad scripts  # is in EasyPrivacy

intergi.com$important  # ad scripts  # is in Malvertising filter list by Disconnect and Peter Lowe’s Ad and tracking server list



Пометка "no root" обозначает, что при попытке зайти на соответствующий хост, не было вменяемого ответа. Обычно это указывает на принадлежность хоста к рекламной или следящей сети. Исключения есть, но они очень редки.

actionbutton.co$important  &nbsp;# ad scripts and no root



Пометка "ad network" обозначает, что была встречена реклама соответствующей рекламной сети. Да, рекламщики активно рекламируют себя :-)
Это больше относится к мелким и средним сетям, крупные и так на виду.

americanclassifiedservices.com  &nbsp;# ad network
<br><br>


Пометка с именем хоста или с названием рекламной сети означает, что данный хост был замечен в связке с ними. Возможно, ложное срабатывание, но обычно нет.

grclk030.com  &nbsp;#printrk.com

gredinatib.biz  &nbsp;#i-adv.biz

offer-notavailable.com  &nbsp;# greatdexchange.com
<br><br>


Пометки с текстом в кавычках указывают текст цитат с соответствующего сайта. Обычно они ярко показывают причину блокировки.

1dmc.com$important  # tracking pixels  # "Data Marketing Platform"  # hermann.ai

1rash.ru$important  # ad scripts and banners  # "контекстно-тизерная реклама"

grattis.ru$important  # "Партнерская программа по продаже аудио поздравлений"  # from Adguard

retentioneering.com  # ad scripts  # "why customers leave your product and reduce churn rate"
<br><br>


Комментарии "!+ " и "! end of " являются вспомогательными техническими. Они не обрабатываются блокировщиком, и служат для упрощения развертывания поддоменов сайта.

innity.net
!+  media.innity.net
! end of innity

eacdn.com  # adsrv.eacdn.com from Malvertising filter list by Disconnect and Peter Lowe’s Ad and tracking server list

!+  adsrv.eacdn.com

! end of eacdn.com


Еще одно техническое замечание - в данном списке комментарии разделяются двумя пробелами.

