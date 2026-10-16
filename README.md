<div align="center">

# Let Me Drive

**插上键盘，打开网页，就能调。**

键盘驱动的网页版。不用下载官方软件，用 Chrome 或 Edge 打开网页就能改键、录宏、调灯光，Mac 和 Windows 通用。

[打开 Let Me Drive](https://letmedrive.cn) · [已适配的键盘](https://letmedrive.cn/keyboards) · [提交适配需求](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml) · [反馈问题](https://github.com/tainanzhui/letmedrive/issues/new?template=bug.yml) · [English](README.en.md)

![Let Me Drive](.github/assets/screenshot.jpg)

</div>

## 为什么做这个

很多键盘的官方驱动只有 Windows 版；有的要装一个常驻后台的程序，只为了改一两个键；换一台电脑，又得重新找、重新装。

浏览器其实已经能直接和键盘对话了（WebHID）。所以我把这件事搬进了网页：插上键盘，打开 letmedrive.cn，选中它，就能调。改动直接写进键盘，换电脑也还在。

## 现在能做什么

- **改键**：点键盘图上的键，换成别的键、组合键、媒体键、鼠标键，或者一段宏。
- **宏**：录一串按键，绑到任意键上。
- **灯光**：灯效、颜色、亮度、速度，部分型号可以逐键上色。
- **磁轴**：触发行程、RT 快速触发、高级键，按型号开放。
- **按键测试**：热力图、连击检测，看看每个键是不是好的。
- **演示模式**：手边没有键盘，也可以先点一点试试。

## 支持哪些键盘

已覆盖 195 个品牌、3,800 多款型号，包括 Keychron、Royal Kludge、黑爵 AJAZZ、狼蛛 Aula、Akko / MonsGeek、达尔优、迈从 MCHOSE、NuPhy、Wooting、DrunkDeer、雷蛇、罗技、海盗船、赛睿、华硕 ROG、魔力鸭、燃风 REALFORCE，以及 QMK / VIA 键盘。

完整列表在 [letmedrive.cn/keyboards](https://letmedrive.cn/keyboards)。每款能调的项目，以连接后页面上显示的为准。

## 怎么用

1. 用数据线把键盘接到电脑。部分型号也支持无线接收器。
2. 用电脑上的 **Chrome** 或 **Edge** 打开 [letmedrive.cn](https://letmedrive.cn)。
3. 点「连接键盘」，在弹窗里选你的键盘，网页会自动认出型号。

## 隐私

所有设置都在你的浏览器里完成，直接写进键盘。键盘配置不会上传，也不需要注册账号。

## 已知限制

- 需要 Chrome 或 Edge 桌面版。Safari、Firefox 和手机浏览器不支持 WebHID。
- 有些型号标着「实验性」，功能还在补全；遇到不对的地方，欢迎反馈。
- 部分无线键盘只能在有线或接收器模式下调。

## 反馈

- **没找到你的键盘**：[提交适配需求](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml)，写上型号；能附上连接后页面里的「设备信息」最好。
- **某个功能不对**：[反馈问题](https://github.com/tainanzhui/letmedrive/issues/new?template=bug.yml)，写清型号、做了什么、看到了什么。

## 说明

Let Me Drive 是个人项目，与任何键盘厂商无关，文中提到的品牌和商标归各自所有。修改键盘设置有一定风险；遇到问题，可以在官方驱动或键盘自带的组合键里恢复出厂设置。

本仓库用于发布和收集反馈，源码暂不公开。
