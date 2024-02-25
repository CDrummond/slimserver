Logitech Media Server
====

Logitech Media Server (aka. LMS, fka. SlimServer, SqueezeCenter, SqueezeboxServer, SliMP3) is the server software that powers audio players from [Logitech](https://www.logi.com) (formerly known as SlimDevices), including [Squeezebox 3rd Generation, Squeezebox Boom, Squeezebox Receiver, Transporter, Squeezebox2, Squeezebox and SLIMP3](http://wiki.slimdevices.com/index.php/Squeezebox_Family_Overview), and many software emulators like [Squeezelite and SqueezePlay](https://sourceforge.net/projects/lmsclients/files/).

With the help of many plugins, Logitech Media Server can stream not only your local music collection, but content from many music services and internet radio stations to your players.

Logitech Media Server is written in Perl. It runs on pretty much any platform that Perl runs on, including Linux, Mac OSX, Solaris and Windows.

## SB Radio, SB Touch, SB Controller and Logitech Media Server 8+

Unfortunately the latest Squeezebox Radio/Touch/Controller firmwares (7.x) come with a bug which causes some irritation connecting to Logitech Media Server 8+. The version string comparison function fails to recognize 8.0.0 as more recent than 7.7.3. While the bug has been fixed years ago, the fixed firmware never got officially released.

There's a workaround built in to Logitech Media Server 8+ now, but you might still get warnings in the log file or on the device.

[The Squeezebox Community has come up with a custom firmware](https://forums.slimdevices.com/forum/user-forums/3rd-party-software/110192-announce-community-firmware-for-squeezebox-radio-touch-controller-and-lms-8?p=1457947#post1457947) which, among other bugs, fixes this issue. If you feel confident enough, you can install that 3rd party provided firmware on your device. In LMS go to "Settings/Manage Plugins" to install the "Community Firmware" plugin from the 3rd party section.

## Outdated workaround instructions for outdated Radio firmware

__Please do not apply this procedure unless you trust a partially patched firmware more than you'd trust a community built alternative firmware__ as outlined in the previous section. We strongly recommend the Community Firmware over applying the patch.

At this point in time we're unfortunately not able to build an official, fixed firmware for distribution.

If you prefer not to replace the full firmware of your Squeezebox _Radio_ (only!), there's a patch available which you can install:

* On the Squeezebox go to Settings/Advanced/Applet Installer. Make sure "Recommended Applets Only" is unchecked, then install the Patch Installer. The device will re-boot.
* Once it's back, go to Settings/Advanced/Patch Installer and install the "Version Comparison Fix".

Enjoy the music on your Squeezebox!
