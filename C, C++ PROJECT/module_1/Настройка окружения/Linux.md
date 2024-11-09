## Установка компилятора

 Для программирования на C вам понадобится компилятор. Наиболее распространённым вариантом является GCC (GNU Compiler Collection).

###  Debian/Ubuntu:

```bash
sudo apt update && sudo apt install build-essential
```

###  Fedora:

```bash
sudo dnf groupinstall "Development Tools"
```

###  Arch Linux:

```bash
sudo pacman -S base-devel
```

## Установка IDE

### CLion (рекомендуется)

#### Debian/Ubuntu/Fedora:

1. **Скачайте CLion:** Перейдите на [официальный сайт JetBrains](https://www.jetbrains.com/clion/download/) и скачайте архив с CLion.

2. **Распакуйте архив:** Откройте терминал и выполните команду:
```bash
tar xzf CLion-*.tar.gz
```

3. **Запустите CLion:** Перейдите в распакованную папку и запустите скрипт:
```bash
cd clion-*/bin && ./clion.sh
```

#### Arch Linux:

1. **Клонируйте репозиторий** с PKGBUILD из AUR

```bash
git clone https://aur.archlinux.org/clion.git && cd clion
```

2. **Соберите и установите** пакет CLion
```bash
makepkg -sirc
```

### Code::Blocks

#### Debian/Ubuntu:

```bash
sudo apt update && sudo apt install codeblocks
```

#### Fedora:

```bash
sudo dnf install codeblocks
```

#### Arch Linux:

```bash
sudo pacman -S codeblocks
```

### Eclipse

#### Debian/Ubuntu:

1. Установите Java Development Kit (JDK):

```bash
sudo apt update sudo apt install default-jdk
```

2. Скачайте Eclipse с [официального сайта](https://www.eclipse.org/downloads/).
3. Распакуйте архив и запустите Eclipse

### Fedora:

1. Установите JDK:

```bash
sudo dnf install java-1.8.0-openjdk-devel
```

2. Скачайте Eclipse с [официального сайта](https://www.eclipse.org/downloads/) и распакуйте его

 Arch Linux:

```bash
sudo pacman -S eclipse
```

### Visual Studio Code

#### Debian/Ubuntu:

1. Добавьте репозиторий Microsoft:

```bash
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add - sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```    
2. Установите VS Code:

```bash
sudo apt update sudo apt install code
```    

#### Fedora:

1. Добавьте репозиторий Microsoft:

```bash
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc sudo bash -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'`
```

2. Установите VS Code:

```bash
sudo dnf install code
```
 
#### Arch Linux:
 
```bash
sudo pacman -S code
```