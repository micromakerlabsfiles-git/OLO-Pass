# OLO Pass — Readme

Welcome to your **OLO Pass**! This hardware password vault and automated keyboard companion helps you store credentials securely and type them instantly over Bluetooth without installing any software on your computer.

Web Controller Link : [OLO Pass WebContrller](https://micromakerlabsfiles-git.github.io/OLO-Pass/)


### 🔑 Default Credentials
For first-time setups, use the following default PIN code to access your vault:
*   **On-Device Password Vault PIN:** `1234`

*(Note: The Web Controller does not use a static password; it secures serial connections dynamically using the temporary OTP unlock code shown on your OLO Pass screen).*

---

## 1. Physical Device & Screen Navigation

Your OLO Pass features a crisp OLED screen and a single physical touch button. All on-device navigation is performed using this button.

### Core Button Actions
*   **Single Tap**: Cycle options, scroll menus downward, or flip pages.
*   **Long Press (Hold for 1 Second)**: Confirm a selection, enter submenus, or toggle states.

---

## 2. On-Device Screens & Clock Modes

By default, the device is in **Clock Mode**. Tapping the button cycles through four dashboard screens:

1.  **Digital Clock Face**: Displays current date, time, and Bluetooth connection status.
2.  **Analog Clock Face**: Shows a classic watch dial on the right side and a digital time readout on the left.
3.  **Bluetooth Status Page**: Displays the current Bluetooth broadcast name (e.g., `OLO Bit`) and connection state (`Connected`, `Advertising`, or `Disabled`).
4.  **IT Security Tips Page**: Displays useful security tips randomly selected from a catalog of 300 preloaded recommendations.
    *   *Paging*: If a tip is long, it is split into multiple pages (e.g., `(1/2)`). **Single tap** to read the next page. Tapping on the final page will bring you back to the Digital Clock Face.

### Accessing the Device Menu
From any of the four clock pages, **Long Press** to open the main menu:
*   **Password Vault**: Access your credentials on-screen to trigger automated typing.
*   **Quick Type**: Instantly type out the stored scratch payload.
*   **Device Settings**: Configure device-level hardware options.
*   **Back**: Return to the clock display screen.

---

## 3. In-Device Settings Menu

Scroll down to **Device Settings** and **Long Press** to access hardware configurations:

*   **LED Settings**: Toggle the colorful status NeoPixel light `ON` or `OFF`.
*   **Sound Settings**: Toggle audio beeps and feedback sounds `ON` or `OFF`.
*   **Bluetooth**: Toggle the Bluetooth antenna `ON` (ready to connect) or `OFF` (silent mode).
    *   *Auto-Disable Feature*: If Bluetooth is enabled but remains disconnected (no host device connects) and the device is idle for **2 minutes**, Bluetooth will automatically toggle `OFF` and save to NVS to save power and improve security. A dual falling-tone beep will sound to notify you.
*   **Time Format**: Toggle between `12-Hour` (AM/PM) and `24-Hour` clock display modes.
*   **Hourly Chime**: Toggle a gentle audio alert on the hour `ON` or `OFF`.
*   **Target OS**: Tell OLO Pass what operating system you are connected to (`Windows`, `macOS`, `Linux`, or `Android`) so that keyboard shortcut keystrokes map correctly.
*   **Reset Settings**: Restore all system options back to factory defaults.
*   **Back**: Return to the main menu.

---

## 4. Web Controller Guide

The Web Controller is a dashboard running directly inside your browser. It allows you to manage your vault credentials, sync your clock, and customize your device name.

### Connecting to the Web Controller
1.  Connect your OLO Pass to your computer using a USB data cable.
2.  Open your web browser (Chrome, Edge, Brave, etc.) and load the Web Controller page.
3.  Click **Connect via USB Serial** and select your device port.
4.  **Security Unlock**: For safety, your OLO Pass screen will display a temporary **Browser OTP Code** (e.g., `1234`). Enter this code on the browser page to unlock the controller panel.

### Managing Your Password Vault
Once unlocked, the **Vault Manager** tab displays your saved accounts:
*   **Add / Edit Account**: Fill out the fields in the editor panel on the right (Title, Username, Password, URL) and click **Save to Device**.
*   **Favorites**: Click the star (★) icon next to any credential to bookmark it. Bookmarked accounts always float to the top of your list on the device screen for immediate access.
*   **Instant Copy**: Click the clipboard (📋) icon to copy a password directly to your computer's clipboard.
*   **Search**: Type in the search box to filter your credentials lists instantly.

### Bulk CSV Importing (Chrome, Edge, Brave)
You can import passwords exported from your browser in bulk:
1.  Export your passwords from your browser settings into a `.csv` file.
2.  Locate the **Bulk Import Credentials** bar at the top of the Vault Manager tab.
3.  Drag and drop your browser CSV file into the dotted zone (or click it to browse).
4.  The credentials will load into the list automatically. Review and save them to the device!

### Backup & Export
*   Click **Export CSV** to save a local spreadsheet copy of your vault records. Store this file in a secure, encrypted drive for backups.
*   Click **Clear Vault** (in red) to wipe all passwords from the OLO Pass hardware memory.

### Customizing Device Settings & Bluetooth Name
Under the **Device Config** section of the Web Controller, you can customize your hardware properties:
*   **Device Broadcast Details**: Edit the **Bluetooth Device Name** and **Manufacturer Name** (e.g., custom labels instead of the defaults).
*   **Keystroke Typing Speed**: Adjust character delay and line delay (in milliseconds). If the device types too fast and misses characters on slow computers, increase these values.
*   **System Sound & Chime**: Toggle chime tones, sound, and Bluetooth via the web control panels.
*   **Click Save Configurations** at the bottom to store changes permanently on the device.

---

## 5. Security Checklist: Things to Do & Follow

To maintain maximum safety for your sensitive accounts, always follow these rules:

*   [ ] **Never Reuse Passwords**: Create unique, randomized passwords for every service. Use your OLO Pass web generator to draft highly secure strings.
*   [ ] **Set a Device PIN**: Enable a secure device startup PIN under the vault settings to prevent unauthorized physical access if your OLO Pass is lost or stolen.
*   [ ] **Enable Multi-Factor Authentication (MFA)**: A password manager is your first line of defense, but always turn on 2FA/MFA on critical accounts (email, online banking) for absolute safety.
*   [ ] **Double-Check Recipient Domains**: Before using the physical OLO Pass to type credentials into a website, check the URL in your address bar to make sure it is not a phishing duplicate.
*   [ ] **Keep Backups**: Regularly export an encrypted CSV backup of your passwords. Keep the backup sheet offline (e.g., on a secure USB drive in a safe).
*   [ ] **Disconnect USB when Unused**: Unplug your OLO Pass from the USB port when you are not actively managing credentials via the Web Controller to block physical access.
*   [ ] **Keep Bluetooth Off when Unnecessary**: If you only use OLO Pass in a fixed desk setup or do not need wireless connections, toggle Bluetooth `OFF` in the device settings. Note that OLO Pass automatically turns off Bluetooth if left disconnected and idle for **2 minutes**.
