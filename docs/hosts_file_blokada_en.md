﻿<!-- [Нажмите сюда для русской версии](hosts_file_blokada_ru.md) -->

#### Yet another smart Blokada hosts file

The name says "Blokada", but it is pretty compartible for any app which supports asterisks (wildcards) in hosts.

This is the [hosts file](https://en.wikipedia.org/wiki/Hosts_(file)) for blocking ads, counters, telemetry and [other things](policy_en.md). It is generated from the files of [the parent project](../README_en.md) and is periodically updated.

Applying of the hosts file can be useful for general ad blocking in the system, not just in the browser.

Wildcard characters are [SUPPORTED](https://community.blokada.org/t/wildcard-support-in-blokada/11659) in this (Blokada) version! You can block a domain and all its subdomains by mask. This means compact list and effective ad blocking.

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

## Blokada (deprecated)

Update: in later versions of Blokada there are no possibility to add custom lists. And the authors removed old working versions from Github. So this app is useless now.

Blokada is opensource and free app to filter traffic on the DNS level. I used it for several years, it is a functional and stable app (but only 4.11.1, see below).

Project resources:
- Official site: https://blokada.org
- Github: https://github.com/blokadaorg/blokada

Attention:
- Blokada is absent in markets, because of its adblocking nature. There is Blokada Slim reduced version in Play Market, but it has very limited functions. Use blokada.org
- There are two versions of Blokada: v4 and v5. Fifth CANNOT add custom lists, use fourth
- In newest versions of Blokada v4 there is [a bug](https://github.com/blokadaorg/blokada/issues/900) which leads to miss some ad requests. Last known good version:

<strike>https://github.com/blokadaorg/blokada/releases/download/4.11.1/blokada-v4.11.1.apk</strike>

Update: The authors removed this working version from Github. Options:
- To download latest v4 from https://github.com/blokadaorg/blokada/releases/tag/archive - latest v4 version there is from 2023-02, so-called blokada4-final.apk (4.15.0 in fact), and it's NOT working properly, bypassing most of the ads
- To download from Russian site [4pda](https://4pda.to/forum/index.php?showtopic=828196) (downloading there needs registration, or you will see 404 errors) - but v4 branch there has only 4.8.3 release
- To search app's apk on third-party sites. I don't really trust them, but... It can be found here: [1](https://apkcombo.com/blokada-4/org.blokada.alarm/download/phone-4.15.0-apk), [2](https://www.apkmirror.com/apk/blokada/blokada-3/blokada-3-4-15-0-release/blokada-4-15-0-android-apk-download/), but they are different, very suspicious! Virustotal says they both are not invected ([1](https://www.virustotal.com/gui/file/1f8cfc7454134eacecb543dd9636fe1c12f289c86217f40a5b4816d63575bfe0),[2](https://www.virustotal.com/gui/file/ba76d9a881412e1fe8eb310c0b26cd14897087e01997ca0647aa7d7a4a3a959a)), but libs in there are different. I wouldn't install this.
- Lastly, I [pulled](https://stackoverflow.com/questions/4032960/how-do-i-get-an-apk-file-from-an-android-device) well-working apk v4.11.1 from my phone and put it [here](https://github.com/mtxadmin/ublock/raw/refs/heads/master/docs/blokada%204.11.1.apk)


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

Update: its depelopment [stopped](https://github.com/ch4t4r/nebulo) in 2022

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

*Nebulo has an interesting feature: Non-VPN mode. So, theoretically, you can use AND Blokada, AND Nebulo. Or AND Blokada, AND any non-filtering VPN app. This is a very promising feature. But in practice, since Android can send DNS queries only on port 53, and the system cannot allow you to set port number in Nebulo lower than 1024, you have to [make a local port redirect](https://github.com/Ch4t4r/Nebulo/blob/master/docs/NONVPNMODE.md) for that.*

## AdAway

AdAway is well-known app, free and opensource. But:
- It needs root. Update: now it can work without root too (local VPN mode)
- [It does not](https://github.com/AdAway/AdAway/issues/678) support asterisks. Asterisks can be in the whitelist there, but the blacklist is ordinary system [hosts file](https://en.wikipedia.org/wiki/Hosts_(file)).

## NextDNS

NextDNS is a service, not an app, but it's worth mentioning.

Pros:
- It is [efficient](https://github.com/serverless-dns/blocklists/pull/81#issuecomment-1381256209) with larger lists

Cons:
- The free version is [still](https://github.com/mtxadmin/ublock/issues/54#issuecomment-1381079479) unusable, query limit is far too low
- You cannot add your blocklist to the system
- Paid plans [still](https://github.com/serverless-dns/blocklists/pull/81#issuecomment-1383155144) "launching soon"
- Its blog stopped in [2022](https://blog.rethinkdns.com/)

## AdGuard

Pros:
- It has versions for Windows, Android, iOS
- It supports custom filters (like this). Didn't tested it though.

Cons:
- App can filter traffic for the whole system, but it is [paid](https://adguard.com/en/adguard-android/overview.html) (~30$ a year or ~100$ lifetime)
- The app is not open source

## DNS66

DNS66 is another hosts-blocking app. But:
- Its depelopment [stopped](https://github.com/julian-klode/dns66) in 2021
- It [does not support](https://github.com/julian-klode/dns66/issues/423) asterisks in hosts

## Pi-Hole

Pi-Hole is a well-known Linux-based locally hosted app. It still doesn't support wildcard domains in blocklists

https://www.reddit.com/r/pihole/comments/bu8fvz/enhance_pihole_with_wildcard_blocking_adguard/

https://discourse.pi-hole.net/t/using-blocklist-to-add-wildcard-blocked-domains/13561

https://discourse.pi-hole.net/t/support-wildcards-in-local-dns-records/32098/24

https://www.reddit.com/r/pihole/comments/bu8fvz/enhance_pihole_with_wildcard_blocking_adguard/

Additionally, it doesn't support regexes or wildcards in blocklists. Example ("Domains on Adlists: 0" after importing):

https://raw.githubusercontent.com/mmotti/pihole-regex/master/regex.list

This is [by design](https://discourse.pi-hole.net/t/collection-of-regex-for-blacklisting/43178/10).

## Other

Please note that there is no point in adding this file to uBlock Origin, although it partially understands this format - it’s better to use [full version of subscription](../README.md) for this.
