[Нажмите сюда для русской версии](README.md)

#### Yet another small uBlock filter list

Constantly updated filter list for uBlock Origin. Removes banners and spying modules. And also removes different [annoyances](docs/policy_en.md) from internet pages. Let's make sites cleaner and reading more comfortable!

Also, there is a child project - [Yet another small hosts file](docs/hosts_file_en.md) 

## How it works?

### Example of site *BEFORE* installing this filter list:

![scrolling_video_newsletter_header_share_icons highlighted](https://user-images.githubusercontent.com/22258847/51348578-16f08980-1a71-11e9-80b8-0f2ad5379bcd.png)

Despite you checked all filters in uBlock Origin (i.e. set default lists), you see some annoyance elements. 

### View of the same site *AFTER* installing the filter list:

![afterinstall](https://user-images.githubusercontent.com/22258847/51348138-e8be7a00-1a6f-11e9-9b0c-5fac61a83f8f.png)

(The example is from a friendly project, inspired to develop the idea.)

## How to setup this filter list?

First, if you didn't setup [uBlock Origin](https://github.com/gorhill/uBlock) yet (variant: [Nano Adblocker](https://github.com/NanoAdblocker/NanoCore)), do it right now. For the time, it is the best banner blocker solution. Think it so: tens of cool and skilled people all around the world will try to make you see *less* ads. :-)

#### On a PC

- [uBlock Origin для Google Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm)

- [uBlock Origin для Mozilla FireFox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)

- [Nano Adblocker для Microsoft Edge](https://www.microsoft.com/en-us/p/nano-adblocker/9nsxdx2tdb3v/)

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

After setup, press [this link](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/mtxadmin/ublock/master/it). In popup window press Ok and that's all.

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


Is something not working? Something is missing? Write about it here:
https://github.com/mtxadmin/ublock/issues/new
