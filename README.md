# APCC HT

> **APCC HT 是骑行台控制程序，不会记录或保存训练。如需记录训练，请自己打开码表（或其他记录设备）。**
>
> **APCC HT is a trainer control app. It does not record or save your rides — start your own bike computer (or other recording device) to record the workout.**
>
> **APCC HT est une application de pilotage du home trainer. Elle n’enregistre pas vos séances : lancez votre propre compteur (ou un autre appareil) pour enregistrer l’entraînement.**

由 Vincuri 设计开发

Designed & developed by Vincuri

Conçu et développé par Vincuri

APCC HT 是 APCC（Asian Paris Cycling Club）的骑行台控制程序，用于通过蓝牙 FTMS 连接智能骑行台（例如 Zwift Hub）。本仓库只发布安装包，**不包含源代码**。

APCC HT is a smart-trainer control app by APCC (Asian Paris Cycling Club). It connects to a trainer over Bluetooth FTMS (for example a Zwift Hub). This repository publishes installers only. **Source code is not in this repo.**

APCC HT est l’application de pilotage de home trainer d’APCC (Asian Paris Cycling Club). Elle se connecte à un home trainer en Bluetooth FTMS (par exemple un Zwift Hub). Ce dépôt ne publie que les installeurs. **Le code source n’est pas dans ce dépôt.**

## 下载 / Downloads / Téléchargements

当前版本 1.6.3（最新）。以下链接始终指向最新正式版：

| 平台 | 文件 | 链接 |
| --- | --- | --- |
| macOS（Apple 芯片） | `APCC-HT-mac-arm64.dmg` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-mac-arm64.dmg |
| Windows | `APCC-HT-windows-setup.exe` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-windows-setup.exe |
| Android | `APCC-HT-android.apk` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-android.apk |

校验和：https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/SHA256SUMS.txt

Release 1.6.3 (latest). These links always point at the latest release:

| Platform | File | Link |
| --- | --- | --- |
| macOS (Apple silicon) | `APCC-HT-mac-arm64.dmg` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-mac-arm64.dmg |
| Windows | `APCC-HT-windows-setup.exe` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-windows-setup.exe |
| Android | `APCC-HT-android.apk` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-android.apk |

Checksums: https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/SHA256SUMS.txt

Version 1.6.3 (dernière). Ces liens pointent toujours vers la dernière version :

| Plateforme | Fichier | Lien |
| --- | --- | --- |
| macOS (Apple silicon) | `APCC-HT-mac-arm64.dmg` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-mac-arm64.dmg |
| Windows | `APCC-HT-windows-setup.exe` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-windows-setup.exe |
| Android | `APCC-HT-android.apk` | https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/APCC-HT-android.apk |

Sommes de contrôle : https://github.com/Vincuri/APCC-HT-Releases/releases/latest/download/SHA256SUMS.txt

## 程序介绍

APCC HT 通过蓝牙 FTMS 连接智能骑行台（例如 Zwift Hub），用 ERG 模式按目标功率带动骑行。内置约 3000 节结构化课程，可以选配蓝牙功率计，每节训练结束后给出总结。App 里还可以用「自定义」自己编排课程（热身、固定功率、渐变、间歇重复、自由骑、放松），并导出为 .zwo 文件；浏览器版本没有自定义功能。提供 Android、Mac（Apple 芯片）和 Windows 安装包，另有浏览器版本。

它只负责控制骑行台。训练记录请用自己的码表或其他记录设备。

## What it does

APCC HT connects to a smart trainer over Bluetooth FTMS (for example a Zwift Hub) and drives it in ERG mode at a target wattage. It includes a built-in library of about 3000 structured workouts, an optional Bluetooth power meter, and a summary after each workout. In the apps you can also build your own workouts with the custom builder (warm-up, steady, ramp, intervals, free ride, cool-down) and export them as .zwo files; the browser version has no builder. Installers are published for Android, Mac (Apple silicon), and Windows. A browser version is also available.

It controls the trainer. It does not record the ride.

## Présentation

APCC HT se connecte à un home trainer intelligent en Bluetooth FTMS (par exemple un Zwift Hub) et le pilote en mode ERG à une puissance cible. La bibliothèque intégrée compte environ 3000 séances structurées. Un capteur de puissance Bluetooth est facultatif, et un résumé s’affiche à la fin de chaque séance. Dans les applications, la « Séance perso » permet de composer vos propres séances (échauffement, puissance fixe, rampe, intervalles, sortie libre, retour au calme) et de les exporter en .zwo ; la version navigateur ne la propose pas. Des installeurs sont publiés pour Android, Mac (Apple silicon) et Windows. Une version navigateur existe aussi.

L’application pilote le home trainer. Elle n’enregistre pas la séance.

## 安装说明

**Mac（仅 Apple 芯片）。** 把 `APCC HT.app` 拖进「应用程序」之后，在终端执行：

```bash
xattr -dr com.apple.quarantine "/Applications/APCC HT.app"
```

**Windows。** 若 SmartScreen 拦截，选择「更多信息」，再选择「仍要运行」。

**Android。** 允许安装未知来源的应用。新版本会覆盖安装到已有的 APCC HT 上。

## Install notes

**Mac (Apple silicon only).** After dragging `APCC HT.app` into Applications, run this in Terminal:

```bash
xattr -dr com.apple.quarantine "/Applications/APCC HT.app"
```

**Windows.** If SmartScreen blocks the installer, choose More info, then Run anyway.

**Android.** Allow installs from unknown sources. The new package installs over an older version of APCC HT.

## Installation

**Mac (Apple silicon uniquement).** Après avoir glissé `APCC HT.app` dans Applications, exécutez dans le Terminal :

```bash
xattr -dr com.apple.quarantine "/Applications/APCC HT.app"
```

**Windows.** Si SmartScreen bloque l’installeur : Informations complémentaires, puis Exécuter quand même.

**Android.** Autorisez les sources inconnues. La nouvelle version s’installe par-dessus l’ancienne.

## 源代码 / Source code / Code source

本仓库没有源代码，只有发布说明和安装包下载。

This repository does not contain source code. It only holds release notes and installer downloads.

Ce dépôt ne contient pas le code source. Il ne contient que les notes de version et les installeurs.

由 Vincuri 设计开发

Designed & developed by Vincuri

Conçu et développé par Vincuri

APCC on Strava: https://www.strava.com/clubs/2347321
