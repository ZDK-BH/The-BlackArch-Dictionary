# android-ndk

**Category:** `mobile`  
**Version in source list:** `r29`  
**Package name:** `android-ndk`

## What it does

Android C/C++ developer kit

## What it can be used for

Android/iOS app review, APK extraction, mobile forensics, and mobile security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed android-ndk
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql android-ndk | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
android-ndk --help
android-ndk -h
man android-ndk
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use apps/devices you own or have permission to test.
2. Copy APKs or backups into a lab folder.
3. Start with static analysis before runtime instrumentation.
4. Document permissions, endpoints, secrets, and insecure storage.

## Example commands

```bash
android-ndk --help
```

```bash
android-ndk -h
```

```bash
# Local APK pattern:
android-ndk ./app.apk
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
