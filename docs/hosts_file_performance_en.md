 [Нажмите сюда для русской версии](hosts_file_performance_ru.md)

On the Internet there are some opinions that with a large [hosts file](hosts_file_en.md) the system can slow down. Is it true?

### Android:
I’ve been using huge hosts files since 2012, and I’m not aware of any performance issues on any available device — and they were then small and weak. Theoretically, some effect may be present, but practically the acceleration from blocking advertising and other parasitic requests far outweighs this effect, even if it exists.

The author of the MoaAB hosts file [confirms this](https://forum.xda-developers.com/showthread.php?t=1916098), although he [notices](https://forum.xda-developers.com/showpost.php?p=62564889&postcount=3313), that using a large (7-8 MB) hosts file causes a consumption of 30-50 MB of RAM:

> ``>>>`` Performance Issue? Will my device run SLOW?<br>
> I am using this 'hosts' file from my chilhood days and never had any performance issue to date, Although you might have a little delay in startup for few seconds (but you will not even notice) and then everything will be cool in standby and active mode. I say "Little delay is better than ADs, Malwares and Spywares..."

> Minimum RAM requirment is only 512MB to 1GB. MoaAB only consumes 30-50MB in general and dont kill the device in any way. ... In practial MoaAB is just small fraction of system load

He also mentions that there were memory leak errors in Android 5.0. Earlier and later versions are not affected by this error.


### Windows:
On Windows 7 (and older) in some cases, indeed, there may be slowdowns. On Windows 10, Microsoft finally made a change, and this problem is already irrelevant. For details, see the author of the hosts file with a 20-year (!) History: http://winhelp2002.mvps.org/hosts.htm

It is worth noting that Windows 7 has already been withdrawn from support and does not receive updates. If you are using this version, or even older, you can try to disable the DNS Client service (see the link above for details). But it is better to go to the current version.

#### Update 2023:
Now on Windows systems Microsoft Antivirus actively protests against hosts file changing. In case of small file, it just throws a "virus-like" notification and suggests user to rollback hosts file to default. In case of relatively big file, it may conflict with network services and therefore render the system unusable.

So, don't directly change hosts file on Windows system. Microsoft wants their telemetry up and running. But you can use intermediate tool like Pi-hole, external DNS or something other solution.
