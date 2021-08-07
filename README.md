# kde-config
My own linux kde plasma quick configurations. Kde is a nice choice which has various fabulous styles. Document has many languages. But it's a whole document. Read it continously regardless of the language. 給出的字體文件之保留作爲自己方便遷移環境時候下載。之後如果有能力將擴展更多語言作爲文檔語言。作爲系統發行版本選擇，Manjaro 個人認爲比 openSUSE 更加方便使用。AUR 軟件源十分豐富而且速度很快，不需要像 zypper 每次安裝都要加載刷新已經存在的源很慢。Mein name ist Nylsus. Sehr danke!

## English
**This is a configuration guidance if you are using kde as linux desktop solution. It's personal, not granted anything like speed or fluency.** Steps are as follows.
* Font. Configure font in **System Settings > Apperance > Fonts**(In different linux distributions, you may use different global configurations. For example, in Manjaro, use `/etc/fonts/local.conf` or `/etc/fonts/conf.d/*` to make a personal configuration. But here, System Settings is just a convenient, quick and visual choice.)
![](screenshots/fonts.png)
    * The names of the fonts are:
    * San Francisco Display Medium (replacements: SF Pro Display, SF UI Text)
    * Sarasa Gothic K
    * PingFang SC
    * Menlo
    * Monaco
* In **System Settings > Apperance**:
  * Application Style. It decides the menu style. Here provides only one note: Set the transparency to **30%** or **40%**.
![](screenshots/application.png)
  * Plasma Style. Use **Future**. Download it from **Get New Plasma Style**.
  * Colors. This may change very frequently. You can customize your own color sheet from **Breeze Light**.
  * Window Decorations. Use **Breeze Blur** or **Genome L. Blur Flat**. Just remember, make the window title bar **BLUR**.
  * Icons. **Mkos-BigSur-Light**. 
  * Splash Screen. **None**.
* In **System Settings > Workspace > Workspace Behaviour**
  * General Behaviour > Animation Speed. **9/16**.
  * Desktop Effects > Apperance. **Fall apart, Fading Popups, Woobly windows, Magic lamp**
* In **System Settings > Hardware > Display and Monitos**
  * Night Colour. **Always On**. **3700K**.
* Back to Desktop. Right click to **Edit Panel**.
  * Make bottom panel and top panel.
  * Bottom panel height **82**. Add **Icon Only Task Manager**. Add two **Panel Spacer** to make task manager be the middle. Order: Panel Spacer + Icon Only Task Manager + Panel Spacer. Make panel **Auto-Hide**.
  * Top panel height **32*. **Application Menu + Global Menu + Panel Spacer + Search + Networks + Battery + Digital Clock (Fuzzy Clock)**. 

## 中文
按照上述的字體方案，中文字體推薦使用兩種字體，分別是 PingFang SC 和 Sarasa Gothic K。
* Kate的配色方案。參見附件 `Nat.theme`。在 Kate 中 Configure Kate 然後在 Color Theme 中導入該配色配置文件即可。字體選擇 Monaco 17 或者 Monaco 16。一般其他插件需要安裝或者顯示 File System Browser, Preview。
* 全局字體推薦使用 Sarasa Gothic K 或者 PingFang SC。附件的 `conf.d` 和 `local.conf` 屬於 `/etc/fonts/` 目錄下。有些部分的字體需要但那都設置例如 Firefox 瀏覽器字體配置。
* 輸入法配置。請安裝使用 Fcitx。然後安裝 fcitx-rime。附件給出的 `rime` 文件夾應該放在 `~/.config/fcitx/` 目錄下。注意主題配置文件不在此目錄，配置主題和部分設置例如快捷鍵（這裏推薦使用 Alt-Space ）可以使用 fcitx-configtool（需要單獨安裝）。
* visual studio code 配置。該文本編輯器使用較少，但是功能很多。配色主題使用 Brackets Light Pro，字體使用 Monaco 和 PingFang SC。文件圖標和其他圖標使用 Fluent Icon/UI。安裝 code runner， 在設置中配置 run in terminal。
* emacs 配置。該配置並沒有很好解決中文顯示問題。主要用於保存一些配色和主題文件。參見 `.emacs.d` 文件夾。
