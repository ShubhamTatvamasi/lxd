# lxd

Check if lxd is installed:
```bash
snap list lxd
```

Initalize:
```bash
sudo lxd init
```
storage backend = dir

### LXC

List running containers:
```bash
lxc list
```

Lanuch a new container:
```bash
lxc launch images:ubuntu/jammy ubuntu
```

Get shell access of container:
```bash
lxc exec ubuntu -- bash
```

List remote image repos:
```bash
lxc remote list
```

List remote images:
```bash
lxc image list images:
lxc image list ubuntu:
```

Search for specfic images:
```bash
lxc image list images: alpine
```

---

# Debian

Lanuch a debian container:
```bash
lxc launch images:debian/10 debian
```

Get shell access of debian container:
```bash
lxc exec debian -- bash
```

Stop debian container
```bash
lxc stop debian
```

Start debian container
```bash
lxc start debian
```

Restart debian container
```bash
lxc restart debian
```

Delete the container:
```bash
lxc delete debian --force
```

### Snapshot

Take snapshot of a container:
```bash
lxc snapshot debian mysnap1
```

Get container info:
```bash
lxc info debian
```

Delete snapshot:
```bash
lxc delete debian/mysnap1
```

Restore snapshot:
```bash
lxc restore debian mysnap2
```

Auto start container when reboot server:
```bash
lxc config set debian boot.autostart 1
```

Set container memory limit:
```bash
lxc config set debian limits.memory 1GB
```

Show container configuration:
```bash
lxc config show debian
```

Set 30 seconds delay before container start:
```bash
lxc config set debian boot.autostart.delay 30
```


