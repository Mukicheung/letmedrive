<div align="center">

# 网页键盘驱动大合集

**Let Me Drive · 从今天开始，不用再下载任何键盘驱动。**

我逆向了 200 多款键盘的官方 Windows 驱动，把它们支持的品牌、型号和每一项功能，全部做进了一个网页。<br>
打开网页就能调，改动实时生效、直接写进键盘。Windows 和 Mac 都一样。

[**打开网页 → letmedrive.cn**](https://letmedrive.cn) · [已适配的键盘](https://letmedrive.cn/keyboards) · [提交适配需求](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml) · [反馈问题](https://github.com/tainanzhui/letmedrive/issues/new?template=bug.yml) · [English](README.en.md)

![网页键盘驱动大合集](.github/assets/screenshot.jpg)

</div>

## 这是什么

每个键盘品牌都有自己的驱动：大多只有 Windows 版，装完常驻后台；换一把键盘要再装一个，换一台电脑又要重新装一遍。Mac 用户更难，很多键盘根本没有 Mac 版驱动。

网页键盘驱动大合集把这些驱动做的事，统一搬进了浏览器。我逐个逆向了 200 多款官方 Windows 驱动，弄清每个品牌、每个型号能调什么，包括**每一个键能改成什么**，再把所有调整都做成网页里能直接操作、实时生效、写入键盘的方式。

一个网页，替代一抽屉的驱动。

- **不用下载、不用安装**：Chrome 或 Edge 打开 [letmedrive.cn](https://letmedrive.cn) 就能用
- **Windows、Mac 通用**：原本只有 Windows 驱动的键盘，在 Mac 上也能调
- **写进键盘**：改完保存在键盘里，拔掉、换电脑、不开网页都还在
- **本地完成**：配置不上传，不用注册账号

## 能调什么

### 改键

点键盘图上任意一个键，把它换成别的键、组合键、媒体键、鼠标按键、层切换或者一段宏。支持多层（比如 Fn 层）分开设置。每把键盘只显示它固件认的选项，不会让你选了再报错。

![改键](.github/assets/remap.jpg)

### 宏

点「录制」直接在键盘上按一遍，或者一步步手动编辑：按下、松开、单击、延时都可以精确调整。宏写进键盘的槽位，再到「改键」里绑到任意键上；也能导出成文件备份。

![宏](.github/assets/macro.jpg)

### 灯光

灯效、颜色、亮度、速度，按键盘自带的全部灯效列出来，一眼就能换。支持逐键灯光的型号，可以给每个键单独上色。

![灯光](.github/assets/lighting.jpg)

### 磁轴

磁轴键盘的每个键都能单独设置触发行程，开关 RT 快速触发、调按下和抬起的灵敏度。键帽上直接显示当前行程，⚡ 表示已开快速触发。

![磁轴](.github/assets/magnetic.jpg)

### 高级键与板载设置

按型号开放：一键多指令（DKS）、长按 / 轻按不同功能、切换键，以及回报率、按键防抖、休眠时间、Win 键锁等键盘自身的设置。

### 按键测试

不连驱动也能用：敲一遍就知道哪个键坏了。热力图显示每个键按了多少次，还能检测连击（一次按下被识别成多次）。

![按键测试](.github/assets/tester.png)

### 配置备份

改过的键会列在一起，可以单个还原、全部恢复默认，也能把整套配置导出成文件，换一把同款键盘再导入。

## 支持哪些键盘

目前覆盖 **195 个品牌、35 类协议、3,800 多款型号**，其中 3,819 款的全部功能都已在模拟设备上逐项「写入 → 读回」核验。

- **键盘品牌**：Keychron、Royal Kludge、黑爵 AJAZZ、狼蛛 Aula、Akko / MonsGeek、达尔优、迈从 MCHOSE、腹灵、VGN、NuPhy、Epomaker、新盟、珂芝、杜伽、阿米洛、ATK、Wooting、DrunkDeer、Dygma、8BitDo……
- **外设大厂**：雷蛇 Razer、罗技 Logitech、海盗船 Corsair、赛睿 SteelSeries、华硕 ROG、HyperX、酷冷至尊、魔力鸭 Ducky、燃风 REALFORCE、冰豹 ROCCAT、山峦 Mountain、Glorious、雷神、机械师……
- **开源固件**：QMK / VIA / Vial 键盘

完整型号列表：[letmedrive.cn/keyboards](https://letmedrive.cn/keyboards)。每款能调的项目以连接后页面上显示的为准；标着「实验性」的型号还在补全。

## 怎么用

1. 用数据线把键盘接到电脑（部分型号也支持 2.4G 接收器）。
2. 用电脑上的 **Chrome** 或 **Edge** 打开 [letmedrive.cn](https://letmedrive.cn)。
3. 点「连接键盘」，在弹窗里选中你的键盘。网页会自动认出型号，切到你想调的功能就行。

手边没有键盘，也可以在首页点「先看演示」，用模拟键盘把所有功能点一遍。

## 常见问题

**真的不用装任何驱动吗？**
不用。浏览器通过 WebHID 直接和键盘通信，网页就是驱动。

**Mac 能用吗？**
能。Mac 上用 Chrome 或 Edge，和 Windows 完全一样。Safari、Firefox 不支持 WebHID。

**改完会不会丢？**
不会。改动直接写进键盘，关掉网页、换电脑都还在。

**会不会把键盘改坏？**
只会写入官方驱动本来就能改的设置。真的调乱了，可以在网页里「恢复全部默认」，或者用官方驱动、键盘自带的组合键恢复出厂设置。

**我的键盘不在列表里怎么办？**
[提交适配需求](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml)，写上型号；连接后页面里的「设备信息」能帮我更快适配。

## 已知限制

- 需要电脑上的 Chrome 或 Edge；手机浏览器、Safari、Firefox 不支持。
- 部分无线键盘只能在有线或接收器模式下调，蓝牙模式下浏览器连不上。
- 少数型号标着「实验性」，部分功能还在补全。

## 反馈

- **没找到你的键盘**：[提交适配需求](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml)
- **某个功能不对**：[反馈问题](https://github.com/tainanzhui/letmedrive/issues/new?template=bug.yml)，写清型号、做了什么、看到了什么

## 说明

网页键盘驱动大合集（Let Me Drive）是个人项目，与任何键盘厂商无关，文中提到的品牌和商标归各自所有。修改键盘设置有一定风险，请自行判断。
