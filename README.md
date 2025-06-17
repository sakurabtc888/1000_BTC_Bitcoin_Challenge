## 1000 BTC Bitcoin Challenge

CPU模式：
![](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge/blob/main/1.png)

GPU模式：
![](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge/blob/main/2.png)

CPU模式碰撞成功：
![](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge/blob/main/3.png)

GPU模式碰撞成功：
![](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge/blob/main/4.png)

🔥 针对 [privatekeys.pw](https://privatekeys.pw/puzzles/bitcoin-puzzle-tx) 的CPU+GPU碰撞工具

在 2015 年，为了展示比特币私钥空间的巨大性及安全性，有人创建了一个“拼图”，他在某个较小的私钥范围中选择特定私钥，生成对应的比特币地址，并向每个特定地址发送越来越多的比特币。
为了解决这个难题，必须遍历特定私钥范围，并检查每个私钥的余额（或寻找到特定地址的私钥）。 私钥范围越小，找到特定私钥的机会就越大。

| 序号 | 私钥范围 | 正确私钥 | 比特币地址 | 比特币数量 |
| :----- | :----: | :----: | :----: | :----: |
| 1 | 1:1 | 0000000000000000000000000000000000000000000000000000000000000001 | 1BgGZ9tcN4rm9KBzDn7KprQz87SZ26SAMH | 0.001 BTC |
| 2 | 2:3 | 0000000000000000000000000000000000000000000000000000000000000003 | 1CUNEBjYrCn2y1SdiUMohaKUi4wpP326Lb | 0.002 BTC |
| 3 | 4:7 | 0000000000000000000000000000000000000000000000000000000000000007 | 19ZewH8Kk1PDbSNdJ97FP4EiCjTRaZMZQA | 0.003 BTC |
| ··· | ··· | ···  | ···  | ···  |
| 71 | 400000000000000000:7fffffffffffffffff | 待破解 | 1PWo3JeB9jrGwfHDNpdGK54CRas7fsVzXU | 7.1 BTC |
| 72 | 800000000000000000:ffffffffffffffffff | 待破解 | 1JTK7s9YVYywfm5XUH7RNhHJH1LshCaRFR | 7.2 BTC |
| 73 | 1000000000000000000:1ffffffffffffffffff | 待破解 | 12VVRNPi4SJqUTsp6FmqDqY5sGosDtysn4 | 7.3 BTC |
| ··· | ··· | ···  | ···  | ···  |
| 158 | 2000000000000000000000000000000000000000:3fffffffffffffffffffffffffffffffffffffff | 待破解 | 19z6waranEf8CcP8FqNgdwUe1QRxvUNKBG | 15.8 BTC |
| 159 | 4000000000000000000000000000000000000000:7fffffffffffffffffffffffffffffffffffffff | 待破解 | 14u4nA5sugaswb6SZgn5av2vuChdMnD9E5 | 15.9 BTC |
| 160 | 8000000000000000000000000000000000000000:ffffffffffffffffffffffffffffffffffffffff | 待破解 | 1NBC8uXJy1GiJ6drkiZa1WuKn51ps7EPTv | 16 BTC |

目前，剩余待破解比特币余额：916.5 BTC

<br>

要自动执行此过程，您可以使用本工具：
- 自动获取最新待破解比特币私钥范围
- CPU、GPU模式可选
- 碰撞全部160个地址
- 私钥范围内随机碰撞
- 碰撞成功发送邮件

<br>

如果该软件对您有所帮助，请点击：

[<img src="https://img.shields.io/github/followers/sakurabtc888?label=follow" height="20" title="Follow me" />](https://github.com/sakurabtc888)  与 [<img src="https://img.shields.io/github/stars/sakurabtc888/1000_BTC_Bitcoin_Challenge" height="20" title="stars" />](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge)

<br>

## 视频教程
📺[YouTube](https://youtu.be/gW9lsRLgQwk)    📺[哔哩哔哩](https://privatekeys.pw/puzzles/bitcoin-puzzle-tx)

<br>

## 碰撞速度参考
````bash
单地址、多地址模式：
CPU：
> i5-8600K    4.12  Mk/s
> i7-8700K    6.36  Mk/s
> i9-8950HK   13.56 Mk/s
> i5-9600KF   5.42  Mk/s
> i7-9700KF   9.90  Mk/s
> i9-9900KF   15.34 Mk/s
> i5-10600KF  12.60 Mk/s
> i7-10700KF  14.36 Mk/s
> i9-10900KF  16.00 Mk/s
> i5-11600KF  15.30 Mk/s
> i7-11700KF  16.22 Mk/s
> i9-11900KF  17.10 Mk/s
> i5-12600KF  18.36 Mk/s
> i7-12700KF  24.58 Mk/s
> i9-12900KF  27.36 Mk/s
> i5-13600KF  26.80 Mk/s
> i7-13700KF  30.60 Mk/s
> i9-13900KF  47.27 Mk/s
> i5-14600KF  30.75 Mk/s
> i7-14700KF  37.23 Mk/s
> i9-14900KF  48.61 Mk/s

GPU：
> GeForce GTX 1660 Ti   89.11   Mk/s
> GeForce RTX 2070      127.28  Mk/s
> GeForce RTX 2080 Ti   215.86  Mk/s
> GeForce RTX 3060 Ti   262.42  Mk/s
> GeForce RTX 3070 Ti   393.69  Mk/s
> GeForce RTX 3080 Ti   536.79  Mk/s
> GeForce RTX 3090 Ti   714.82  Mk/s
> GeForce RTX 4060      316.86  Mk/s
> GeForce RTX 4060 Ti   585.07  Mk/s
> GeForce RTX 4070      642.38  Mk/s
> GeForce RTX 4070 Ti   2060.93 Mk/s
> GeForce RTX 4080      1268.03 Mk/s
> GeForce RTX 4090 D    1970.12 Mk/s
> GeForce RTX 5060      514.33  Mk/s
> GeForce RTX 5060 Ti   670.66  Mk/s
> GeForce RTX 5070      865.23  Mk/s
> GeForce RTX 5070 Ti   1186.44 Mk/s
> GeForce RTX 5080      1522.51 Mk/s
> GeForce RTX 5090 D    2476.93 Mk/s

单公钥、多公钥模式速度为上述速度的4-10倍。
````

<br>

## BTC-ETH-EVM-LTC-TRX-Collision

收费软件Collision，针对BTC、ETH（EVM）、LTC、TRX链的私钥、公钥碰撞

[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=sakurabtc888&repo=BTC-ETH-EVM-LTC-TRX-Collision&theme=radical)](https://github.com/sakurabtc888/BTC-ETH-EVM-LTC-TRX-Collision)

<br>

## 接币圈软件定制
[![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=c++&link=https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)[![C#](https://img.shields.io/badge/C%23-239120.svg?style=flat&logo=c++&link=https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)[![Python](https://img.shields.io/badge/-Python-black?style=flat&logo=python&link=https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)[![Nodejs](https://img.shields.io/badge/-Nodejs-black?style=flat&logo=Node.js&link=https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E6%8E%A5%E5%B8%81%E5%9C%88%E8%BD%AF%E4%BB%B6%E5%AE%9A%E5%88%B6)

本人精通C++、C#、python、Nodejs的编程，接币圈软件定制，嘴严、技术好、效率高，可提供源码

<br>

## 与我联系
[![微信](https://img.shields.io/badge/%E5%BE%AE%E4%BF%A1-SakuraBtc-brightgreen?logo=wechat&link=https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E4%B8%8E%E6%88%91%E8%81%94%E7%B3%BB)](https://github.com/sakurabtc888/1000_BTC_Bitcoin_Challenge?tab=readme-ov-file#%E4%B8%8E%E6%88%91%E8%81%94%E7%B3%BB)

---
![](https://views.whatilearened.today/views/github/sakurabtc888/1000_BTC_Bitcoin_Challenge.svg)
