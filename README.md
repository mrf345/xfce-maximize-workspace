# xfce-maximize-workspace

This is a fork from [DimseBoms/XFCE-Dynamic-Workspace](https://github.com/DimseBoms/XFCE-Dynamic-Workspace) it maintains the same dynamic workspaces functionality, and adds to it maximizing newly opened window into a new workspace, and moves back to the previous workspace once the window's closed.

<p align="center" style="margin-top: 30px;">
    <a href="https://raw.githubusercontent.com/mrf345/xfce-maximize-workspace/main/demo.gif">
        <img src="demo.gif" width="80%" />
    </a>
</p>

### Blacklisting:

If you want some windows to be ignored (no maximizing into workspace), you can add the window title or class name into a new line in `~/.xfce_max_blacklist`.

My blacklist:

```
Thunar
Peek
Safelock
GIMP Startup
VirtualBox
VirtualBoxVM
```

### Installation:
```bash
# Install the required dependencies:
# Ubuntu/Debian
sudo apt install python3-gi libwnck-3.0 wmctrl
# Fedora
sudo dnf install python3-gobject libwnck3 wmctrl
# Arch based
sudo pacman -S libwnck3 python-gobject wmctrl

# Clone the repository:
git clone https://github.com/mrf345/xfce-maximize-workspace.git

# Usage
python3 xfce-maximize-workspace/dynamic_workspaces.py
```
