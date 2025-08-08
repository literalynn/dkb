# dkb — Disk bars viewer

```bash
lynn@ltn1:~$ dkb
=== Disques physiques ===
sda  12To  WDC WD120      [███████████████████░░░░░░░░░░░]  65,5%  (7,9 To/12,0 To)
sdb  14To  WDC WD140      [████████████████░░░░░░░░░░░░░░]  56,2%  (7,9 To/14,0 To)
sdc   8To  HGST HUH       [███████████████░░░░░░░░░░░░░░░]  51,2%  (4,1 To/8,0 To)
sdd  16To  ST16000        [████████████░░░░░░░░░░░░░░░░░░]  40,5%  (6,5 To/16,0 To)
sde   8To  ST8000V        [████████████████████████████░░]  96,0%  (7,7 To/8,0 To)
sdf  12To  ST12000        [██████████████████░░░░░░░░░░░░]  61,0%  (7,3 To/12,0 To)
sdg  10To  ST10000V       [█████████████████████████████░]  97,3%  (9,7 To/10,0 To)
sdh   2To  WD Green       [████████████████░░░░░░░░░░░░░░]  55,6%  (1,1 To/2,0 To)
sdi 256Go  SanDisk        [██████████████████████░░░░░░░░]  73,5%  (188,2 Go/256,1 Go)

=== MergerFS ===
all      46To  mergerfs  [████████████████████░░░░░░░░░░]  68,2%  (31,2 To/45,8 To)
storage  20To  mergerfs  [██████████████████░░░░░░░░░░░░]  60,3%  (12,0 To/19,8 To)
```

## Installation (1-ligne)
```bash
sudo apt update && sudo apt install -y jq curl \
&& sudo curl -fsSL https://raw.githubusercontent.com/literalynn/dkb/main/dkb -o /usr/local/bin/dkb \
&& sudo chmod +x /usr/local/bin/dkb && dkb
```

## Usage
```bash
dkb
dkb 50
```

## Exigences
- jq, util-linux (lsblk/df), bash

## Licence
MIT
