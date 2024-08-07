
Эти боты помогут сделать пробив гораздо дешевле:

Usеrbоx (https://t.me/user_szbot)

Глaз Бoга (https://t.me/yahoobotgbot)

Fun-stat-bot (https://link.funstat.ru/)

Unamer (https://t.me/unamer_bot)

Quick OSINT (https://t.me/QulickOoSI1NTquilckoOSIiNT1bot)

GTA Search (https://t.me/gta_searchers_bot)

XKeyscore (https://t.me/XKeyscore_search_bot)

Onion Market — анонимный Р2Р-обменник для людей! (http://t.me/onion_market_bot)





# **Geogramint - OSINT Geolocalization tool for Telegram**
<p align="center">
<img src="https://github.com/Alb-310/Geogramint/blob/master/appfiles/Geogramint.png" width="300"/>
</p>

<p align="center"> <img src="https://img.shields.io/badge/version-1.4-orange" /> <img src="https://img.shields.io/badge/PYTHON-03b1fc?style=for-the-badge&logo=python"/> <a href="https://github.com/Alb-310"> <img alt="GitHub" src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/><a/> <a href="https://twitter.com/Alb_310"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/by-alb310.svg"/><a/> <img src="https://img.shields.io/badge/License-GPLv3-blue.svg"/>
<p align="center"> <a href="https://projetfox.com/"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/fox%20badge.png" width="200"/> <a/>

## **About**

Geogramint is an OSINT tool that uses Telegram's API to find nearby users and groups. Inspired by [Tejado's Telegram Nearby Map](https://github.com/tejado/telegram-nearby-map), which is no longer maintained, it aims to provide a more user-friendly alternative.

Geogramint only finds Telegram users and groups which have activated the nearby feature. Per default it is deactivated.

The tool is fully supported on Windows and partially supported on Mac OS and Linux distributions.

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/assets/52386954/7dde5789-2a58-438e-a256-06b4612f1443" />

## 🛠️ Installation

**Requirements:** [Python 3.9, 3.10 or 3.11](https://www.python.org/downloads/release/python-3112/)<br>

### On Windows [![Windows](https://img.shields.io/badge/Windows-03b1fc?style=for-the-badge&logo=windows)](https://svgshare.com/i/ZhY.svg)

+ #### With the installer: Click [here!](https://github.com/Alb-310/Geogramint/releases)
+ #### With Github:
```bash
git clone https://github.com/Alb-310/Geogramint.git
cd Geogramint/
pip3 install -r requirements.txt

python3 geogramint.py # for GUI mode
python3 geogramint.py --help # for CLI mode
```
Or depending on your installation :
```bash
git clone https://github.com/Alb-310/Geogramint.git
cd Geogramint/
pip install -r requirements.txt

python geogramint.py # for GUI mode
python geogramint.py --help # for CLI mode
```

### On Mac OS  ![macOS](https://img.shields.io/badge/Mac_OS-abbfc7?style=for-the-badge&logo=apple) and Linux ![Linux](https://img.shields.io/badge/Linux-ffffff?style=for-the-badge&logo=linux)

+ #### With Github:
```bash
git clone https://github.com/Alb-310/Geogramint.git
cd Geogramint/
pip3 install -r requirements.txt

python3 geogramint.py # for GUI mode
python3 geogramint.py --help # for CLI mode
```
Or depending on your installation :
```bash
git clone https://github.com/Alb-310/Geogramint.git
cd Geogramint/
pip install -r requirements.txt

python geogramint.py # for GUI mode
python geogramint.py --help # for CLI mode
```

More details in the [Wiki](https://github.com/Alb-310/Geogramint/wiki/Installation-Guide).


## 📡 Example: GUI

1. Start by creating an API key for your Telegram account [here](https://my.telegram.org). You will also need to put a profile picture on your account and, in your `Privacy and Security` settings, enable the profile picture for everyone.

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/privacy_settings.jpg" width="300"/>

2. Launch **Geogramint**
3. In the settings, write your information (api_id, api_hash and phone number), report preference and then `save`

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/Geogramint_settings_1.png" width="500"/> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/Geogramint_settings_2.png" width="500"/>

4. Choose the location where you want to search, either by moving around the map or by using the search feature with coordinates in `lat, lon` format

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/Geogramint_search.png" width="700"/>

5. Telegram will send you a verification code, write it in the pop-up window (+ your two-step verification password if you have one)

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/Geogramint_code.png" width="700"/>

6. Then click `Start Search`
7. All results will be displayed following: 
+ green for 500m
+ yellow for 1000m
+ orange for 2000m
+ red for >3000m

(NB: results can also be found in `Geogramint/cache_telegram/` in `json` and `csv` format + profiles pictures)

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/Geogramint_results.png" width="700"/>

8. `Reset` will clear the results and erase the `cache_telegram`

More details in the [Wiki](https://github.com/Alb-310/Geogramint/wiki/Demonstration:-GUI).

## 📡 Example: CLI

1. Start by creating an API key for your Telegram account [here](https://my.telegram.org). You will also need to put a profile picture on your account and, in your `Privacy and Security` settings, enable the profile picture for everyone.

<p align="center"> <img src="https://github.com/Alb-310/Geogramint/blob/master/.github/privacy_settings.jpg" width="300"/>

2. Launch **Geogramint**

![image](https://user-images.githubusercontent.com/52386954/210659094-506e3018-6784-4602-bf4e-e446534f6f15.png)

3. Start with the config, with the command `set-config` set your information (api_id, api_hash and phone number)

![image](https://user-images.githubusercontent.com/52386954/210659472-dbb1804e-dd8a-468e-b0a1-bfcd77652113.png)

4. Start the search feature by using coordinates in `lat lon` format with the command `start-scan` :

![image](https://user-images.githubusercontent.com/52386954/210659762-4fffc2ac-957d-4377-9615-d339dcb17aef.png)

 <p align="center"> <img src="https://user-images.githubusercontent.com/52386954/210661716-9a3db8c7-4627-447e-b18b-dcf2c8c54a36.png" width="500"/>
  <p align="center"> ⬇ </p>
  
<p align="center"> <img src="https://user-images.githubusercontent.com/52386954/210661742-7e7a6242-5915-4b0e-a52d-38d4dd779eff.png" width="500"/>
 
5. All results will be displayed following: 
+ green for 500m
+ yellow for 1000m
+ orange for 2000m
+ red for >3000m

(NB: results can be exported depending options used with `start-scan`, by default profile pictures and results in `json` format are present in `Geogramint/cache_telegram/`)

6. `reset-scan` will clear `cache_telegram`

More details in the [Wiki](https://github.com/Alb-310/Geogramint/wiki/Demonstration:-CLI).
  
## 📖 Wiki

Remember to check the [Wiki](https://github.com/Alb-310/Geogramint/wiki) before posting an issue or asking a question.

## 📝 License

[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.fr.html)

## 🙏 Thanks to:
+ My teammates at Projet FOX
+ [sergiombd](https://github.com/sergiombd)












![TOSINT](https://user-images.githubusercontent.com/76810020/118490326-bb546a80-b715-11eb-96e8-9ec87af27832.png)
<div align="center">
  <a href="https://awesome.re/">
  	<img src="https://awesome.re/badge-flat2.svg">
  </a>
</div>
<div align="center">
  	<b>👉 <a href="https://github.com/ItIsMeCall911/Awesome-Telegram-OSINT/pulls">Feel Free To Contribute</a> 👈</b>
</div>

## 📑 Contents

- [Search Engines](#-search-engines)
- [Directories & Catalogues](#-directories-and-catalogues)
- [Misc Directories & Catalogues](#-misc-directories-and-catalogues)
- [Tools](#-tools)
- [Bots](#-bots)
- [Resources](#-resources)

## [↑](#contents) Search Engines

* [Intelligence X](https://intelx.io/tools?tab=telegram)
* [Telegram Search Engine](https://xtea.io/ts_en.html#gsc.tab=0)
* [BUZZ.IM](https://search.buzz.im/)
* [Lyzem](https://lyzem.com/)
* [Telegram Chinese Search](http://www.sssoou.com/)
* [名刀电报搜索](https://xtea.io/ts.html#gsc.tab=0)
* [Telegra.ph Search Engine](https://telegcrack.com/)

## [↑](#contents) Directories And Catalogues
* [TelegramDB](https://telegramdb.org/)
* [Telemetrio](https://telemetr.io/en/channels)
* [TGStat](https://tgstat.ru/)
* [Telemetr](https://telemetr.me/)
* [TgramSearch](https://tgramsearch.com/)
* [TelegramCatalog](https://telegramcatalog.com/en/channels)
* [Telegram Catalog](https://telegram-catalog.ru/catalog/20)
* [Tgram](https://tgram.ru/channels)
* [TelegramGroup](https://www.telegram-group.com/en/)
* [Tgram.io](https://tgram.io/)
* [Tlgrm.eu](https://tlgrm.eu/channels)
* [HotTg](https://www.hottg.com/telegram-group/) - [Tg-Me](https://www.tg-me.com/)
* [Telegram Store](https://telegram-store.com/)
* [TelegramIndex](https://telegramindex.com/)
* [Telega.io](https://telega.io/catalog)
* [Combot](https://combot.org/telegram/top/groups)
* [Telegram Channels](https://telegramchannels.me/)
* [TGRM.SU](https://tgrm.su/)
* [All-Catalog Telegram](https://all-catalog.ru/)
* [Telegrator](https://telegrator.ru/channels/)
* [Telegram.org.ru](https://telegram.org.ru/channels/)
* [Telegram-Cat](https://telegrm-cat.com/channelscat/allchannels)
* [TeleChappy](https://telechappy.com/catalog/channels/)
* [Telegram Directory](https://tgdr.io/)
* [TGRAM β](https://tgram.me/channels)
* [BotLIST.ru](https://botlist.ru/)
* [TelegramBots.info](https://www.telegrambots.info/channels/)
* [Catalog-Telegram.info](https://catalog-telegram.info/)
* [LinkBaza](https://linkbaza.com/catalog)
* [@TMBotsStore](https://tmbots.info/)
* [Telegram Community](https://telegram.community/)
* [UzTelegram](https://uztelegram.com/)
* [ADD GROUPS](https://add-groups.com/telegram/)
* [Telegram Club](https://telegram-club.ru/)
* [Telegramzy](https://telegramzy.ru/katalog-kanalov/)
* [Tginfo](https://tginfo.ru/)
* [TelegramBox](https://tgbox.pro/)
* [TeleTarget](https://teletarget.com/catalog/)
* [TgCatalog](https://tgcatalog.ru/)
* [Telegram Region](https://telegram-region.com/)
* [ChannelGram](https://channelgram.com/)
* [Telegros](https://telegros.ru/)
* [ReaderGRAM](https://readergram.com/)
* [电报群组大全](https://www.dianbaoqun.net/)
* [Taiwan Group Index](https://www.telegram.url.tw/)
* [Telegram 公眾索引系統](https://tgtw.cc/)
* [TgChannels](https://en.tgchannels.org/)
* [Telegoo](https://telegoo.net/)
* [TelegramReader](https://telegramreader.com/)
* [Telegram-Sliv](https://telegram-sliv.ru/)
* [TG頻道群組合集](https://telegramgroups.com.hk/)

## [↑](#contents) Misc Directories And Catalogues

* [Telegram-List](https://github.com/goq/telegram-list)
* [TELEGRAM CATALOG](https://katalogtelegram.ru/)
* [Telegram channel list](http://telegram-downloads.ru/kanaly)
* [r/TelegramChannels](https://www.reddit.com/r/TelegramChannels/)
* [r/TelegramGroups](https://www.reddit.com/r/TelegramGroups/)
* [Telegram Channels Exchange](https://smmacc.ru/shop/telegram.html)
* [CatalogTelegram](https://catalog-telegram.ru/)
* VK DB : [1](https://vk.com/topic-27339681_35246829) - [2](https://vk.com/topic-156599162_36469304) - [3](https://vk.com/topic-104630729_33036142) - [4](https://vk.com/topic-18200000_33478269) - [5](https://vk.com/topic-42713470_31758284) - [6](https://vk.com/topic-34185416_34307947) - [7](https://vk.com/topic-42281098_35740699) - [8](https://vk.com/topic-130067045_34430403)
* Chinese Directory : [1](https://zxfast.com/telegram_list.html) - [2](https://www.yuque.com/telegram/yxg3h6/tm) - [3](https://congcong0806.github.io/2018/04/24/Telegram/) - [4](https://www.newlearner.site/2018/10/19/telegram-group/channel/bot.html)

## [↑](#contents) Tools

* [Telegram Index](https://github.com/odysseusmax/tg-index)
* [Save Telegram Chat History](https://github.com/pigpagnet/save-telegram-chat-history)
* [TGViewer](https://github.com/TGViewer/TGViewer.github.io)
* [Telegram OSINT Library](https://github.com/Postuf/telegram-osint-lib)
* Telegram API for OSINT : [P1](https://fabledowlblog.wordpress.com/2017/07/10/telegram-api-for-osint-part-1-users/) - [P2](https://fabledowlblog.wordpress.com/2017/09/09/telegram-api-for-osint-part-2-messages/)
* [TelegramOnlineSpy](https://github.com/Forichok/TelegramOnlineSpy)
* [Genisys](https://github.com/Cryptonian007/Genisys)
* [Informer](https://github.com/paulpierre/informer)
* [TGCF](https://github.com/aahnik/tgcf)
* [Archive-Bot](https://github.com/Nukesor/archivebot)
* [Telescan](https://github.com/pielco11/telescan)
* [Telethon (For Creating Custom Tools)](https://github.com/LonamiWebs/Telethon)
* [Telegram Trilateration](https://github.com/jkctech/Telegram-Trilateration)
* [Telegram Nearby Map](https://github.com/tejado/telegram-nearby-map)

## [↑](#contents) Bots

* [TgScanRobot](https://tgdev.io/bot/tgscanrobot)
* [ChatSearchRobot](https://tgdev.io/bot/chatsearchrobot)
* [IDBot](https://t.me/username_to_id_bot)
* [UserInfoBot](https://t.me/userinfobot)
* [Account Creation Date Bot](https://t.me/creationdatebot)
* [Username History Bot](https://t.me/SangMataInfo_bot)
* [MotherSearch (Telegram Search Engine Bot)](https://t.me/MotherSearchBot)
* [Inv-Link Creator Finder](https://t.me/LinkCreatorBot)

## [↑](#contents) Resources

* [Leveraging Telegram for OSINT purposes](https://www.youtube.com/watch?v=e_aXQYq2l6U)
* [Telegram bot to find which groups the person is member of.](https://www.reddit.com/r/OSINT/comments/kvb5jd/telegram_bot_to_find_which_groups_the_person_is/)
* [Tactics for Telegram OSINT](https://widgets.figshare.com/articles/13655591/embed?show_title=1)
* [Telegram Network Visualization](https://medium.com/dataseries/telegram-network-visualization-tracing-forwards-and-mentions-f75746712fcf)
* [How to Get Data From Telegram Using Python](https://betterprogramming.pub/how-to-get-data-from-telegram-82af55268a4b)
* [Tips how to find private, hidden, personal groups and channels](https://telegra.ph/Tips-how-to-find-private-hidden-personal-groups-and-channels---TelegramPrivateChatLeaks-08-10)

