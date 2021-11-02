# banana

---

## docs

- https://voicemeeter.com/user-guides/
- https://vb-audio.com/Voicemeeter/Voicemeeter_UserManual.pdf
- https://vb-audio.com/Voicemeeter/VoicemeeterBanana_UserManual.pdf

### 教程

[**骑士豆豆君** -- VoiceMeeter入门到精通](https://space.bilibili.com/177930661/channel/detail?cid=91045&ctype=0)

## brief

https://vb-audio.com/Voicemeeter/banana.htm

### input

将所有东西连接在一起的通用虚拟音频设备

![input](https://vb-audio.com/Voicemeeter/VoicemeeterBananaConnectivity.gif)

### 虚拟 I/O & output

所有音频接口支持：MME、Direct-X、KS、WaveRT、WASAPI 和 ASIO

![虚拟IO](https://vb-audio.com/Voicemeeter/VoicemeeterBananaUniversalAudioDevice.jpg)



### 规格

官网有规格清单

![](https://vb-audio.com/Voicemeeter/VoicemeeterBananaConnectionDiagram.gif)



## 声卡

### 板载声卡

REALTEK ALC1220-VB 支持ASIO



## 声卡驱动

ASIO最牛逼，然后是WDM，MME最垃圾

ASIO需要专业的声卡才支持

### MME

MME（MultiMedia Extensions）：级别最低的驱动，于Windows 3.1时代首次推出。由于等待时间长，Cubase VST、Logic Audo等音序软件应避免使用，除非找不到替换者。然而它在Cakewalk Sonar中使用似乎有着优良的性能，一些独立的软件合成器使用时MME也具有相当好的性能。

### WDM

WDM（Win32 Driver Model）：Microsoft的最新类型驱动，最先作为Windows 98 SE的选项（当时有一些问题，少数厂家因此推出自己的驱动），它们能够成功地运行于Windows ME，当然意义更为重大的是对于Windows 2000和XP的用户。它们提供比MME或DirectSound驱动低得多的等待（某些情况下可以达到惊人的1.5毫秒）。它们往往比操作系统迟一些推出，以后有些好转。如果在Windows 2000和XP下运行Sonar，WDM是必须的。

### ASIO (专业声卡驱动)

ASIO（Audio Stream Input Output）：音频流输入输出，通过Steinberg流行的的MIDI加音频软件Cubase VST走向世界，是第一个真正提供了小于10毫秒低等待时间的驱动。ASIO2.0同时支持多口（通过ADAT传送）采样精度的寻址和零等待的监听。如果你的音序器和声卡二者都支持ASIO，考虑优先使用它。



## 混音 

多声道输入输出路由



## banana 自带调音

### 输入

#### INTELLPAN

#### 效果器

##### 压缩 

##### 门限



### 输出

#### MASTER SECTION

##### Nomal mode

输出模式

##### EQ



##### mono

多声道合并成单声道

##### Solo

开启Solo相当于独奏，屏蔽其他声道的声音。

##### Mute

静音

---

## 软件机架调音

- 专业硬件声卡 + ASIO专业声卡驱动
- voicemeeter虚拟ASIO驱动

