# 🍊 Dark Orange Theme for Home Assistant

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg?style=for-the-badge)](https://github.com/hacs/default)
[![GitHub Release](https://img.shields.io/github/v/release/sajiko5821/Dark-Orange?style=for-the-badge&color=DF6040)](https://github.com/sajiko5821/Dark-Orange/releases)
[![HACS Validation](https://img.shields.io/github/actions/workflow/status/sajiko5821/Dark-Orange/validate.yml?branch=main&label=HACS%20Validation&style=for-the-badge)](https://github.com/sajiko5821/Dark-Orange/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

A clean, modern, and high-contrast dark theme with vibrant warm orange accents for [Home Assistant](https://www.home-assistant.io/).

---

## ✨ Features

- 🎨 **Original Tones**: Built on deep charcoal and soft gray surfaces (`#282A2F` & `#303236`) restored from [JuanMTech's orange_dark](https://github.com/JuanMTech/orange_dark) theme, paired with a signature warm orange accent (`#DF6040`).
- 👁️ **High Contrast & Legibility**: Pure crisp text (`#FFFFFF` and `#C5C9D0`) to eliminate unreadable gray-on-gray elements in dialogs, tables, and settings.
- 🍄 **Mushroom & Lovelace Ready**: Full RGB channels defined for seamless translucency and opacity effects across custom cards.
- 📐 **Material 3 / Modern HA**: Extensive coverage of MDC and M3 color tokens, preventing stubborn black-text-on-dark-background glitches.
- 🌗 **Light Mode Fallback**: Includes a clean, complementary light variant when switching to system light mode.

---

## 📦 Installation via HACS (Recommended)

### 1-Click Install
Click the badge below to directly open this repository in your Home Assistant HACS:

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=sajiko5821&repository=Dark-Orange&category=theme)

---

### Manual HACS Steps

1. Open **Home Assistant** and navigate to **HACS**.
2. Click the **three dots `⋮`** in the top right corner and choose **Custom repositories**.
3. Enter the following repository details:
   - **Repository:** `https://github.com/sajiko5821/Dark-Orange`
   - **Type:** `Theme`
4. Click **Add**.
5. Find **Dark Orange** in HACS and click **Download**.

---

## ⚙️ Setup & Activation

### 1. Enable Themes in Home Assistant
Ensure your `configuration.yaml` is set up to load themes from the `themes/` folder:

```yaml
frontend:
  themes: !include_dir_merge_named themes
```

*(If you already have themes enabled, you can skip this step).*

### 2. Reload Themes
You don't need to restart Home Assistant! Simply reload themes:
- Go to **Developer Tools** > **Actions** (or Services).
- Select `Frontend: Reload themes` (`frontend.reload_themes`).
- Click **Perform Action**.

### 3. Select the Theme
1. Click on your **User Profile** (bottom-left avatar).
2. Under **Theme**, choose **Dark Orange**.
3. *(Optional)* Select **Dark** mode to enjoy the full dark orange experience.

---

## 🎨 Color Palette

| Token | Color | Hex | Role |
| :--- | :--- | :--- | :--- |
| Primary Accent | <img src="https://via.placeholder.com/15/DF6040/000000?text=+" width="15" height="15" /> `#DF6040` | `#DF6040` | Buttons, Active Icons, Toggles, Sliders |
| Light Accent | <img src="https://via.placeholder.com/15/FF7A59/000000?text=+" width="15" height="15" /> `#FF7A59` | `#FF7A59` | Hover states, links, highlights |
| Background | <img src="https://via.placeholder.com/15/282A2F/000000?text=+" width="15" height="15" /> `#282A2F` | `#282A2F` | Main app background, sidebar |
| Card Surface | <img src="https://via.placeholder.com/15/303236/000000?text=+" width="15" height="15" /> `#303236` | `#303236` | Cards, popups, app header |
| Text Primary | <img src="https://via.placeholder.com/15/FFFFFF/000000?text=+" width="15" height="15" /> `#FFFFFF` | `#FFFFFF` | High-contrast readable headings & text |
| Text Secondary | <img src="https://via.placeholder.com/15/C5C9D0/000000?text=+" width="15" height="15" /> `#C5C9D0` | `#C5C9D0` | Subtitles, disabled states, borders |

---

## 🛠️ Manual Installation (Without HACS)

If you do not use HACS:
1. Download `dark_orange.yaml` from this repository.
2. Place it in your Home Assistant config directory under `themes/dark_orange.yaml`.
3. Reload themes under **Developer Tools** > **Actions** > `frontend.reload_themes`.

---

## 🙏 Credits & Acknowledgments

- The base colors and original gray tones are based on [JuanMTech's orange_dark theme](https://github.com/JuanMTech/orange_dark).

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).