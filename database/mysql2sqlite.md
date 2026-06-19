# mysql2sqlite

**Category:** `database`  
**Version in source list:** `14.e5b2c31`  
**Package name:** `mysql2sqlite`

## What it does

Converts a mysqldump file into a Sqlite 3 compatible file.

## What it can be used for

Testing database configuration, injection risk, access controls, and data exposure in lab/approved systems.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed mysql2sqlite
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql mysql2sqlite | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
mysql2sqlite --help
mysql2sqlite -h
man mysql2sqlite
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use local databases or intentionally vulnerable lab apps.
2. Create backups before testing anything with write capability.
3. Start with read-only enumeration where possible.
4. Use findings to patch queries, permissions, and exposure.

## Example commands

```bash
mysql2sqlite --help
```

```bash
mysql2sqlite -h
```

```bash
# Lab database/app pattern after checking help:
mysql2sqlite <local-lab-target>
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
