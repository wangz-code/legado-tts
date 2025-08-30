
<div align="center">
<img width="125" height="125" src="https://github.com/gedoor/legado/raw/master/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png" alt="legado"/>  
  
Legado / 开源阅读
<br>
Legado is a free and open source novel reader for Android.
</div>

## legado-tts/阅读内置EdgeTTS 微软大声朗读
基于legado https://github.com/gedoor/legado

### 主要修改
- 修改音频流的暂存方式 (写硬盘=>写内存)
- 原作者来是把音频缓存硬盘上会频繁执行写入和删除(有多少段落就写多少次),
- 频繁执行写入影响寿命或许对于现代存储来说影响微乎其微😋 但是我改成了放在内存中, 每读完一章就释放已读完的的媒体, 修改内容参见PR:gedoor/legado#5304
- 跟随rany2/edge-tts EdgeVersion 140.0.3485.14
![detail.png](https://raw.githubusercontent.com/WangSunio/img/main/images/pre.png)


### happy every day 😄 😄