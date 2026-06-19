# androidpincrack

**Category:** `mobile`  
**Version in source list:** `5.6439bd2`  
**Package name:** `androidpincrack`

## What it does

Bruteforce the Android Passcode given the hash and salt.

## What it can be used for

Android/iOS app review, APK extraction, mobile forensics, and mobile security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed androidpincrack
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql androidpincrack | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
androidpincrack --help
androidpincrack -h
man androidpincrack
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use apps/devices you own or have permission to test.
2. Copy APKs or backups into a lab folder.
3. Start with static analysis before runtime instrumentation.
4. Document permissions, endpoints, secrets, and insecure storage.

## Example commands

```bash
androidpincrack --help
```

```bash
androidpincrack -h
```

```bash
# Local APK pattern:
androidpincrack ./app.apk
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
