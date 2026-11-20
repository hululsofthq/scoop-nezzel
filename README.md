<div align="center">

<img src="https://raw.githubusercontent.com/hululsofthq/nezzel-desktop/main/src-tauri/icons/128x128@2x.png" width="96" height="96" alt="Nezzel icon">

# Nezzel for Windows, with Scoop

**One command to install. One command to update. No warning screen.**

The [Scoop](https://scoop.sh) bucket for [Nezzel Desktop](https://github.com/hululsofthq/nezzel-desktop),<br>
the free, open-source app that saves videos, audio and photos from links.

[![Scoop version](https://img.shields.io/scoop/v/nezzel?bucket=https%3A%2F%2Fgithub.com%2Fhululsofthq%2Fscoop-nezzel&style=flat-square&color=006B5E&label=scoop)](bucket/nezzel.json)
[![Install test](https://img.shields.io/github/actions/workflow/status/hululsofthq/scoop-nezzel/install-test.yml?branch=main&style=flat-square&label=install%20test)](https://github.com/hululsofthq/scoop-nezzel/actions/workflows/install-test.yml)
[![Tests](https://img.shields.io/github/actions/workflow/status/hululsofthq/scoop-nezzel/ci.yml?branch=main&style=flat-square&label=tests)](https://github.com/hululsofthq/scoop-nezzel/actions/workflows/ci.yml)
[![Auto-update](https://img.shields.io/github/actions/workflow/status/hululsofthq/scoop-nezzel/excavator.yml?branch=main&style=flat-square&label=auto-update)](https://github.com/hululsofthq/scoop-nezzel/actions/workflows/excavator.yml)

[Nezzel Desktop](https://github.com/hululsofthq/nezzel-desktop) · [Website](https://nezzel.hululsoft.mr/desktop/) · [العربية](#بالعربية) · [Français](#en-français)

<img src="https://raw.githubusercontent.com/hululsofthq/nezzel-desktop/main/.github/assets/demo-quickbar.gif" width="528" alt="Nezzel's quick bar opens over another app, reads a copied YouTube link and offers best quality, audio only or 720p">

</div>

## Install

In PowerShell:

```pwsh
scoop bucket add nezzel https://github.com/hululsofthq/scoop-nezzel
scoop install nezzel/nezzel
```

Then open **Nezzel** from the Start menu, or type `nezzel`.

New to Scoop? It is a command-line installer for Windows. Set it up once, as described on [scoop.sh](https://scoop.sh):

```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## Why install this way

- **No "Windows protected your PC" screen.** Nezzel's installer is not signed with a paid certificate yet, so a normal download shows that warning. A Scoop install does not; the [install test](https://github.com/hululsofthq/scoop-nezzel/actions/workflows/install-test.yml) checks this on a clean Windows machine.
- **Checked download.** Scoop compares the file with the checksum published with each Nezzel release before it installs anything.
- **No administrator rights.** Everything goes into your own Scoop folder.

## Update and remove

```pwsh
scoop update nezzel        # get the newest version
scoop uninstall nezzel     # remove the app, keep your settings
scoop uninstall -p nezzel  # remove the app and your settings
```

This bucket looks for a new Nezzel release every four hours and updates itself, so `scoop update nezzel` gives you the new version soon after it is published.

## What you get

| | |
|---|---|
| Build | The portable build of Nezzel Desktop, for 64-bit Intel/AMD and ARM64 Windows |
| Shortcuts | A **Nezzel** entry in the Start menu and a `nezzel` command |
| Settings | Kept in Scoop's `persist` folder, so they survive updates |
| Source | The same files as on the [releases page](https://github.com/hululsofthq/nezzel-desktop/releases/latest) |

Prefer a normal installer, or use macOS or Linux? See [Nezzel Desktop](https://github.com/hululsofthq/nezzel-desktop#install).

## Help

- A problem with the app itself: [Nezzel Desktop issues](https://github.com/hululsofthq/nezzel-desktop/issues).
- A problem with installing or updating through Scoop: [issues here](https://github.com/hululsofthq/scoop-nezzel/issues).

## بالعربية

<div dir="rtl">

هذا المستودع يتيح تثبيت Nezzel على Windows بأمر واحد عبر <a href="https://scoop.sh">Scoop</a>، ومن دون شاشة التحذير الزرقاء التي تظهر عند تنزيل المثبّت العادي.

</div>

```pwsh
scoop bucket add nezzel https://github.com/hululsofthq/scoop-nezzel
scoop install nezzel/nezzel
```

<div dir="rtl">

للتحديث: <code>scoop update nezzel</code>. تبقى إعداداتك محفوظة بين التحديثات. لمعرفة المزيد عن التطبيق: <a href="https://github.com/hululsofthq/nezzel-desktop#بالعربية">Nezzel Desktop</a>.

</div>

## En français

Ce dépôt permet d'installer Nezzel sur Windows en une commande avec [Scoop](https://scoop.sh), sans l'écran d'avertissement bleu qui apparaît avec l'installateur classique.

```pwsh
scoop bucket add nezzel https://github.com/hululsofthq/scoop-nezzel
scoop install nezzel/nezzel
```

Pour mettre à jour : `scoop update nezzel`. Vos réglages sont conservés entre les mises à jour. En savoir plus sur l'application : [Nezzel Desktop](https://github.com/hululsofthq/nezzel-desktop#en-français).

## License

The files in this bucket are released under the [Unlicense](LICENSE). Nezzel Desktop itself is [AGPL-3.0](https://github.com/hululsofthq/nezzel-desktop/blob/main/LICENSE).
