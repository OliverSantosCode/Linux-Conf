### Install Programs _.deb_

```bash
    ~$ sudo dpkg -i [name program].deb
```

### Remove Programs _.deb_

```bash
    ~$ sudo dpkg -r [name program]
```

### Install Programs _snap_

```bash
    ~$ sudo apt install snapd
    ~$ sudo snap install [name program]
```

### Install Programs _apt_

```bash
    ~$ sudo apt-get install [name program]
    ~$ sudo add-apt-repository ppa:[name program]
```

### Install Programs _.run_ || _.bin_

```bash
    ~$ sudo ./[name program].run
    ~$ sudo ./[name program].bin
```

### Install Key _SSH_

```bash
    ~$ ssh-keygen -t rsa -b 4096 -C "[your email]"
    ~$ [Press Enter] [Press Enter]
    ~$ eval "$(ssh-agent -s)"
    ~$ ssh-add ~/.ssh/id_rsa
```

### Visual Studio _Code_

```bash
    - Node.js Exec
    - Material Icon Theme
    - Color Highlight
    - Bracket Pair Colorizer
    - Omni Theme
    - Live Server
    - Font Fira Code
    - ESLint
    - Prettier Code formatter
    - Advanced New File
    - File Utils
    - Font Cascadia Code
    - Live Share - Audio - Extention
    - Auto Rename Tag
    - Quokka
    - VSCode-pdf
    - Python - Pylance
    - Jupyter
```

### Drivers _NVIDIA_

```bash
    ~$ lsmod | grep -i [driver]
    ~$ lscpi
    ~$ apt search [driver]
    ~$ cd /etc/modprobe.d
    ~$ touch nvidia-graphics-drivers.conf
        blacklist nouveau
        blacklist lbm-nouveau
        alias nouveau off
        alias lbm-nouveau off
    ~$ update-initramfs -u
    ~$ boot up
    ~$ lsmod | grep -i [driver]
```
