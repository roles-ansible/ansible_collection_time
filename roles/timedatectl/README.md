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
| `timedatectl__rootdistancemaxsec` | `5` |
| `timedatectl__pollintervalminsec` | `32` |
| `timedatectl__pollintervalmaxsec` | `2048` |
| `timedatectl__connectionretrysec` | `30` |
| `timedatectl__saveintervalsec` | `60` |

## Requirements

+ ``community.general``

## Author

+ L3D <l3d@c3woc.de>

## LICENSE

[MIT](../../LICENSE)
