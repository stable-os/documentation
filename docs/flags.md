---
sidebar_position: 2
---

# Flags
Flags are Stable OS's solution to feature flags. A flag indicates wether a feature is enabled, and can sometimes have a value. Flags should not be used to configure entire programs, just indicating wether a feature is enabled or not. Flags get processed by [`flagd`](https://github.com/stable-os/flagd) in the background.

## Why not just use a configuration file?
Configuration files aren't very easily editable by scripts, flags can be enabled or disabled simply by doing `touch` or `rm`. This allows scripts to complete a lot faster.

## Flags
All (documented) flags currently shipped in `flagd` are listed here.

### Boot
Flags related to bootloaders and bootmanagers

- boot.bootmanager.refind_enabled (bool)