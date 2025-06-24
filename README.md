# Home Assistant Dashboard

Welcome! This repository contains my Home Assistant dashboard configurations and assets.

Several people have asked to see my setup, so I'm excited to share what I’ve built so far.  
I hope it inspires or helps you with your own smart home dashboard.

---

## How to Use

1. Install all required components listed in the [Components](#components) section below.
2. Create a new dashboard from scratch in Home Assistant.
3. Replace the dashboard code:
   - Open the newly created dashboard in YAML mode.
   - Copy the contents of `dashboard.yaml` from this repository and paste it into your dashboard.

4. Expect initial errors — don’t worry.  
   Red warning messages are normal at first since my entity IDs likely won’t match yours.

5. Customize for your setup:
   - Replace my entity IDs (e.g., `person.richard`, `light.kitchen_ceiling`) with your own.
   - Adjust any sections to fit your devices or preferences.

6. Verify all custom components are installed and working correctly to ensure smooth operation.

---

## Latest Version

### Homepage
![Homepage](/assets/v2/Homepage.jpg)

### Living Room
![Living Room](/assets/v2/Livingroom.jpg)

### Homelab
![Homelab](/assets/v2/office.jpg)

### Bedroom & Kitchen
![Bedroom & Kitchen](/assets/v2/BedroomKitchen.jpg)

> Other rooms not shown here are available in the code.

### Vacuum Page
![Vacuum Page](/assets/v2/Vacuum.jpg)

---

## Components

- [Lovelace Mini Graph Card](https://github.com/kalkih/mini-graph-card)
- [Bubble Card](https://github.com/Clooos/Bubble-Card)
- [Yet Another Media Player](https://github.com/jianyu-li/yet-another-media-player)
- [Navbar Card](https://github.com/joseluis9595/lovelace-navbar-card)
- [Calendar Card Pro](https://github.com/alexpfau/calendar-card-pro)
- [Mushroom](https://github.com/piitaya/lovelace-mushroom)
- [button-card](https://github.com/custom-cards/button-card)
- [card-mod](https://github.com/thomasloven/lovelace-card-mod)
- [layout-card](https://github.com/thomasloven/lovelace-layout-card)
- [Vacuum Card](https://github.com/denysdovhan/vacuum-card)
- [Vertical Stack In Card](https://github.com/ofekashery/vertical-stack-in-card)
- [Custom Brand Icons](https://github.com/elax46/custom-brand-icons)
- [Kiosk Mode](https://github.com/NemesisRE/kiosk-mode)

---

## Initial Version

### Homepage
![Homepage](/assets/v1/Homepage.jpg)

### Living Room
![Living Room](/assets/v1/Livingroom.jpg)

### Homelab
![Homelab](/assets/v1/Homelab.jpg)

### Navbar
![Navbar](/assets/v1/Navbar.jpg)

---

## Room Card Logic (Homepage)

The Room Cards on the homepage reflect the real-time status of each room using intelligent backend logic.

### How It Works

- If everything in a room is turned off or in a normal state, the main room icon appears neutral (no color).
- If anything is turned on or requires attention — such as a TV, lights, or a scene — the icon becomes highlighted to show something is active in that room.

This allows for a quick visual check of room status at a glance.

---

### Example: Idle vs Active Room Card

#### Idle Room (No active devices or scenes)
![Idle Room Card Screenshot](/assets/v2/Off.png)

#### Active Room (Something is on or triggered)
![Active Room Card Screenshot](/assets/v2/Onn.png)

---

## Living Room Page – Media Section

The media section on the Living Room page does not display what's currently playing. Instead, it acts as a trigger for backend scripts that handle playback logic.

### How It Works

- **TV Shows (Completed)**  
  Example: *The Office*  
  - Turns on the TV (if it's off)
  - Plays a random episode

- **Movies**  
  - Selects a random unwatched movie
  - Plays it immediately

- **TV Shows (In Progress)**  
  - Resumes playback from the last watched point

This setup offers a seamless, personalized viewing experience based entirely on your watch history.

---

## Need Help?

If you run into issues or need help customizing the dashboard, feel free to open a discussion or reach out.  
If you notice a missing component or want yours listed, open an issue or PR.

---

## Support

<a href="https://www.buymeacoffee.com/richardbmh" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174">
</a>

---

## YouTube Channel

<a href="https://www.youtube.com/@richardbmh" target="_blank">
  <img src="https://img.shields.io/badge/Subscribe-YouTube-red?logo=youtube&style=for-the-badge" alt="YouTube Subscribe Badge">
</a>

**Click above to subscribe to my YouTube channel:**  
[https://www.youtube.com/@richardbmh](https://www.youtube.com/@richardbmh)
