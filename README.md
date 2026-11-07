# Ariadne Binaries

Prebuilt binaries of the Ariadne CLI, a static-analysis engine for Java and Spring security review. The Ariadne VS Code extension downloads its scanner from this repo's releases.

## Download

Get the latest build from [Releases](https://github.com/tallbreadstick/ariadne-binaries/releases). Each file is named after its build target, followed by the version, for example `x86_64-unknown-linux-gnu-0.0.2`. Windows builds end in `.exe`.

| OS | Targets |
| --- | --- |
| Linux | x86_64, i686, aarch64, armv7 |
| Windows | x86_64, i686, aarch64 (MSVC), plus x86_64 and i686 MinGW builds |
| macOS 11+ | universal2, aarch64 (Apple Silicon), x86_64 (Intel) |

## Usage

On Linux and macOS, make the file executable first:

```sh
chmod +x ./x86_64-unknown-linux-gnu-0.0.2
```

If macOS Gatekeeper blocks the unsigned binary, remove the quarantine flag:

```sh
xattr -d com.apple.quarantine <file>
```

## VS Code extension

You don't need to download anything by hand. The extension picks the right binary for your system and downloads it. To update to a newer release, delete the old scanner with the trash icon so the extension downloads the latest one.
