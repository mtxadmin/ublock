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

If your phone is rooted, you can also block ad hosts in [system hosts file](hosts_file_en.md), to protect your phone while rebooting and just after it, before the filtering app (Blokada or else) started.

For this hosts file version, you have to install an app which can works with asterisks in subdomains. At the moment, I know only one such app: Blokada. Update: @ignoramous recommends another filtering app: Nebulo. There are other DNS filtering apps, but they do not support asterisks.

## Blokada

Blokada is opensource and free app to filter traffic on the DNS level. I used it for several years, it is a functional and stable app (but only 4.11.1, see below).

Project resources:
- Official site: https://blokada.org
- Github: https://github.com/blokadaorg/blokada

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

## Nebulo

@ignoramous [recommends](https://github.com/mtxadmin/ublock/issues/54#issuecomment-1381255510) another filtering app: Nebulo. Free and opensource.

Project resources:
- [Nebulo](https://play.google.com/store/apps/details?id=com.frostnerd.smokescreen). Yes, you can download this app right from the Google Play Market
- [XDA developers thread](https://forum.xda-developers.com/t/app-5-0-nebulo-dns-changer-for-doh-dot-against-censorship-open-source-no-root.4156645/)
- Github: https://github.com/ch4t4r/nebulo

After install, go to the app menu -> DNS rules:
- Switch DNS rules on (at the right-top corner)
- Tap on the + button (round button at the bottom)
- Enter any name and the address of the hosts file of this project:
```
https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts_blokada.txt
```
(yes, the link is quite long, but it needs to enter it only once)
- After adding the blocklist, tap refresh button. In less than a minute counter "Rules from this source: " will change from 0 to actual number. If not, recheck link again.
- Enable query logging (Settings -> Query logging). This can be very useful to find out which domains was blocked and which was not.

Nebulo has an interesting feature: Non-VPN mode. So, you can use AND Blokada, AND Nebulo. Or AND Blokada, AND any non-filtering VPN app. This is a very promising feature.

## Other

Please note that there is no point in adding this file to uBlock Origin, although it partially understands this format - it’s better to use [full version of subscription](../README.md) for this.
