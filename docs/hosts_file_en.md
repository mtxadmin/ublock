[Нажмите сюда для русской версии](hosts_file_ru.md)

#### Yet another small hosts file

This is the [hosts file](https://en.wikipedia.org/wiki/Hosts_(file)) for blocking ads, counters and [other things](policy_en.md). It is generated from the files of [the parent project](../README_en.md) and is periodically updated.

Applying of the hosts file can be useful for general ad blocking in the system, not just in the browser.

**Restrictions:**
- The capabilities of the hosts file are limited only by blocking nodes by name
- Wildcard characters and name masks are not supported
- In general, nothing else from the rich arsenal of browser-type banner cutters like uBlock Origin is supported
- To change the hosts file, you need full rights in the system. Administrator on Windows, root on Android, jailbreak on iOS
- When connecting via a proxy server, the hosts file will most likely not be used
- When updating the hosts file, it is desirable to reboot the system
- There are no applications updating hosts on official app markets (for example, Google deletes them for blocking ads).

However, there are **advantages:**
- Blocking with the use of hosts applies to the entire system. Banners and commercials in applications, various telemetry and other
- Blocking works continuously and does not require resources

Thus, it is best to install **AND** banner cutter in the browser, **AND** application that updates the hosts.

What application to install? Anyone that can download new versions of hosts from the Internet. Of course, it is much better if you can specify several sources at once to combine them. For Android, for example, you can look at [AdAway] (https://github.com/AdAway/AdAway) - an open, free project. Or any other to your taste. Unlike the banner banner cutter, there are minimum requirements for such an application.

The address of the hosts file of this project:
> ```
``https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts.txt``
> ```

Please note that there is no point in inserting this file into uBlock Origin, although it understands this format - use better [the full version of the subscription](../README.md) for this.
