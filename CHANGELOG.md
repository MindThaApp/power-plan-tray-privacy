# Power Plan Manager — What's new

Release notes for Power Plan Manager Pro and Lite on the Microsoft Store.

## Pro 1.0.16.0 / Lite 1.0.9.0

**No separate downloads needed**
- The app now includes everything it needs to run. You no longer need to install the .NET Desktop Runtime.
- Sensor readings come only from the app's own built-in helper. The app no longer offers to install or start a separate hardware monitor, and it no longer runs a web server for one.

**Fan safety**
- A hot graphics card now always spins its own fans to full speed, including at 90 °C and above on the GPU core. The app decides which fans belong to the graphics card from the hardware itself.
- If a temperature sensor stops responding, the fans go to full speed instead of following the last reading.
- An overheat now holds until the temperature has actually dropped. A sensor that stops responding no longer counts as "cooled down".
- Graphics memory and voltage-regulator temperatures now have their own safe limits, so they no longer cause needless fan noise.

**Security**
- Changing which power settings are hidden no longer runs a temporary script file with admin rights.
- A charging change requested by another app now always asks you first, one request at a time.

**Automation**
- Other apps can see whether a request worked, and can follow changes as they happen (power plan, preset, charge limit, Keep Awake, battery events). This is read-only, and only when "Allow links from other apps" is on.
- Keep Awake can now run for 30, 60 or 120 minutes, or any number of minutes when another app sets it.
- New link actions: next plan, and cycle power mode.
- The Automation page lists your rules first and offers starter rules, which are added switched off.
- There is a log of requests from other apps. A plan switch made by another app can be undone.

**Easier to use**
- Clearer page names: Energy history, Tariff & meter, Switch history, Windows power mode, Appearance.
- The tray popup opens tall enough to show all your widgets, up to near the top of the screen. A height you set yourself is kept.
- The Pro trial shows how many days are left. You get one reminder 3 days before it ends, and one summary when it ends.
- "Switch back" in switch history, better screen-reader labels, and fixes for text cut off in the tray popup and on the Fans page.
- Fixed: hiding a power plan in the plan list didn't save.
- Confirmation dialogs now treat Enter as Cancel.

## Pro 1.0.15.0 / Lite 1.0.8.0

- Power Plan Manager Pro is now free, with a 30-day trial of Pro features and an optional one-time Pro unlock afterward.
  Anyone who already purchased Pro keeps full access automatically, with nothing to do.
- Power flow: the detailed breakdown of power by part (CPU, GPU, memory, storage and so on) is now a Pro feature. Everyone
  still sees total live power draw either way.
- Added hardware compatibility details for fan control and battery charge limit to the Store listing, so you know before
  buying whether your PC supports them.
- Security and reliability: hardened the elevated fan-control helper against tampering, safer checks on the app's data
  folder, and built-in power plans now back themselves up before being removed so they can always be restored.

## Pro 1.0.13.0 / Lite 1.0.7.0 and earlier updates

- Fan control, sensor logging and battery tools kept improving: stale-sensor fail-safes, a read-only status pipe for
  third-party automation tools, and a safer picker for which fan engine controls your fans.
- Smaller fixes across the Power, Fans and Battery pages.

## Pro 1.0.12.0 / Lite 1.0.6.0 — 21 October 2026

A big update with a fresh new look.

**New**
- New design: frosted glass surfaces, calmer colours and grouped navigation. Colours are adjustable.
- Power flow: watch your PC's power travel from the wall or battery to the CPU, graphics card and other parts, live.
  Click a part to expand it.
- New tray popup: tiles you can arrange, resize and hide, including a power flow tile. Separate layouts for the
  left-click and right-click popups. Change the tray icon from the popup.
- Desktop power page: real CPU and GPU watts, plus readings from smart plugs on your network. *(Pro)*
- Battery care for laptops: battery health, design and current capacity, voltage, charge reminders, and a charge limit
  on supported Lenovo laptops. *(Charge limit: Pro)*
- Energy costs and history with your own tariff. *(Pro)*
- Fan control and a Sensors page, through an optional helper. Fans are handed back to the motherboard when you exit.
  *(Pro)*
- Schedules, keyboard shortcuts, presets and switch history. *(Pro)*
- Plain-language descriptions for advanced power settings.
- Now in 50 languages.
- What's new screen after each update, and Send feedback in About.
- Optional crash reports: nothing is sent without your consent. See the [privacy policy](README.md).

**Fixes**
- Many smaller fixes and stability improvements, including safer recovery after a crash.

## Earlier versions

Power Plan Manager started as a simple tray utility for switching power plans, and grew battery care, fan control,
energy tracking, automation and the current design over many smaller releases.
