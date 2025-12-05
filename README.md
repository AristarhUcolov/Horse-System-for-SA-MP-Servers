# 🐴 Horse System for SA-MP Servers

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![SA-MP](https://img.shields.io/badge/SA--MP-0.3.7+-orange.svg)](https://www.sa-mp.com/)
[![Pawn](https://img.shields.io/badge/Language-Pawn-yellow.svg)](https://www.compuphase.com/pawn/pawn.htm)

**Author:** Aristarh Ucolov (Аристарх Уколов)

A horse riding system for San Andreas Multiplayer (SA-MP) servers. Originally developed for Wild West themed servers.

---

## 📋 Table of Contents

- [English](#english)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Controls](#controls)
- [Русский](#русский)
  - [Возможности](#возможности)
  - [Установка](#установка)
  - [Использование](#использование)
  - [Управление](#управление)
- [Screenshots](#screenshots--скриншоты)
- [Archive](#archive--архив)
- [License](#license)

---

## English

### Features

- 🎮 Realistic horse riding animation using bike animations
- 🕹️ Responsive movement controls (walk, turn left/right)
- 📦 Simple integration - just copy and include in your gamemode
- 🎨 Visual horse model attached to player

### Installation

1. Download `HorseSystem.pwn` from this repository
2. Copy the code into your gamemode or filterscript
3. Make sure the horse model (ID: 11733) is available on your server
4. Compile and run your server

### Usage

To spawn a horse, use the command:
```pawn
/horse
```

### Controls

| Key | Action |
|-----|--------|
| `ALT` (Walk Key) | Move forward |
| `SPACE` (Sprint) or `SHIFT` (Jump) | Turn right |

### Code Example

```pawn
CMD:horse(playerid, params[])
{
    // Attach horse object to player
    SetPlayerAttachedObject(playerid, 5, 11733, 5, -0.627999, 1.480000, -0.126000, 
        93.399879, 1.999998, 77.299987, 1.103000, 1.112997, 1.014999);
    // Apply riding animation
    ApplyAnimation(playerid, "BIKED", "BIKED_RIDE", 4.1, 1, 1, 1, 1, 0, 1);
}
```

---

## Русский

### Возможности

- 🎮 Реалистичная анимация езды на лошади с использованием велосипедных анимаций
- 🕹️ Отзывчивое управление движением (ходьба, поворот влево/вправо)
- 📦 Простая интеграция - просто скопируйте и включите в ваш gamemode
- 🎨 Визуальная модель лошади, прикреплённая к игроку

### Установка

1. Скачайте `HorseSystem.pwn` из этого репозитория
2. Скопируйте код в ваш gamemode или filterscript
3. Убедитесь, что модель лошади (ID: 11733) доступна на вашем сервере
4. Скомпилируйте и запустите ваш сервер

### Использование

Для вызова лошади используйте команду:
```pawn
/horse
```

### Управление

| Клавиша | Действие |
|---------|----------|
| `ALT` (Клавиша ходьбы) | Движение вперёд |
| `SPACE` (Спринт) или `SHIFT` (Прыжок) | Поворот вправо |

### Пример кода

```pawn
CMD:horse(playerid, params[])
{
    // Прикрепление объекта лошади к игроку
    SetPlayerAttachedObject(playerid, 5, 11733, 5, -0.627999, 1.480000, -0.126000, 
        93.399879, 1.999998, 77.299987, 1.103000, 1.112997, 1.014999);
    // Применение анимации езды
    ApplyAnimation(playerid, "BIKED", "BIKED_RIDE", 4.1, 1, 1, 1, 1, 0, 1);
}
```

---

## Screenshots / Скриншоты

![Horse System Screenshot 1](https://github.com/AristarhUcolov/Horse-System-for-SA-MP-Servers-by-Aristarh-Ucolov-SA-MP-/assets/56760026/89276dc0-f0dc-4652-8a27-9cb6e3f0c6ac)

![Horse System Screenshot 2](https://github.com/AristarhUcolov/Horse-System-for-SA-MP-Servers-by-Aristarh-Ucolov-SA-MP-/assets/56760026/ffdfcb09-d166-4f01-a6d5-b225dab4fbf6)

![Horse System Screenshot 3](https://github.com/AristarhUcolov/Horse-System-for-SA-MP-Servers-by-Aristarh-Ucolov-SA-MP-/assets/56760026/416fcd4e-63db-43ea-aa9f-19bae7b5a549)

---

## Archive / Архив

📚 Original SA-MP Forum thread (archived):
https://sampforum.blast.hk/showthread.php?tid=677383&pid=4155030

---

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

---

**Made with ❤️ by Aristarh Ucolov**

*Also known as: Jon_Stark / Jon_Motorskull / John_Motorskull / ToGoRo*
