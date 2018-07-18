---
title:   常見的目錄結構
isChild: true
anchor:  common_directory_structure
---

## 常見的目錄結構 {#common_directory_structure_title}

在剛開始開發網頁程式時一個常見的問題是, "我要把東西放在哪?" 許多年過去了, 這個問題的答案依然是 "`DocumentRoot` 的所在." 雖然這個答案並不完整, 但這是一個好的開始位置.

基於安全性的理由, 設定檔案不應該被網站的瀏覽者取得; 所以, 公開的程式就保留在一個公開的目錄中, 而私人的設定和資料則存放在這個目錄之外.

對於參與一個團隊, CMS, 框架, 一個標準的目錄結構就是其正在使用的結構. 但是, 如果是一個獨立執行的專案, 知道該使用何種檔案目錄架構是艱鉅的.

[Paul M. Jones] 針對 github 上成千上萬的專案進行了一個出色的研究. 基於這個研究編排了一份檔案與目錄的標準結構, [Standard PHP Package Skeleton]. 在這個目錄結構中, `DocumentRoot` 應該要指向 `public/`, 單元測試應該要放在 `tests/` 目錄中, 而第三方的程式庫, 就如同使用 [composer] 安裝, 放置於 `vendor/` 目錄中. 其他的檔案與目錄, 遵守 [Standard PHP Package Skeleton] 對於參與專案來說會是個最合理的方式.

[Paul M. Jones]: https://twitter.com/pmjones
[Standard PHP Package Skeleton]: https://github.com/php-pds/skeleton
[Composer]: /#composer_and_packagist
