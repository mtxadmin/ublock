<!-- [Нажмите сюда для русской версии](hosts_file_blokada_ru.md) -->

#### Yet another smart Blokada hosts file

This is the [hosts file](https://en.wikipedia.org/wiki/Hosts_(file)) for blocking ads, counters, telemetry and [other things](policy_en.md). It is generated from the files of [the parent project](../README_en.md) and is periodically updated.

Applying of the hosts file can be useful for general ad blocking in the system, not just in the browser.

Wildcard characters are SUPPORTED in this (Blokada) version! You can block a domain and all its subdomains by mask. This means compact list and effective ad blocking.

**Restrictions:**
- The capabilities of the hosts file are limited only by blocking nodes by name (and mask in this version)
- In general, nothing else from the rich arsenal of browser-type banner cutters like uBlock Origin is supported
- Standard operation systems cannot use this version. Nor Windows, nor Android, nor Linux. You have to install an app which could use this format.

However, there are **advantages:**
- Blocking with the use of hosts applies to the entire system. Banners and commercials in applications, various telemetry and other
- Blocking works continuously and [almost does not require resources](hosts_file_performance_en.md) (Upd 2023: on Windows systems now Microsoft Antivirus actively protests against hosts file changing and even may freeze the system. Microsoft wants their telemetry up and running)

Thus, it is best to install **AND** an ad blocker in the browser, **AND** an application that updates the hosts.

If your phone is rooted, you can also block ad hosts in [system hosts file](hosts_file_en.md), to protect your phone while rebooting and just after it, before Blokada started.


For this hosts file version, you have to install an app which can works with asterisks in names. At the moment, I know only one such app: [Blokada](https://blokada.org). It is opensource and free.

Attention:
- Blokada is absent in markets, because of its adblocking nature. There is Blokada Slim reduced version in Play Market, but it has very limited functions. Use blokada.org
- There are two versions of Blokada: v4 and v5. Fifth CANNOT add custom lists, use fourth
- In newest versions of Blokada v4 there is [a bug](https://github.com/blokadaorg/blokada/issues/900) which leads to miss some ad requests. Last known good version:

https://github.com/blokadaorg/blokada/releases/download/4.11.1/blokada-v4.11.1.apk

The address of the hosts file of this project:
```
https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts_blokada.txt
```

After adding this new host list, go to *Ad blocking Sessions* and set options:
- Advanced adblocking rules: Yes
- Smart List: No
- CName-Blocking: Yes

Please note that there is no point in adding this file to uBlock Origin, although it partially understands this format - it’s better to use [full version of subscription](../README.md) for this.
