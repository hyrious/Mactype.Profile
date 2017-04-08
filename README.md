# Mactype.Profile.Mac

Mactype's profile for self use.  
Trying to find the best solution that similar to Mac.

### Notes

For the best visual effect, please make sure the scale of your PC is 100% or 200%, etc.

If you meet crashes, try run with **HotShift & AsAdmin**.

Mactype seems not to work well on Windows 10 Version 1703, even with the newest CTP build.  
Use 1607 instead and wait for any side's solution.  
Having Retina screen, I suggest you use 200%/300%/etc on the newest (1703) Win10 without Mactype, which seems a bit better than before.

## Install

1. Install Fonts.
    - [XHei OSX](https://pan.baidu.com/s/1ntqNBrb)
    - [Inziu IosevkaCC SC](https://be5invis.github.io/Iosevka/inziu.html)
2. Install [Mactype](http://www.mactype.net/).
3. Download [the latest release](https://github.com/hyrious/Mactype.Profile.Mac/releases/latest), extract it to Mactype's ini folder.  
   e.g. `C:\Program Files\MacType\ini`
4. Run `MacWiz`(`Mactype 用户向导` in Chinese) from Start Menu, choose this profile marked hyrious and \[OK\].

## Information

Inspired by 3 profiles:  
- LCD.W7.默认字体.仿Mac.ini (at `<Mactype>/ini/`, default INIs)
- OSX.ini (at `<Mactype>/ini/IoF/HotShift/HotShift→XHei…`, default INIs)
- [Mactype.Decency](https://github.com/renkun-ken/MacType.Decency)

## Recommended Applications

Applications that friendly to Mactype.
- [CentBrowser](https://www.centbrowser.com/): Turn off **DirectWrite** at **chrome://flags**.

## Still, there are many apps not fully supporting Mactype

osu!, VirtualBox, PaintToolSAI, etc.

The suggestion is make Mactype turn blind to these specific apps:  
put them into section **[UnloadDll]** or **[ExcludeSub]**.
