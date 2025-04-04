[Click here for English version](hosts_file_en.md)

#### Yet another small hosts file

Это [файл hosts](https://ru.wikipedia.org/wiki/Hosts) для блокировки рекламы, счетчиков, телеметрии [и всякого прочего](policy_ru.md). Генерируется из файлов [родительского проекта](../README.md) и периодически обновляется.

Применение файла hosts может быть полезно для общей блокировки рекламы в системе, а не только в браузере.

**Ограничения:**
- Возможности hosts ограничиваются только блокировкой узлов по имени
- Подстановочные символы и маски имён не поддерживаются (в первую очередь, звездочки, wildcards). См. [подробнее](https://github.com/mtxadmin/ublock/blob/master/docs/hosts_file_blokada_en.md) на английском
- Вообще ничего другого из богатого арсенала браузерных баннерорезок типа uBlock Origin не поддерживается
- Для изменения файла hosts необходимы полные права в системе. Администратор в Windows, root в Андроид, jailbreak в iOS
- При подключении через прокси-сервер файл hosts, скорее всего, не будет применяться
- При обновлении файла hosts желательно перезагрузить систему
- Приложений, обновляющих hosts, нет в официальных маркетах (например, Гугл удаляет их за блокировку рекламы). 

Тем не менее, есть и **преимущества:**
- Блокировка с применением hosts распространяется на всю систему. Баннеры и рекламные ролики в приложениях, разнообразная телеметрия и прочее
- Блокировка работает постоянно и [не требует ресурсов](hosts_file_performance_ru.md)

Таким образом, лучше всего установить **И** баннерорезку в браузер, **И** приложение, обновляющее hosts. 

Какое приложение ставить? Любое, которое умеет скачивать новые версии hosts из интернета. Конечно, намного лучше, если можно задавать сразу несколько источников для их объединения. 

### Android

Для рутованного(!) Android, например, можете посмотреть на [AdAway](https://github.com/AdAway/AdAway) - свободный, открытый, бесплатный проект. Или же любой другой по вкусу, требования, в отличие от баннерной баннерорезки, к такому приложению минимальные. Но нерутованный Android, "из коробки", не разрешит менять hosts-файл.

### Windows

~~Для Windows можно использовать программу [hostsmgr](https://github.com/henrypp/hostsmgr) (консольная), либо же скрипты Powershell с автообновлением. (Еще есть [HostsMan](http://www.abelhadigital.com/hostsman/) c GUI, но оно не работает с файлами Github [[1]](https://github.com/crazy-max/WindowsSpyBlocker/issues/103))~~

~~Также, есть упоминания о том, что Windows Defender может считать изменение HOSTS-файла с блокировкой телеметрии ошибкой/проблемой: [[1]](https://www.bleepingcomputer.com/news/microsoft/windows-10-hosts-file-blocking-telemetry-is-now-flagged-as-a-risk/), [[2]](https://windowsreport.com/windows-hosts-file-modification-bug/)~~

Update 2023: В настоящее время не рекомендуется изменять hosts-файл Windows - это может привести к полному ступору системы. См. заметку [здесь](https://github.com/mtxadmin/ublock/blob/master/docs/hosts_file_performance_ru.md). Вместо этого используйте Pi-Hole или любое другое внешнее сетевое решение.

## Резюме

Адреса файлов hosts данного проекта:

- **https://mtxadmin.github.io/hosts_pi-hole.txt** - полная версия для Pi-Hole
- **https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts.txt** - сокращенный список для Android
- **https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts_blokada.txt** - версия с wildcard-доменами. См. [подробнее](https://github.com/mtxadmin/ublock/blob/master/docs/hosts_file_blokada_en.md) на английском

Обратите внимание, что нет смысла добавлять данный файл в uBlock Origin, хотя он и понимает этот формат - используйте лучше [полную версию подписки](../README.md) для этого. 
