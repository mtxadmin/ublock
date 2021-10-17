[Нажмите сюда для русской версии](README.md)

#### Yet another small uBlock filter list

Constantly updated filter list for uBlock Origin. Removes banners and spying modules, blocks fraudulent sites. And also removes different annoyances from internet pages. [See the full list here.](docs/policy_en.md) Let's make sites cleaner and reading more comfortable and secure!

Also, there is a child project - [Yet another small hosts file](docs/hosts_file_en.md) and [Yet another smart Blokada hosts file](docs/hosts_file_blokada_en.md)


## How it works?

### Example of site *BEFORE* installing this filter list:

![scrolling_video_newsletter_header_share_icons highlighted](https://user-images.githubusercontent.com/22258847/51348578-16f08980-1a71-11e9-80b8-0f2ad5379bcd.png)

Despite you checked all filters in uBlock Origin (i.e. set default lists), you see some annoyance elements. 

### View of the same site *AFTER* installing the filter list:

![afterinstall](https://user-images.githubusercontent.com/22258847/51348138-e8be7a00-1a6f-11e9-9b0c-5fac61a83f8f.png)

(The example is from a friendly project, inspired to develop the idea. The idea has developed very much further, but the example gives a good idea)

Of course, the matter is not limited to visual removal of unnecessary things - as mentioned above, [ads, tracking scripts, etc., etc. ...](docs/policy_en.md) are deeply blocked. Many of the rules in this list are based on colleagues' findings (see references `from` in the sources), but many were found independently and were absent in the available sources at the time of adding.


## How to setup this filter list?

First, if you didn't setup [uBlock Origin](https://github.com/gorhill/uBlock) yet, do it right now. For the time, it is the best banner blocker solution. Think it so: tens of cool and skilled people all around the world will try to make you see *less* ads. :-)

#### On a PC

- [uBlock Origin для Google Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)

- [uBlock Origin для Mozilla FireFox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)

- [uBlock Origin для Apple Safari](https://github.com/el1t/uBlock-Safari#installation)

- [uBlock Origin для Opera](https://addons.opera.com/extensions/details/ublock/)

#### On a smartphone

- [uBlock Origin для Mozilla FireFox на Android](https://addons.mozilla.org/EN-US/android/addon/ublock-origin/) 


## Additional settings

After installing uBlock Origin check its settings:

1. Open uBlock Origin window, pressing the key ![](https://user-images.githubusercontent.com/22258847/39936895-7ca7a8fc-553d-11e8-9496-45a96b623614.png).
2. Go to Settings ![](https://user-images.githubusercontent.com/22258847/39938114-5dc5cf00-5541-11e8-996d-5d583611f76f.png)
3. Select Filter lists tab
4. Check, that on the Filter lists tab two upper checkboxes are enabled and the third checkbox is disabled:
- Auto-update filter lists 
- Parse and enforce cosmetic filters
- Ignore generic cosmetic filters

The third checkbox sometimes is enabled after installing. Disable it, or else many blocking rules will not work. Right view of these settings:

![](https://raw.githubusercontent.com/mtxadmin/ublock/master/docs/images/ublock_settings_general_en.png)


## Adding the list

After setup, click [this link](https://subscribe.adblockplus.org/?location=https%3A//raw.githubusercontent.com/mtxadmin/ublock/master/it). In next window press Subscribe and that's all.

<details>
    <summary>
    Sometimes this method maybe doesn't work. Let's do it long way.
    </summary>
  
1. Open uBlock Origin's window, pressing its button ![](https://user-images.githubusercontent.com/22258847/39936895-7ca7a8fc-553d-11e8-9496-45a96b623614.png).

2. Go to settings ![](https://user-images.githubusercontent.com/22258847/39938114-5dc5cf00-5541-11e8-996d-5d583611f76f.png)

3. Choose Lists tab

![](https://user-images.githubusercontent.com/22258847/39937403-1da7b8b8-553f-11e8-865a-73a3f2fa4bb8.PNG). 

4. Scroll to bottom and add the address:

> ```

``https://raw.githubusercontent.com/mtxadmin/ublock/master/it``

> ```

5. Press Apply button. 


I noticed the list sometimes cannot be added from the first try. Yes, it's happens, I don't know why. Please try again. Or you can add zero to the address:

> ```

``https://raw.githubusercontent.com/mtxadmin/ublock/master/it0``

> ```

After successful installing you will see "Yet another small uBlock filter list" label. It means you did it.

The author of [the friendly project](https://github.com/yourduskquibbles/webannoyances/) made a small demonstration of adding list. The process looks like that (with different address, of course):

![](https://user-images.githubusercontent.com/22258847/39935902-25add6be-553a-11e8-82b0-badc73f44ed3.gif)
</details>


## Adding more lists

As you may have noticed in the previous paragraph, there are a lot of lists on the Filter lists tab. These are the lists installed "out of the box" with adblocker - the oldest and well known.

When setting up, I usually enable maximum number of them. Maybe, except regional lists.

Also, you can add some other filter lists:

- NoCoin Filter List<br>
A good list to block mining scripts. Many servers from it added in different lists too, but the author constantly finds something new. The list address:
https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/nocoin.txt

- Web Annoyances Ultralist<br>
A list designed to block annoying and generally distracting elements. The list address:
https://raw.githubusercontent.com/yourduskquibbles/webannoyances/master/ultralist.txt

<details>
    <summary>
        What about of more lists?
    </summary>
    See additional lists on https://filterlists.com . But many of them, unfortunately, were abandoned long time ago - see the last change dates.
</details>


## Feedback

Maybe something doesn't work? Something is missing? Please, feel free to write about it here:

https://github.com/mtxadmin/ublock/issues/new

(it will need a GitHub account. If you don't have one yet, create it - that is easy and useful)
