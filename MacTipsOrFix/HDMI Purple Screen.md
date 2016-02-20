---
layout: page
title: "HDMI Purple Screen"
description: 
tagline: Macbook Pro HDMI輸出外接螢幕偏紫
group: TipsForMac
---
{% include JB/setup %}

##問題

##環境
系統：OS X EI Capitan  
輸出方式：HDMI  
螢幕型號：ViewSonic VX2270


##解法
[Force RGB mode in Mac OS X to fix the picture quality of an external monitor](http://www.ireckon.net/2013/03/force-rgb-mode-in-mac-os-x-to-fix-the-picture-quality-of-an-external-monitor/comment-page-11#comment-14866)

1. Run [Fix Script](https://gist.github.com/adaugherity/7435890).
  * 修正產生檔案中的DisplayProductName, 除去亂碼資料。
3. boot into recovery mode (Command+R) and start Terminal from the Utilities menu.
4. 複製檔案至/Volumes/ Macintosh\ HD/System/Library/Displays/Contents/Resources/Overrides/DisplayVendorID-XXXX  
  * Turn off FileVault to find /Volumes/ Macintosh\ HD/
5. reboot


##參考資料
[How to modify System Integrity Protection in El Capitan](http://www.macworld.com/article/2986118/security/how-to-modify-system-integrity-protection-in-el-capitan.html)
[外接 HDMI 螢幕模糊問題解決方法](http://iphone4.tw/forums/showthread.php?t=206400)