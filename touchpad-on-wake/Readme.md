# Touchpad Resume On Wake
--------
## Background

On some Lenovo Thinkpad T-series laptops running some Linux distros, there are reports of the touchpad losing all configuration after a sleep/wake cycle. This has been confirmed to happen with the T440 and T450, in both Arch Linux as well as Ubuntu-derived distros.

On my T440s, I had this issue running Pop!_OS 18.04. This systemd/system-sleep script is my solution.

## How it works

It works by disabling and re-enabling the mouse using modprobe. That's it.

## Installation

- Copy wake-restart-touchpad to /lib/systemd/system-sleep
- Make wake-restart-touchpad executable


Or

```
$ sh ./install.sh
```

Enjoy!
