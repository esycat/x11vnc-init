# Upstart Config for X11 VNC

## Installation

Install the `x11vnc` package first:
```bash
sudo apt-get install x11vnc
```

Copy configuration files:
```bash
sudo cp ./default/x11vnc /etc/default/
sudo cp ./init/x11vnc.conf /etc/init/
sudo ln -s /lib/init/upstart-job /etc/init.d/x11vnc
```

### Usage

```bash
service xvfb start
service xvfb status
```
