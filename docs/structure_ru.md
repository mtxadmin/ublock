# Структура

Структура списка

📁&nbsp;&nbsp;**filters** - каталог с файлами субфильтров, содержащими преимущественно косметические фильтры<br>
📁&nbsp;&nbsp;**hosts** - каталог с файлами субфильтров, содержащими преимущественно хосты<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;📁&nbsp;&nbsp;**subdomains** - технические списки поддоменов<br>

**hosts.txt** - hosts-файл. Содержит перечисление поддоменов как есть<br>
**hosts_blokada.txt** - hosts-файл для программы Blokada. Содержит умное перечисление поддоменов, и поэтому кардинально меньше обычного<br>
**it** - общий индексный файл. Содержит команды включения всех необходимых сублистов с правилами<br>
**it0** - его копия
<br><br>


Технические списки поддоменов (subdomains) не используются напрямую в блокировщике, а нужны только для автоматического формирования hosts-файла


Субфильтры с косметическими правилами (filters):

**_headers** - общие правила для нормализации заголовков, убирания логотипов и прочих общих элементов<br>
**_plugins** - список блокируемых плагинов CMS (Wordpress, Drupal, Joomla)<br>
**_removeparams** - список удаляемых из URL "мусорных" параметров, широко применяемых для отслеживания<br> 
**_sites** - общий список косметических правил, не вошедших в другие списки<br>
**_social** - список блокирования иконок соцсетей и скриптов стороннего отслеживания<br>
**_urlshorteners** - список сокращалок URL<br>
**aliexpress** - специфический список правил для Aliexpress<br>
**google** - специфический список правил для сервисов Google<br>
**microsoft** - специфический список правил для сервисов Microsoft<br>
**online_films** - список правил для русскоязычных онлайн-кинотеатров<br>
**online_films_kinopolosa** - список правил для русскоязычных онлайн-кинотеатров сети Кинополоса<br>
**stackexchange** - специфический небольшой список правил для Stackexchange (stackoverflow, serverfault, superuser ...)<br>
**yandex** - специфический список правил для сервисов Яндекса<br>

Субфильтры с хостами (hosts):

 **_all_bets_are_off** - хосты онлайн-казино, букмереров и связанных<br>
**_consultants** - хосты онлайн-консультантов, сервисов звонков и "консультантских" чат-ботов. А также пуш-уведомления<br>
**_fakenews** - хосты Fakenews, общеизвествестно доказанные, а также сильно подозрительные<br>
**_malware** - хосты с вредоносной активностью<br>
**_malware_miners** - хосты, замеченные или связанные с майнинговой активностью<br>
**_malware_scam** - мошеннические сайты<br>
**_malware_typo** - мошеннические сайты, мимикрирующие под легальные<br>
**_marketing** - общий список рекламных, отслеживающих и прочих вредоносных сайтов, не вошедших в другие списки<br>
**_marketing__subdomains** - список маркетинговых поддоменов, принадлежащих легальным сервисам<br>
**_marketing\*** - прочие маркетинговые сайты<br>
**_scam_loans** - список микрофинансовых контор (МФО) и связанных с ними сайтов<br>
**_telemetry\*** - хосты телеметрии и отслеживания. Отличие от обычных маркетологических сайтов довольно условное<br>
**_trash_closed** - закрытые сервисы и отсутствующие в DNS домены. Но иногда они возвращаются (см. zombie)<br>
**_trash_cn** - азиатскоязычные маркетологические сайты<br>
**_trash_dyndns** - поддомены DynDNS и других сервисов, замеченные в нехорошей активности<br>
**_trash_litres** - мусорные домены Литреса<br>
**_trash_random** - служебные домены рекламных сетей, сайты со случайными именами<br>
**_trash_redirects** - небольшой список сайтов-редиректов, возможно, будет преобразован<br>
**_trash_zombies** - ранее закрытые и отсутствовавшие в DNS домены, появившиеся вновь<br>
**_wap** - сайты, навязывающие платные подписки клиентам сотовых операторов и связанные с ними<br>
**_wapclick\*** - сайты, навязывающие платные подписки клиентам сотовых операторов и связанные с ними<br>


Обратите внимание, что использование отдельных субфильтров не тестировалось, не предусматривалось и не рекомендуется. Все субфильтры объединяются в общий список **it**, его адрес для использования:

**https://raw.githubusercontent.com/mtxadmin/ublock/master/it**


