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
    - Markdown Preview Enhanced
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

### GRUB - THEMES

```bash
    /themes
        /ubuntu
            /icons
            - icon.png 32x32
        - background.jpg
        - fonts.pf2
        - menu.png
        - line.png
        - theme.txt
```

### GRUB RESCUE - INITRAMFS

```bash
    grub rescue> set root=(hd0,msdos5)
    grub rescue> set prefix=(hd0,msdos5)/dev/sda5
    grub rescue> insmod normal
    grub rescue> normal
    
    ~$ sudo fdisk -l
    - /dev/sda5   Linux
    ~$ sudo mount /dev/sda5 /mnt
    ~$ sudo grub-install --root-directory=/mnt /dev/sda
    initramfs> fsck -y /dev/sda5
```
### DEL GRUB - RESTORE WINDOWS
```bash
   >bootsect /nt60 all/force /mbr
```
### Exercism

```bash
    ~$ sudo snap install exercism
    ~$ exercism version
    ~$ exercism configure --token=[your token]
    ~$ exercism download --exercise=[exercise] --track=[language]
    ~$ exercism submit [path]
```
