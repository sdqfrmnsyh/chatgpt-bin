# ChatGPT for Arch Linux

Unofficial Arch Linux packaging for the ChatGPT desktop application.

This package repackages the official RPM published by OpenAI into a native Arch Linux package.

![](chatgpt.png)

## Installation

Clone the repository:

```bash
git clone https://github.com/sdqfrmnsyh/chatgpt-bin.git
cd chatgpt-bin
```

Build and install:

```bash
makepkg -si
```

`makepkg` downloads the RPM directly from OpenAI's official distribution server.

## Update

The package tracks the version declared in `PKGBUILD`. When OpenAI releases a newer version, update `pkgver` and regenerate `.SRCINFO`:

```bash
makepkg --printsrcinfo > .SRCINFO
```

## Architecture

Supported architectures:

- `x86_64`
- `aarch64`

The appropriate RPM is selected automatically by `makepkg`.

## System Tray

The Linux application currently does **not** provide a system tray icon. This is an upstream application behavior and is not caused by this Arch package.

## Disclaimer

This is an unofficial community package. It is not affiliated with or endorsed by OpenAI.

The application itself is proprietary software distributed by OpenAI. The upstream RPM identifies its license as `Proprietary`.

Upstream:

https://developers.openai.com/codex/app
