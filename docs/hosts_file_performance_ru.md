[Click here for English version](hosts_file_performance_en.md)

В сети встречаются мнения, что при большом [файле hosts](hosts_file_ru.md) система может подтормаживать. Так ли это?

### Android:
Я использую огромные файлы hosts с 2012 года, и ни на одном доступном устройстве - а они тогда были маленькие и слабые - не замечал проблем с производительностью. Теоретически, некоторый эффект может наличествовать, но практически ускорение от блокировки рекламных и прочих паразитных запросов намного перекрывает этот эффект, даже если он есть.

Автор hosts-файла MoaAB [подтверждает это](https://forum.xda-developers.com/showthread.php?t=1916098), хотя [замечает](https://forum.xda-developers.com/showpost.php?p=62564889&postcount=3313), что использование большого (7-8 МБ) hosts-файла вызывает потребление 30-50 МБ оперативной памяти, что является очень небольшой частью нагрузки системы:

> ``>>>`` Performance Issue? Will my device run SLOW?<br>
> I am using this 'hosts' file from my chilhood days and never had any performance issue to date, Although you might have a little delay in startup for few seconds (but you will not even notice) and then everything will be cool in standby and active mode. I say "Little delay is better than ADs, Malwares and Spywares..."

> Minimum RAM requirment is only 512MB to 1GB. MoaAB only consumes 30-50MB in general and dont kill the device in any way. ... In practial MoaAB is just small fraction of system load

Также он упоминает, что в Android 5.0 были ошибки утечки памяти. Более ранние и поздние версии не подвержены этой ошибке.


### Windows: 
На Windows 7 (и старше) в некоторых случаях, действительно, могут отмечаться подтормаживания. На Windows 10 Microsoft, наконец-то, внесла изменения и эта проблема уже неактуальна. Подробнее смотрите у автора файла hosts с 20-летней (!) историей: http://winhelp2002.mvps.org/hosts.htm 

Стоит отметить, что Windows 7 уже снята с поддержки и не получает обновлений. Если вы используете эту версию, или даже старше, можно попробовать отключить службу DNS Client (подробности по ссылке выше). Но лучше всё же перейти на актуальную версию.

#### Update 2023:

Сейчас на системах Windows стандартный майкрософтовский антивирус активно протестует против изменения файла hosts. В случае небольшого файла он просто выдает «вирусоподобное» уведомление и предлагает пользователю выполнить откат файла хостов до значения по умолчанию. В случае относительно большого файла он может конфликтовать с сетевыми службами и, таким образом, сделать систему непригодной для использования.

Поэтому не изменяйте непосредственно файл хостов в системе Windows. Майкрософт хочет, чтобы их телеметрия была запущена и работала. Но можно использовать промежуточный инструмент, такой как Pi-hole, внешний DNS или какое-то другое решение.
