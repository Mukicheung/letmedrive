<div align="center">

# Let Me Drive

### A keyboard configurator in your browser

Remap keys, record macros, adjust lighting and configure Hall-effect switches.

[简体中文](README.md) · **English**

[Open the app](https://letmedrive.cn) · [Find your keyboard](https://letmedrive.cn/keyboards) · [User guide](docs/guide.en.md) · [Report an issue](https://github.com/MukiCheung/letmedrive/issues/new?template=bug-en.yml)

![Windows / macOS](https://img.shields.io/badge/platform-Windows%20%2F%20macOS-24292f?style=flat-square)
![Chrome / Edge](https://img.shields.io/badge/browser-Chrome%20%2F%20Edge-24292f?style=flat-square)
![WebHID](https://img.shields.io/badge/connection-WebHID-24292f?style=flat-square)

![Let Me Drive keyboard configuration interface](.github/assets/screenshot.jpg)

</div>

[Quick start](#quick-start) · [Features](#features) · [Compatibility](#compatibility) · [FAQ](#faq) · [Feedback](#feedback)

## About

Let Me Drive brings configuration tools for multiple keyboard brands into one browser interface. Supported keyboards can connect through Chrome or Edge on Windows and macOS, without installing a separate desktop client for this project.

The app communicates with the keyboard over WebHID. Available controls and save behavior depend on the model and firmware.

**This repository contains product information, documentation and issue tracking. The app is currently free to use. Its application source code is not published in this repository.**

## Quick start

1. **Check your model** in the [keyboard directory](https://letmedrive.cn/keyboards), including its supported connection modes.
2. **Connect the keyboard**, preferably with a USB data cable. Receiver support varies by model.
3. **Open [letmedrive.cn](https://letmedrive.cn)** in desktop Chrome or Edge.
4. **Grant device access** using the connect button and select your keyboard in the browser dialog.
5. **Make a small change**, follow the save instructions and verify the result on the device.

No keyboard nearby? Open the demo from the home page to explore the interface.

[Connection, saving and troubleshooting guide →](docs/guide.en.md)

## Features

These are the available feature categories. Each keyboard exposes the controls supported by its hardware and firmware.

<table>
<tr>
<td width="50%">
<h3>Remapping & layers</h3>
<p>Select keys on the keyboard layout and assign keys, shortcuts, media controls, mouse actions or layer switches.</p>
<img src=".github/assets/remap.jpg" alt="Key remapping and layers">
</td>
<td width="50%">
<h3>Macro recording & editing</h3>
<p>Record input, edit press/release events and delays, then assign the macro to a key. Export macros for backup.</p>
<img src=".github/assets/macro.jpg" alt="Macro recording and event editor">
</td>
</tr>
<tr>
<td>
<h3>Lighting</h3>
<p>Adjust effects, colors, brightness and speed. Per-key color is available on supported models.</p>
<img src=".github/assets/lighting.jpg" alt="RGB lighting controls">
</td>
<td>
<h3>Hall effect & rapid trigger</h3>
<p>Set actuation distance, rapid trigger and press/release sensitivity on supported Hall-effect keyboards.</p>
<img src=".github/assets/magnetic.jpg" alt="Hall-effect actuation and rapid trigger controls">
</td>
</tr>
</table>

| Feature | Purpose |
| --- | --- |
| Advanced keys | Configure DKS, tap/hold actions and toggle behavior on supported models |
| Onboard settings | Adjust available polling rate, debounce, sleep timer and Win-key lock controls |
| Profile backup | Export configurations; check model and format compatibility before importing |
| Key tester | Inspect key response, press counts and chatter detection results |

<details>
<summary>View the key tester</summary>

![Key tester and heat map](.github/assets/tester.png)

</details>

## Compatibility

| Environment | Notes |
| --- | --- |
| Windows / macOS | Use desktop Chrome or Edge |
| Safari / Firefox / mobile browsers | Not supported environments for the configurator |
| USB wired | Recommended starting point |
| 2.4 GHz receiver | Depends on the keyboard and receiver protocol |
| Bluetooth | Configuration support is not guaranteed; prefer wired mode |

The directory includes models from Keychron, Royal Kludge, AJAZZ, Aula, Akko / MonsGeek, NuPhy, MCHOSE, Wooting, DrunkDeer, Dygma and 8BitDo, plus some QMK / VIA / Vial keyboards. **A listed brand does not imply support for every model, and firmware revisions can differ.**

Check the exact entry in the [live directory](https://letmedrive.cn/keyboards) and the controls shown after connection. Entries marked experimental are still being developed.

### Validation scope

Simulated-device write/read-back checks validate protocol handling. Physical-device behavior also depends on firmware, connection mode and hardware responses. Passing simulation does not establish complete physical-device validation for a model. Include model and firmware details when reporting differences.

## FAQ

<details>
<summary><strong>Is this a driver or a web app?</strong></summary>

It is a web configuration tool. Normal keyboard input is handled by the operating system's HID support. The app reads and changes supported device settings; it does not replace the operating system driver.

</details>

<details>
<summary><strong>Do settings remain after I close the page?</strong></summary>

Settings with onboard persistence can be saved on the keyboard. Save behavior varies by model. Follow the app's write instructions and reconnect to verify. Export important configurations first.

</details>

<details>
<summary><strong>Why is my keyboard missing from the device dialog?</strong></summary>

Use Chrome or Edge, check that the cable supports data, switch to wired mode and close vendor configuration tools that may be using the device. See the [troubleshooting guide](docs/guide.en.md#connection-troubleshooting).

</details>

<details>
<summary><strong>What if my model is missing or a feature behaves incorrectly?</strong></summary>

[Request support](https://github.com/MukiCheung/letmedrive/issues/new?template=support-request-en.yml) for a missing model, or [report an issue](https://github.com/MukiCheung/letmedrive/issues/new?template=bug-en.yml) for unexpected behavior. Include the full model name, OS, browser, connection mode and reproduction steps.

</details>

## Feedback

- [Report a bug](https://github.com/MukiCheung/letmedrive/issues/new?template=bug-en.yml): include steps, expected behavior and actual results.
- [Request keyboard support](https://github.com/MukiCheung/letmedrive/issues/new?template=support-request-en.yml): include the full model and official product or configuration-tool links.
- [Improve the docs](CONTRIBUTING.md): corrections, translations and notes verified on real hardware are welcome.

Maintained by [Muki Cheung](https://github.com/MukiCheung). This project is not affiliated with the keyboard manufacturers mentioned. All brands and trademarks belong to their respective owners.
