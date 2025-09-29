# pi5-kiosk-bash

A single-script solution to turn a Raspberry Pi 5 into a kiosk that displays a webpage in full screen. Ideal for dashboards (e.g., Power BI) and status boards.

> **Note:** Not intended for use with touchscreens.

## Features

- Lightweight setup using Raspberry Pi OS (Bookworm)
- Auto-launches a specified webpage on boot
- Optional auto-refresh capability
- Single executable Bash script

---

## Prerequisites

- Raspberry Pi 5
- Monitor and peripherals (keyboard/mouse) for initial setup
- Raspberry Pi OS **Bookworm** (desktop version — *not headless*)
- Internet connection

---

## Installation

1. Flash Raspberry Pi OS (Bookworm, with desktop) onto your Pi.
2. Boot up the Pi and connect it to a monitor.
3. [Download the latest release](https://github.com/yourusername/pi5-kiosk-bash/releases) from this GitHub repository.
4. Open the script in a text editor (e.g., nano) and set your desired webpage URL:

   ```bash
   nano pi5-kiosk.sh
   ```

   Find the line marked for the URL and replace it with your own (e.g., Power BI report URL).

5. Make the script executable and run it:

   ```bash
   chmod +x pi5-kiosk.sh
   ./pi5-kiosk.sh
   ```

---

## Optional

To enable periodic refreshes, you can modify the script or add a cron job.

---

## License

MIT License
