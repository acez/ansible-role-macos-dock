Role Name
=========

A role to setup the macOS dock in a configured order. This role relies on [dockutil](https://github.com/kcrawford/dockutil) installed.

Requirements
------------

Homebrew must be setup and installed beforehand.

Role Variables
--------------

| Variable        | Description                           |
|-----------------|---------------------------------------|
| macos_dock_apps | List of Dock Applications and Folders |

For parameters of view and sort, please use `dockutil -h`

Example for configuration
-------

```yaml
macos_dock_apps:
  - { path: "/System/Applications/Launchpad.app" }
  - { path: "/System/Applications/Mail.app" }
  - { path: "/Applications/iTerm.app" }
  - { path: "~/Downloads", view: "grid", sort: "name" }
  - { path: "/Applications", view: "grid", sort: "name" }
```

License
-------

MIT
