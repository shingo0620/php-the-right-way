---
title: Windows 安裝
isChild: true
anchor:  windows_setup
---

## Windows Setup {#windows_setup_title}

你可以從 [windows.php.net/download][php-downloads] 下載二進制檔. 解壓縮後, 建議你將 PHP 的所在位置加入 [PATH][windows-path] (php.exe所在的位置), 如此一來你就可以在任意的地方執行 PHP.

基於學習或是本地開發, 你可以使用 PHP 5.4+ 開始內建的網頁伺服器, 如此一來你就不需要擔心如何設定它. 若是你打算使用整合好 網頁伺服器 Mysql 的工具像是 [Web Platform Installer][wpi], [XAMPP][xampp], [EasyPHP][easyphp], [OpenServer][openserver] 與 [WAMP][wamp] 將可以為你快速的建立起 Windows 開發環境. 但是請注意, 如果你打算在 Windows 上開發然後部署至 Linux, 這些工具將會與實際的正式環境有些許的差別.

如果你需要將專案部署於 Windows, IIS7 將可以提供你最穩定與最好的效能. 你可以使用 [phpmanager][phpmanager] (一個 IIS7 的圖形化插件) 來輕易的設定與管理 PHP. IIS7 也有內建 FastCGI, 你只需要將 PHP 設定為他的處理器即可. 更多的相關資源請見[dedicated area on iis.net][php-iis].

一般而言, 專案在開發與上線時使用了不同的環境, 在實際上線時將會產生一些奇怪的Bug, 如果你是個 Windows 的開發者並且打算部署在 Linux(或是任何非 Windows 的系統) 上, 請認真的考慮使用[虛擬機](/#virtualization_title).

Chris Tankersley 寫了一篇關於他[在 Windows 開發 PHP][windows-tools] 所使用的工具的實用文章.

[easyphp]: http://www.easyphp.org/
[phpmanager]: http://phpmanager.codeplex.com/
[openserver]: http://open-server.ru/
[wamp]: http://www.wampserver.com/en/
[php-downloads]: http://windows.php.net/download/
[php-iis]: http://php.iis.net/
[windows-path]: http://www.windows-commandline.com/set-path-command-line/
[windows-tools]: http://ctankersley.com/2016/11/13/developing-on-windows-2016/
[wpi]: https://www.microsoft.com/web/downloads/platform.aspx
[xampp]: http://www.apachefriends.org/en/xampp.html
