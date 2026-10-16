<div align="center">

# Let Me Drive

**The web keyboard driver collection. Stop installing keyboard drivers.**

I reverse-engineered the official Windows drivers of 200+ keyboards and rebuilt every brand, model and setting they support — down to what each individual key can be remapped to — as a single web page.<br>
Open it, tune your keyboard, and the change is written to the keyboard instantly. Same on Windows and macOS.

[**Open letmedrive.cn**](https://letmedrive.cn) · [Supported keyboards](https://letmedrive.cn/keyboards) · [Request a keyboard](https://github.com/tainanzhui/letmedrive/issues/new?template=support-request.yml) · [Report a problem](https://github.com/tainanzhui/letmedrive/issues/new?template=bug.yml) · [中文](README.md)

![Let Me Drive](.github/assets/screenshot.jpg)

</div>

## What it is

Every keyboard brand ships its own driver. Most are Windows-only, keep a service running in the background, and need reinstalling for every new keyboard and every new computer. On a Mac, many keyboards have no driver at all.

Let Me Drive moves all of that into the browser. Each of those 200+ official drivers was reverse-engineered to learn exactly what every model can do, and every setting was rebuilt so it works straight from a web page, applies live and is saved to the keyboard.

- **Nothing to install**: open [letmedrive.cn](https://letmedrive.cn) in Chrome or Edge
- **Windows and macOS**: keyboards that only had a Windows driver now work on a Mac too
- **Saved on the keyboard**: settings stay after you unplug it or move to another computer
- **Local only**: nothing is uploaded, no account needed

## Features

### Remapping
Click any key on the on-screen keyboard and turn it into another key, a shortcut, a media or mouse button, a layer switch or a macro, with separate layers such as Fn. Each keyboard only offers the options its firmware accepts.

![Remapping](.github/assets/remap.jpg)

### Macros
Record a macro by typing it, or edit it step by step — press, release, tap and precise delays. Macros live in the keyboard's slots and can be exported as files.

![Macros](.github/assets/macro.jpg)

### Lighting
Every built-in effect of the keyboard, plus colour, brightness and speed. Per-key colour on models that support it.

![Lighting](.github/assets/lighting.jpg)

### Hall-effect keyboards
Per-key actuation point, rapid trigger and its press / release sensitivity. The current actuation is shown on each keycap; ⚡ marks rapid trigger.

![Hall effect](.github/assets/magnetic.jpg)

### Advanced keys and onboard settings
Depending on the model: dynamic keystrokes (DKS), tap / hold actions, toggle keys, polling rate, debounce, sleep timer, Win-key lock and more.

### Key tester
Works without connecting: type to find dead keys, with a heat map and chatter detection.

![Key tester](.github/assets/tester.png)

### Backups
See every remapped key in one list, restore any of them or everything, and export / import full profiles.

## Supported keyboards

195 brands, 35 protocol families, 3,800+ models; 3,819 of them pass a full write → read-back check against simulated firmware. Including Keychron, Royal Kludge, AJAZZ, Aula, Akko / MonsGeek, Dareu, MCHOSE, NuPhy, Epomaker, Wooting, DrunkDeer, Dygma, 8BitDo, Razer, Logitech, Corsair, SteelSeries, ASUS ROG, HyperX, Cooler Master, Ducky, REALFORCE, ROCCAT, Mountain, Glorious and QMK / VIA / Vial boards. Full list: [letmedrive.cn/keyboards](https://letmedrive.cn/keyboards).

## How to use

1. Connect the keyboard with a cable (some models also work over their 2.4 GHz receiver).
2. Open [letmedrive.cn](https://letmedrive.cn) in desktop **Chrome** or **Edge**.
3. Click **Connect** and pick your keyboard; the model is detected automatically.

No keyboard at hand? Try the demo on the home page.

## FAQ

**Do I really not need any driver?** No. The browser talks to the keyboard directly over WebHID — the web page is the driver.
**Does it work on a Mac?** Yes, in Chrome or Edge. Safari and Firefox don't support WebHID.
**Will my settings be lost?** No, they're written to the keyboard.
**Can it break my keyboard?** It only writes settings the official driver can change. If things get messed up, use "restore all defaults", the vendor tool, or the keyboard's own factory-reset combo.

## Limitations

Desktop Chrome or Edge only. Some wireless keyboards can only be configured when wired or on their receiver (not over Bluetooth). Models marked "experimental" are still being completed.

## About

Let Me Drive is a personal project and is not affiliated with any keyboard manufacturer; all trademarks belong to their owners. Changing keyboard settings carries some risk.
