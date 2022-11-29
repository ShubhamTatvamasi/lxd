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

