# 🕐 WordClock User Manual

## Introduction

Welcome to your WordClock! This clock displays the time using illuminated words on an LED matrix. You can change colors, brightness, and add fun visual effects.

**New User?** Start with the [Quick Start Guide](QUICK_START.md) to get your clock running in minutes.

---

## Table of Contents

1. [Web Interface](#web-interface)
2. [Button Menu](#button-menu)
3. [Display Settings](#display-settings)
4. [Visual Effects](#visual-effects)
5. [Firmware Updates](#firmware-updates)
6. [Troubleshooting](#troubleshooting)
7. [Home Assistant Integration](#home-assistant-integration)
8. [Scrolling Text](#scrolling-text)

---

## Web Interface

The web interface is the easiest way to control your WordClock. You can change settings, update firmware, and customize the display.

**📖 See the [Quick Start Guide - Customize Your Clock](QUICK_START.md#customize-your-clock) for how to access the web interface.**

## Button Menu

Your WordClock has three physical buttons for quick changes without opening the web interface:
- **Mode** button - Navigate between menu options
- **Plus (+)** button - Increase values or scroll up
- **Minus (-)** button - Decrease values or scroll down

### How to Use the Buttons

- **Short press Mode** - Cycle through menu options (Color, IP address, etc.)
- **Short press Plus/Minus** - Change the value of the current menu item
- **Long press Mode** - Enter WiFi setup or exit button menu

### Available Menus

Short press **Mode** to cycle through the following menu options:

**1. Color**
- Cycle through preset colors (Red, Green, Blue, Cyan, Yellow, Magenta)
- Use **Plus** or **Minus** buttons to change
- Colors change instantly as you scroll
- Changes save automatically

**2. Animation Mode**
- Choose when to show animations
- Use **Plus** or **Minus** to cycle through:
  - No effects (instant changes)
  - Quick transitions only
  - Animations every hour
  - Animations every 15 minutes
  - Animations every 5 minutes
  - Always show animations

**3. Night Mode**
- Turn night mode on or off
- Use **Plus** or **Minus** to toggle

**4. Night Start Hour**
- Set when night mode begins (0-23 hours)
- Use **Plus** or **Minus** to adjust the hour

**5. Night End Hour**
- Set when night mode ends (0-23 hours)
- Use **Plus** or **Minus** to adjust the hour

**6. Night Brightness**
- Set brightness level during night mode (0-7)
- Use **Plus** or **Minus** to adjust

**7. Night Effects**
- Enable or disable effects during night mode
- Use **Plus** or **Minus** to toggle on/off

**8. IP Address**
- View the clock's IP address
- Use **Plus** or **Minus** to scroll through the address

**9. USB Current**
- Shows detected USB power limit (read-only)
- Displays the detected mA rating from your power source

**10. Firmware Update**
- Only appears when an update is available
- Press **Plus** to start the firmware update

The menu will automatically close after 30 seconds of inactivity, or you can long press **Mode** to exit immediately.

---

## Display Settings

### Brightness

You can choose from 8 brightness levels:
- **Level 0** - Off/very dim
- **Level 1-6** - Increasing brightness
- **Level 7** - Maximum brightness

**How to Change:**
- Use the web interface **Settings** tab
- Use the brightness slider or dropdown

**Tip:** Level 3-4 works well during the day, Level 1-2 is good for nighttime.

### Color

Choose from preset colors or set your own:
- Red
- Green
- Blue
- Cyan (blue-green)
- Yellow
- Magenta (pink-purple)

**How to Change:**
- Use the web interface **Settings** tab
- Or use the button menu: Short press **Mode** to the Color menu, then use **Plus/Minus** to change colors

### Timezone

Make sure your clock shows the right time by setting your timezone:
- Use the web interface **Settings** tab
- Select your timezone from the dropdown list
- The clock will automatically adjust for daylight saving time

### Night Mode

Automatically reduce brightness during nighttime hours.

**How to Set Up:**

**Using the Web Interface:**
- Go to the **Night Mode** tab (🌙)
- Check "Enable Night Mode"
- Set start hour (when to dim) - default: 22:00 (10 PM)
- Set end hour (when to brighten) - default: 07:00 (7 AM)
- Choose night brightness level (0-7)
- Optionally enable/disable effects during night mode

**Using the Button Menu:**
1. Short press **Mode** to navigate to the night mode settings:
   - Night Mode - Turn on/off
   - Night Start Hour - Set start hour (0-23)
   - Night End Hour - Set end hour (0-23)
   - Night Brightness - Set brightness level (0-7)
   - Night Effects - Enable/disable effects
2. Use **Plus/Minus** to adjust each setting

**Tip:** Night mode is perfect for bedrooms. Set it to automatically dim at bedtime and brighten in the morning.

---

## Visual Effects

Your WordClock can show fun animations when the time changes!

### Types of Effects

**Quick Transitions** (less than 2 seconds):
- **Random** - Letters light up randomly
- **Line** - A line sweeps across
- **Shift** - Time slides in from the side
- **Bounce** - Bouncing animation

**Long Animations** (2-10 seconds):
- **Snake** - Classic snake game animation
- **Snow** - Falling snowflakes
- **Matrix** - Matrix movie falling letters
- **Firework** - Firework explosion
- **And more!**

### When to Show Effects

**Using the Web Interface:**
Open the **Effects** tab and choose:

- **OFF** - No effects (time changes instantly)
- **Transitions Only** - Quick effects every minute
- **Animations Hourly** - Big animation at the top of each hour
- **Animations Every 15 Min** - Big animation at :00, :15, :30, :45
- **Animations Every 5 Min** - Big animation every 5 minutes
- **Animations Only** - Always show big animations

**Using the Button Menu:**
1. Short press **Mode** until you reach the Animation Mode menu
2. Use **Plus** or **Minus** to cycle through the options:
   - No effects (instant changes)
   - Quick transitions only
   - Animations every hour
   - Animations every 15 minutes
   - Animations every 5 minutes
   - Always show animations

### Turning Effects On/Off

In the **Effects** tab, you can check or uncheck individual effects. The clock will randomly choose from the effects you have enabled.

If you uncheck all effects, the time will change instantly with no animation.

---

## Firmware Updates

Keep your WordClock up to date with the latest features and improvements.

### Easy Automatic Updates (Recommended)

**Method 1: Using the Button Menu** (Easiest!)

1. When an update is available, a Firmware Update option will appear in the button menu
2. Short press **Mode** until you reach the Firmware Update menu
3. Press **Plus** to start the update
4. Watch the green progress bar on the LED matrix
5. The clock will restart automatically when done

**Method 2: Using the Web Interface**

1. Open the web interface
2. Go to the **Firmware** tab (🔄)
3. The page will automatically check if a new version is available
4. If an update is ready, you'll see:
   - Your current version
   - The new version number
   - An "Update to Latest Version" button
5. Click the button
6. Wait for the progress bar to reach 100%
7. The clock will restart with the new version

**Both methods automatically download and install the latest firmware - no files to download or cables to connect!**

### Manual Update (Advanced)

If you have a custom firmware file (`.bin` file):

1. Open the web interface
2. Go to the **Firmware** tab
3. Scroll to "Manual File Upload"
4. Click "Choose File" and select your `.bin` file
5. Click "Upload Firmware"
6. Wait for the upload to complete
7. The clock will restart

### Important

- ⚠️ **Do not unplug the clock during an update!**
- The LED matrix will show a green progress bar
- If something goes wrong, the clock will automatically go back to the previous version
- Updates usually take 1-2 minutes

---

## Troubleshooting

### Clock Won't Connect to WiFi

**Check:**
- Is the WiFi password correct?
- Is the clock close enough to your router?
- Does your router use 2.4GHz? (The clock doesn't work with 5GHz-only networks)

**Try:**
- Restart your router
- Move the clock closer to the router
- Re-enter the WiFi password in the web interface
- Long press the Mode button to re-enter WiFi setup

### Clock Shows Wrong Time

**Check:**
- Is the clock connected to WiFi? (It needs internet to sync time)
- Is the timezone set correctly?

**Try:**
- Open the web interface and check the timezone setting
- Restart the clock (unplug and plug back in)

### Clock is Too Bright or Too Dim

**Solution:**
- Open the web interface
- Go to **Settings** tab
- Adjust the brightness slider
- Or use Night Mode to automatically dim at certain times

### Can't Access the Web Interface

**Try:**
- Make sure your phone/computer is on the same WiFi network as the clock
- Use the button menu to check the IP address
- Try typing the IP address exactly as shown
- Restart the clock

### Display is Frozen

**Try:**
- Restart the clock (unplug for 10 seconds, then plug back in)
- Check if the web interface still works
- If still frozen, see Recovery Mode below

### Buttons Don't Work

**Check:**
- Are the buttons pressed firmly?
- Try short pressing **Mode** to cycle through menus
- Try using **Plus** or **Minus** buttons to change values
- The menu times out after 30 seconds - short press **Mode** again to re-open
- Try long pressing **Mode** to enter WiFi setup mode

### Update Failed

**Try:**
- Check your internet connection
- Make sure the clock is connected to WiFi
- Try the web interface method instead
- Wait a few minutes and try again

### Recovery Mode (Advanced)

If nothing else works, you may need to reflash the firmware using a USB cable. Contact support or see the technical documentation for details.

---

## Home Assistant Integration

*This section is for users who have Home Assistant for smart home control. If you don't use Home Assistant, you can skip this section.*

### Setup

1. Make sure you have Home Assistant with MQTT configured
2. Open the WordClock web interface
3. Go to the **Home Assistant** tab
4. Enter your MQTT broker address (usually your Home Assistant IP)
5. Enter port `1883`
6. Add username and password if needed
7. Click Save

Your WordClock will appear in Home Assistant automatically.

### What You Can Do

Once connected, you'll see your WordClock in Home Assistant:

- **Light Control** - Turn on/off, change color, adjust brightness
- **Update Status** - See when updates are available and install them
- **Font Size** - Choose Small, Regular, or Large
- **Effects** - Turn individual effects on/off
- **Scrolling Text** - Send custom messages
- **Automations** - Schedule brightness changes, send birthday messages, etc.

### Example: Morning Brightness Automation

```yaml
automation:
  - alias: "WordClock Morning Brightness"
    trigger:
      platform: time
      at: "07:00:00"
    action:
      - service: light.turn_on
        target:
          entity_id: light.wordclock_XXXXXX
        data:
          brightness: 200
```

---

## Scrolling Text

Send custom messages that scroll across your WordClock display.

### Using the Web Interface

*(Feature availability depends on firmware version)*

1. Open the web interface
2. Find the text input field
3. Type your message
4. Press Send
5. The message will scroll across the clock once
6. The clock returns to showing the time

### Using Home Assistant

If you have Home Assistant connected:

1. Find the `text.wordclock_scroll_text` entity
2. Enter your message
3. Submit
4. Watch it scroll on your clock

### Tips

- Keep messages short for best readability
- The display uses the current font size setting
- Messages scroll from right to left
- Both uppercase and lowercase letters are supported

---

**Enjoy your WordClock!**

Need more help? Check the [project repository](https://github.com/psnl/wordclock-firmware) for updates and documentation.
