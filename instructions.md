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

### Remove Programs _snap_

```bash
    ~$ sudo snap remove [name program]
```

### Install Programs _apt_

```bash
    ~$ sudo apt-get install [name program]
    ~$ sudo add-apt-repository ppa:[name program]
```

### Remove Programs _apt_

```bash
    ~$ sudo apt-get remove --purge [name program]
```

### Install Programs _.run_ || _.bin_ || _.sh_

```bash
    ~$ sudo ./[name program].run
    ~$ sudo ./[name program].bin
    ~$ sudo ./[name program].sh
```

### Remove Programs _.run_ || _.bin_ || _.sh_

```bash
    ~$ sudo cd /[path]/$ ./uninstall
    ~$ sudo ./[name program].bin --uninstall
    ~$ cd /[path]/$ sudo rm -r [name program]
```

### Install Key _SSH_

```bash
    ~$ ssh-keygen -t rsa -b 4096 -C "[your email]" or
    ~$ ssh-keygen -t ed25519 -C "[your email]"
    ~$ [Press Enter] [Press Enter]
    ~$ eval "$(ssh-agent -s)"
    ~$ ssh-add ~/.ssh/id_rsa
```

### Install Key Signing _GPG_

```bash
    ~$ gpg --list-secret-keys --keyid-format=long
    ~$ gpg --full-generate-key
    ~$ gpg --list-secret-keys --keyid-format=long
    ~$ gpg --armor --export [key number]
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
    - Code Spell Checker
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

### NUM KEY WINDOWS

```bash
    C:> wmic path softwareLicensingService get OA3xOriginalProductKey
```

### LINUX

```bash
    ~$ sudo apt --fix-broken install
```

### Exercism

```bash
    ~$ sudo snap install exercism
    ~$ exercism version
    ~$ exercism configure --token=[your token]
    ~$ exercism download --exercise=[exercise] --track=[language]
    ~$ exercism submit [path]
```

### Node JScript

```bash
    ~$ curl -fsSL https://deb.nodesource.com/setup_lts.x |
        sudo -E bash - sudo apt-get install -y nodejs
    ~$ yarn
    ~$ yarn init - y
    ~$ yarn tsc --init
    ~$ yarn global [name]
    ~$ yarn add [name]
    ~$ yarn add [name] -D
```

### Node JScript NVM

```bash
    ~$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
    ~$ source ~/.bashrc
    ~$ nvm list-remote
    ~$ nvm install [--version]
    ~$ nvm use [--version]
    ~$ node -v
    ~$ npm -v
```

### Git

```bash
    ~$ git init
    ~$ git add [name file]
    ~$ git add .
    ~$ git status
    ~$ git log
    ~$ git commit -m "[message]"
    ~$ git push
    ~$ git rm --cache [name file]
    ~$ git pull
    ~$ git branch
    ~$ git branch [name]
    ~$ git checkout [name]
    ~$ git branch [name] --delete
    ~$ git config --global user.signingKey [key number]
```

### Remembered Links

```bash
    · TYPING:
        - https://www.typingclub.com
    · DEVELOPMENT:
            PAID OUT:
                - https://www.rocketseat.com.br/
                - https://www.labenu.com.br/
                - https://www.betrybe.com/
                - https://www.alura.com.br/
        - https://vanhack.com/english-for-tech-talent
        - https://blog.rocketseat.com.br/
        - https://www.dio.me/
        - https://www.w3schools.com/
        - https://www.tutorialspoint.com/tutorialslibrary.htm
        - https://www.tutorialsteacher.com/
        - https://web.dev/
        - https://devdocs.io/
        - https://javascript.info/
        - https://www.freecodecamp.org/learn/
        - https://vitejs.dev/guide/
        - https://nativebase.io/
        - https://www.prisma.io/
        - https://graphql.org/
        - https://jestjs.io/pt-BR/
        - https://railway.app/
        - https://jwt.io/
        - https://realm.io/
        - https://expo.dev/
        - https://moti.fyi/
        - https://www.frontendmentor.io/
        - https://randomuser.me/
        - https://mailtrap.io/
        - https://exercism.org/
        - https://grasshopper.app/pt_br/
        - https://flexboxfroggy.com/
        - https://skillshop.exceedlms.com/student/catalog
        - https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
        · SECURITY:
            - https://www.hacker101.com/
    · ICONS:
        - https://boxicons.com/
        - https://ant.design/
        - https://phosphoricons.com/
        - https://remixicon.com/
    · ANIMATION:
        - https://scrollrevealjs.org/
```
