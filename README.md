# Notion Widgets With [vercel](https://vercel.com/)
## 1. Music Player
> Based on [Aplayer](https://github.com/MoePlayer/APlayer) & [MetingJS](https://github.com/metowolf/MetingJS)

![](./img/1.png)
Just use https://simple-notion-widgets.vercel.app/music-player?auto=https://y.qq.com/n/yqq/playlist/7888484143.html

### Quick Start
> You must use [QQ Music](https://y.qq.com/) or [NetEase Cloud Music](https://music.163.com/) on Web to get the URL.  Using QQ music may be easier.
- https://music.163.com/#/song?id=28754103
  - https://simple-notion-widgets.vercel.app/music-player?server=netease&type=song&id=28754103
- https://music.163.com/#/playlist?id=60198
  - https://simple-notion-widgets.vercel.app/music-player?server=netease&type=playlist&id=60198
- https://y.qq.com/n/yqq/song/001RGrEX3ija5X.html
  - https://simple-notion-widgets.vercel.app/music-player?auto=https://y.qq.com/n/yqq/song/001RGrEX3ija5X.html
- https://y.qq.com/n/yqq/playlist/7888484143.html
  - https://simple-notion-widgets.vercel.app/music-player?auto=https://y.qq.com/n/yqq/playlist/7888484143.html
- If you want to use paid songs, you may need to find resources yourself. **Any links are not allowed to appear \ and &**, otherwise you need to use shortening link services, such as [suowo.cn](https://suowo.cn/).
  - https://simple-notion-widgets.vercel.app/music-player?name=rainymood&artist=rainymood&url=https://rainymood.com/audio1110/0.m4a&cover=https://rainymood.com/i/badge.jpg

### Option

|option               |default      |description|
|--------------------|------------|----------|
|id              |**require**   |song id / playlist id / album id / search keyword|
|server          |**require**   |music platform: `netease`, `tencent`, `kugou`, `baidu`|
|type            |**require**   |`song`, `playlist`, `album`, `search`, `artist`|
|auto            |options       |music link, support: `tencent`|
|fixed           |`false`       |enable fixed mode|
|mini            |`false`       |enable mini mode|
|autoplay        |`false`       |audio autoplay|
|theme           |`#2980b9`     |main color|
|loop            |`all`         |player loop play, values: 'all', 'one', 'none'|
|order           |`list`        |player play order, values: 'list', 'random'|
|preload         |`auto`        |values: 'none', 'metadata', 'auto'|
|volume          |`0.7`         |default volume, notice that player will remember user setting, default volume will not work after user set volume themselves|
|mutex           |`true`        |prevent to play multiple player at the same time, pause other players when this player start play|
|lrc-type         |`0`           |lyric type|
|list-folded      |`false`       |indicate whether list should folded at first|
|list-max-height   |`340px`       |list max height|
|storage-name     |`metingjs`    |localStorage key that store player setting|

## 2. Video Player
> Based on [Dplayer](https://github.com/MoePlayer/DPlayer)
Not very useful for now.