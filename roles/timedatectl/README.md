 Ansible role timedatectl
=========================

Ansible role to configure timedatectl on linux.

## What does thes role do?

+ Configure /etc/systemd/timesyncd.conf
+ Set timezone
+ install tzdata
+ make sure systemd-timesyncd is started

## Variables

| Variable | Value |
| --- | --- |
| `timedatectl__timezone` | `Europe/Busingen` |
| `timedatectl__timeservers` | *see [defaults/main.yml](defaults/main.yml)*
| `timedatectl__RootDistanceMaxSec` | `5` |
| `timedatectl__PollIntervalMinSec` | `32` |
| `timedatectl__PollIntervalMaxSec` | `2048` |
| `timedatectl__ConnectionRetrySec` | `30` |
| `timedatectl__SaveIntervalSec` | `60` |

## Author

+ L3D <l3d@c3woc.de>

## LICENSE

[MIT](../../LICENSE)
