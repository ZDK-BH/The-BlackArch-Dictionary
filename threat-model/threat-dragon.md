# threat-dragon

**Category:** `threat-model`  
**Version in source list:** `2.2.0`  
**Package name:** `threat-dragon`

## What it does

Electron Threat Modelling and diagramming tool.

## What it can be used for

Structured review of systems to identify threats, controls, and design weaknesses.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed threat-dragon
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql threat-dragon | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
threat-dragon --help
threat-dragon -h
man threat-dragon
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Document assets, trust boundaries, data flows, and actors.
2. Identify likely threats and existing controls.
3. Prioritize mitigations by impact and effort.
4. Review the model whenever architecture changes.

## Example commands

```bash
threat-dragon --help
```

```bash
threat-dragon -h
```

```bash
# Project prep:
mkdir -p threat-model-notes
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
