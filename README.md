
<div align="center">
<img width="125" height="125" src="https://github.com/gedoor/legado/raw/master/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png" alt="legado"/>  
  
Legado / 开源阅读
<br>
Legado is a free and open source novel reader for Android.
</div>

## legado-tts/阅读内置EdgeTTS 微软大声朗读
- app基于legado https://github.com/gedoor/legado ✅
- tts基于rany2/edge-tts https://github.com/rany2/edge-tts ✅
- 豆包tts 基于 https://github.com/callmerio/doubao-tts  ❌(未开发,简单测试能用, 我对豆包有执念,提上日程)

### 为什么会有这个仓库? 
- 我曾经提交过PR挂了几个星期也没人合并, So waht ever! 我=null, 我+GPT=无所不能
- 自己确实有这个需求,晚上不听几章睡不着 装了阅读再安装TTS有些多余,现有的TTS核心仍是rany2/edge-tts

### 书源
- 要么去喵公子导入, 要么本地, 不喜欢书源搜出来都是一对垃圾, 除非本地实在找不到才会用
- 本地电子书推荐: https://github.com/BlankRain/ebooks

### 主要修改
- 修改音频流的暂存方式 (写硬盘=>写内存)
- 原作者来是把音频缓存硬盘上会频繁执行写入和删除(有多少段落就写多少次),
- 频繁执行写入影响寿命或许对于现代存储来说影响微乎其微😋 但是我改成了放在内存中, 每读完一章就释放已读完的的媒体, 修改内容参见PR:gedoor/legado#5304
- 跟随rany2/edge-tts EdgeVersion 143.0.3650.75
- 不定时合并(gedoor/legado)主仓更新最近一次是在 2025-12-08
![detail.png](https://raw.githubusercontent.com/WangSunio/img/main/images/pre.png)

### happy every day 😄 😄