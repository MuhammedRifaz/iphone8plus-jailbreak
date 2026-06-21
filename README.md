# iPhone 8 Plus — iOS 16.7.15 Jailbreak Guide (palera1n + Hacktivator)

> **A complete, real-world walkthrough for jailbreaking iPhone 8 Plus on iOS 16.7.15 — including baseband/IMEI loss bypass, activation workaround, and full tweak setup.**

---

## 📱 Device Info

| Field | Details |
|---|---|
| Device | iPhone 8 Plus |
| iOS Version | 16.7.15 |
| Jailbreak Type | Rootless |
| Jailbreak Tool | [palen1x v1.2.1](https://github.com/palera1n/palen1x/releases/tag/v1.2.1) (Live Boot Linux) |
| Activation Bypass | [Hacktivator v1.5.1](https://hackt1vator.com) |
| Package Manager | Sileo |
| Tweak Injector | ElleKit |

---

## ⚠️ Disclaimer

> This guide is for **educational purposes only**. Jailbreaking may void your warranty. You are solely responsible for any damage to your device. This guide does **not** encourage piracy — AppSync Unified is listed for sideloading purposes only.
>
> Jailbreaking is **legal** in India and many other countries. Always do your research based on your local laws.

---

## 🧩 The Problem — Baseband / IMEI Issue

This iPhone 8 Plus had a **baseband chip failure**, which caused:
- Loss of IMEI
- "No Service" shown permanently
- Unable to complete normal iOS activation (Hello screen stuck)
- iTunes activation failed
- WiFi activation failed

This is a **known hardware issue** on some iPhone 8/8 Plus units. The solution used here was **Hacktivator** — a free Windows/macOS tool that bypasses the Hello screen activation entirely.

---

## 🛠️ What You Need

### Hardware
- iPhone 8 Plus
- USB to Lightning cable (preferably Apple OEM or a quality cable — cheap cables cause DFU issues)
- A Windows PC

### Software — Download Everything Before Starting

| Tool | Version | Link |
|---|---|---|
| palen1x | v1.2.1 | [GitHub Release](https://github.com/palera1n/palen1x/releases/tag/v1.2.1) |
| Ventoy or Rufus | Latest | [ventoy.net](https://www.ventoy.net) / [rufus.ie](https://rufus.ie) |
| Hacktivator | v1.5.1 | [hackt1vator.com](https://hackt1vator.com) |
| 3uTools | Latest | [3u.com](http://www.3u.com) |
| USB Drive | 8GB+ | — |

---

## 📋 Step-by-Step Guide

### Step 1 — Reset the iPhone (Required for palen1x)

> palen1x requires the device to be in a clean state when running iOS 16+. If your phone has data on it, you must erase it first.

1. Go to **Settings → General → Transfer or Reset iPhone → Erase All Content and Settings**
2. If you can't get past the Hello screen (activation screen), see Step 2 first, then come back

---

### Step 2 — Flash palen1x to a USB Drive

1. Download **palen1x v1.2.1** ISO from the link above
2. Flash it to your USB drive using **Ventoy** or **Rufus**
   - If using Rufus: select the ISO, leave settings default, click Start
   - If using Ventoy: just copy the ISO file onto the Ventoy USB drive

---

### Step 3 — Boot into palen1x (Live Linux)

1. Plug the USB into your PC
2. Restart your PC and boot from the USB drive
   - On most PCs: press `F12`, `F10`, `F2`, or `DEL` during startup to get boot menu
   - Select your USB drive
3. palen1x will boot into a live Linux environment — **no installation needed**

---

### Step 4 — Jailbreak with palera1n (Rootless)

1. Connect your iPhone to the PC via USB while in palen1x
2. In the palen1x menu, navigate:
   ```
   palera1n → Switch → Rootless → (Press Enter) → Start
   ```
3. Follow the **on-screen DFU mode instructions** exactly:
   - Hold **Volume Down + Side button** for 5 seconds
   - Release **Side button** but keep holding **Volume Down** for another 10 seconds
   - Device enters DFU (screen goes black)
4. palera1n will now run — wait for the process to complete
5. Your iPhone will reboot — **jailbreak is done**

> ✅ After reboot you'll see the **palera1n** app on your home screen (or after activation bypass)

---

### Step 5 — Activation Bypass with Hacktivator (IMEI/Baseband Issue)

> **This step is only needed if your iPhone is stuck on the Hello/activation screen** due to IMEI loss or baseband failure.

1. Boot back into Windows (remove palen1x USB, restart PC normally)
2. Connect your jailbroken iPhone to Windows via USB
3. Open **Hacktivator v1.5.1**
4. In the **Activation** section, choose **"Hello Activation"**
5. If Hacktivator prompts you to jailbreak first — press **OK** (you've already done it)
6. Let Hacktivator complete the bypass
7. Your iPhone will pass the Hello screen ✅

---

### Step 6 — Verify with 3uTools

1. Download and open **3uTools** on Windows
2. Connect your iPhone
3. 3uTools will confirm:
   - Device model
   - iOS version
   - Jailbreak status
4. If it shows **"Jailbroken"** — you're good ✅

---

### Step 7 — Setup Sileo & Add Sources

After bypass, open the **palera1n** app on your device and complete the jailbreak environment setup. Then open **Sileo**.

Add the following repositories in Sileo → Sources → `+`:

```
https://apt.procurs.us/           (Procursus — core packages)
https://ellekit.space/            (ElleKit — tweak injector)
https://repo.palera.in/           (palera1n official)
https://repo.chariz.com/          (Chariz)
https://havoc.app/                (Havoc)
http://apt.thebigboss.org/repofiles/cydia/  (BigBoss)
https://therealhoodboy.github.io/coreux/    (CoreUX)
https://mtac.app/repo/            (MTAC's Repo)
https://sparkdev.me/              (SparkDev)
http://tigisoftware.com/repo/     (TIGI Software)
https://skitty.xyz/repo/          (Skitty's Repo)
https://ivintagelover.github.io/repo/       (iVintageRepo)
```

---

## 📦 Installed Packages

See [`packages/installed-packages.txt`](packages/installed-packages.txt) for the full list of installed packages on this device.

### Key Tweaks Installed

| Tweak | Purpose |
|---|---|
| **SnowBoard** | Icon theme engine |
| **Solid Glass 2** | iOS 26-style glassmorphism UI |
| **Vitreux** | Blur/glass effects |
| **Zetsu** | App icon customization |
| **GesturesXV** | Custom gesture controls |
| **CC26** | iOS 26-style Control Center |
| **CCSupport** | Control Center tweak support |
| **RoundDock Remastered** | Rounded dock UI |
| **VisibleIsland** | Dynamic Island style notch tweak |
| **Atria** | UI customization |
| **Choicy** | Per-app tweak toggling |
| **AppSync Unified** | Sideload unsigned IPA files |
| **TrollStore Lite** | Permanent app installation |
| **Filza File Manager** | Full filesystem access |
| **iCleaner Pro** | System cleaner |

---

## 🗂️ Repo Structure

```
iphone8plus-jailbreak/
├── README.md                  ← You are here
├── docs/
│   ├── BASEBAND-ISSUE.md      ← Explanation of the IMEI/baseband problem
│   ├── DFU-GUIDE.md           ← Detailed DFU mode instructions
│   └── TROUBLESHOOTING.md     ← Common issues and fixes
├── packages/
│   └── installed-packages.txt ← Full Sileo package list
└── screenshots/               ← Device screenshots
```

---

## ❓ FAQ

**Q: Will this work on other iPhone models?**
palera1n supports all A8–A11 devices. iPhone 6s through iPhone X on compatible iOS versions. The Hacktivator bypass is specific to activation issues.

**Q: Is this a tethered or untethered jailbreak?**
palera1n on iOS 16 is **semi-tethered** — you need to re-run palera1n after a full reboot to re-enable tweaks. A regular restart (not full power off) is fine.

**Q: My device keeps failing DFU mode. What do I do?**
Try a different USB cable. Cheap cables fail DFU entry very often. See [`docs/DFU-GUIDE.md`](docs/DFU-GUIDE.md).

**Q: Can I use this without the baseband issue?**
Yes — just skip Step 5 entirely. If your iPhone activates normally, Hacktivator is not needed.

**Q: Will OTA updates break the jailbreak?**
Yes. Do not update iOS. Disable OTA updates via a tweak or profile.

---

## 🔗 Credits & Tools Used

- [palera1n](https://github.com/palera1n/palera1n) — The jailbreak
- [palen1x](https://github.com/palera1n/palen1x) — Live boot Linux environment for palera1n
- [Hacktivator](https://hackt1vator.com) — Free activation bypass tool
- [Sileo](https://getsileo.app) — Package manager
- [ElleKit](https://ellekit.space) — Tweak injection framework
- [3uTools](http://www.3u.com) — Device verification

---

*Guide written by [Mohammed Rifaz](https://github.com/MuhammedRifaz) — tested on personal device.*
