# Antigravity Installer (Arch / Garuda / Manjaro)

Unofficial installer for **Google Antigravity** on Arch-based Linux distributions.

Неофициальный установщик **Google Antigravity** для дистрибутивов на базе Arch Linux.

---

## ✨ Features / Возможности

- ✅ Fetches the **latest Antigravity build** directly from Google APT
- ✅ Verifies integrity via **SHA256 checksum**
- ✅ Installs binaries into **`/opt/antigravity`**
- ✅ Creates a convenient **`antigravity`** launcher in `*/usr/local/bin*`
- ✅ Installs **.desktop launcher** and application icon
- ✅ Applies **Chrome-style sandbox** fix for better compatibility
- ✅ **Idempotent:** re-running the installer updates Antigravity to the latest version

---

## 📂 Repository

GitHub: https://github.com/apipa12/antigravity-installer

---

## 🇬🇧 INSTALL / UPDATE

### 1. Clone the repository

```bash
git clone https://github.com/apipa12/antigravity-installer.git
cd antigravity-installer
```

### 2. Make the installer executable

```bash
chmod +x antigravity-installer.sh
```

### 3. Run the installer

```bash
./antigravity-installer.sh
```

The script will:

- Fetch the latest Antigravity package from Google APT
- Verify SHA256 checksum
- Install files into `/opt/antigravity`
- Create a symlink `/usr/local/bin/antigravity`
- Install desktop entries and icons
- Apply sandbox fixes if needed

### 4. Run Antigravity

```bash
antigravity
```

### 5. Uninstall

```bash
./antigravity-installer.sh --uninstall
```

This will remove Antigravity binaries, symlinks, and desktop entries installed by the script.

---

## 🇷🇺 УСТАНОВКА / ОБНОВЛЕНИЕ

### 1. Клонируйте репозиторий

```bash
git clone https://github.com/apipa12/antigravity-installer.git
cd antigravity-installer
```

### 2. Сделайте скрипт исполняемым

```bash
chmod +x antigravity-installer.sh
```

### 3. Запустите установку

```bash
./antigravity-installer.sh
```

Скрипт автоматически:

- Находит последнюю доступную версию Antigravity в репозиториях Google APT
- Проверяет целостность файла по **SHA256**
- Устанавливает программу в каталог **`/opt/antigravity`**
- Создаёт удобный ярлык **`/usr/local/bin/antigravity`**
- Добавляет ярлык приложения в меню и иконку
- Настраивает sandbox, как у Google Chrome
- При повторном запуске обновляет Antigravity до последней версии

### 4. Запуск программы

```bash
antigravity
```

### 5. Удаление

```bash
./antigravity-installer.sh --uninstall
```

Скрипт удалит:

- Установленные файлы Antigravity из `/opt/antigravity`
- Символическую ссылку `/usr/local/bin/antigravity`
- Desktop-файлы и иконки, добавленные этим инсталлером

---

## 📋 Requirements / Требования

На системе должны быть установлены следующие утилиты:

- `curl`
- `bsdtar`
- `sha256sum`
- `awk`
- `sudo`

Проверить наличие можно, например, так:

```bash
which curl bsdtar sha256sum awk sudo
```

Если какая-то утилита не найдена, установите её через пакетный менеджер:

```bash
sudo pacman -S curl libarchive coreutils gawk sudo
```

(пакеты могут немного отличаться в разных Arch-совместимых дистрибутивах).

---

## ⚠️ Disclaimer

- This installer is **unofficial** and is **not affiliated with or endorsed by Google**.
- Use at your own risk. Always review shell scripts before running them with elevated privileges.
- The script aims to be safe and minimal, but you are responsible for your own system.

---

## 🛠 Support / Поддержка

If you find a bug or have a feature request:

- Open an issue in the repository: https://github.com/apipa12/antigravity-installer/issues

Если вы нашли баг или хотите предложить улучшение:

- Создайте issue в репозитории: https://github.com/apipa12/antigravity-installer/issues

Contributions, pull requests, and feedback are welcome! 🚀
