---
title: Mac 安裝
isChild: true
anchor:  mac_setup
---

## Mac Setup {#mac_setup_title}

macOS 會預載PHP, 但通常都會略舊於最新的穩定版. 有許多的方式可以在 macOS 上安裝最新版本的 PHP。

### 使用 Homebrew 安裝 PHP

[Homebrew] 是一個 macOS 的套件管理器, 可以幫助你輕易的安裝 PHP 與許多其他的擴充套件. Homebrew 核心庫源提供了 PHP 5.6, 7.0, 7.1 與 7.2 的相關"配方". 使用以下指令來安裝最新版本:

```
brew install php@7.2
```

你可以透過修改 `PATH` 變數來切換 Homebrew PHP 版本. 或是可以使用[brew-php-switcher][brew-php-switcher] 來自動切換 PHP 版本.

### 使用 Macports 安裝 PHP

[MacPorts] 是一個由社群發起的開源專案, 主旨是設計一個可以輕易編譯, 安裝, 升級各種基於 command-line, X11 或是 Aqua 的 OS X 作業系統開源軟體.

如果你缺少了某些套件, MacPorts 支援預編譯的二進制文件, 因此你不需要每次都從相依套件的原始檔壓縮包來重新編譯, 這可以省下你很多的時間.

此時, 你可以使用 `port install` 指令來安裝 `php54`, `php55`, `php56`, `php70` 或 `php71`, 比如:

    sudo port install php56
    sudo port install php71

你也可以執行 `select` 指令來切換目前的 PHP 版本:

    sudo port select --set php php71

### 使用 phpbrew 安裝 PHP

[phpbrew] 是一個可以安裝並且管理不同 PHP 版本的工具. 在應用程式/專案需要不同版本的 PHP 時它非常的方便, 讓你不再需要使用虛擬機.

### 透過 Liip's binary installer 安裝 PHP

另一個熱門的選擇是 [php-osx.liip.ch], 他提供了從版本 5.3 至 7.3 的單行安裝方法. 它並不會覆寫原本 Apple 系統中的 PHP 二進制檔案, 而是會安裝在一個獨立的位置(/usr/local/php5).

### 從原始檔編譯

另一個可以提供你控制安裝 PHP 版本的方法就是[自行編譯][mac-compile]. 如果採用這個方法, 請先確認是否已經透過 Apple's Mac Developer Center 安裝了 [Xcode][xcode-gcc-substitution] 或是 ["Command Line Tools for XCode"].

### 整合安裝包

上面所列出的方法, 主要都是針對 PHP 本身, 但不提供像是 Apache, Nginx 或是 SQL 伺服器. 整合包像是 [MAMP][mamp-downloads] 與 [XAMPP][xampp] 將可以為你安裝這些其他的軟體並且將他們都綁在一起, 但易於安裝的同時也犧牲了一些彈性.

[Homebrew]: https://brew.sh/
[Homebrew PHP]: https://github.com/Homebrew/homebrew-php#installation
[MacPorts]: https://www.macports.org/install.php
[phpbrew]: https://github.com/phpbrew/phpbrew
[php-osx.liip.ch]: https://php-osx.liip.ch/
[mac-compile]: https://secure.php.net/install.macosx.compile
[xcode-gcc-substitution]: https://github.com/kennethreitz/osx-gcc-installer
["Command Line Tools for XCode"]: https://developer.apple.com/downloads
[mamp-downloads]: https://www.mamp.info/en/downloads/
[xampp]: https://www.apachefriends.org/index.html
[brew-php-switcher]: https://github.com/philcook/brew-php-switcher
