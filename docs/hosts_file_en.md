[Нажмите сюда для русской версии](hosts_file_ru.md)

#### Yet another small hosts file

This is the [hosts file](https://en.wikipedia.org/wiki/Hosts_(file)) for blocking ads, counters, telemetry and [other things](policy_en.md). It is generated from the files of [the parent project](../README_en.md) and is periodically updated.

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
- Blocking works continuously and [does not require resources](hosts_file_performance_en.md)

Thus, it is best to install **AND** an ad blocker in the browser, **AND** an application that updates the hosts.

What application to install? Anyone that can download new versions of hosts from the Internet. Of course, it is much better if you can specify several sources at once to combine them. For Android, for example, you can look at [AdAway](https://github.com/AdAway/AdAway) - an open, free project. Or any other to your taste. Unlike the browser ad blocker, there are minimum requirements for such an application. For Windows you can use [hostsmgr](https://github.com/henrypp/hostsmgr) (console) or some autoupdating Powershell scripts. (Also, there is [HostsMan](http://www.abelhadigital.com/hostsman/) with GUI, but it doesn't work with Github files [[1]](https://github.com/crazy-max/WindowsSpyBlocker/issues/103))

Also, there is mentions that Windows Defender could assume changing HOSTS-file with telemetry blocking as a bug/error: [[1]](https://www.bleepingcomputer.com/news/microsoft/windows-10-hosts-file-blocking-telemetry-is-now-flagged-as-a-risk/),[[2]](https://windowsreport.com/windows-hosts-file-modification-bug/)

The address of the hosts file of this project:
> ```
``https://raw.githubusercontent.com/mtxadmin/ublock/master/hosts.txt``
> ```

Please note that there is no point in adding this file to uBlock Origin, although it understands this format - it’s better to use [full version of subscription](../README.md) for this.
