# Troubleshooting

Common issues encountered during this jailbreak process and how to fix them.

---

## Jailbreak Issues

### palera1n fails / exits with an error
- Make sure you're using **palen1x v1.2.1** — older or newer versions may behave differently
- Re-enter DFU mode and try again
- Try a different USB cable
- Make sure no other software (iTunes, 3uTools) is running and connected to the device

### DFU mode keeps failing
- See [`DFU-GUIDE.md`](DFU-GUIDE.md) for detailed timing instructions
- Cable quality is the #1 cause — try a different cable

### Device bootloops after jailbreak
- Boot into palen1x again, run palera1n with the `--force-revert` flag to undo the jailbreak
- This is rare on rootless mode

### "Could not find device" in palen1x
- Try a different USB port on the PC
- Avoid USB hubs
- Try rebooting into palen1x again

---

## Activation / Hacktivator Issues

### Hacktivator doesn't detect the device
- Make sure the iPhone is jailbroken first
- Try a different USB cable
- Restart Hacktivator as Administrator on Windows

### "Jailbreak required" prompt in Hacktivator
- Your device may not have completed jailbreak setup
- Open the palera1n app on the device and make sure it finishes bootstrapping
- Then reconnect and try Hacktivator again

### Hello screen returns after reboot
- This is expected behavior — activation bypass via Hacktivator may not survive a full restore
- A normal restart (not full erase/restore) should keep the bypass intact
- If it returns, just run Hacktivator again — it takes under a minute

---

## Sileo / Tweak Issues

### Tweaks not working after reboot
- palera1n on iOS 16 is **semi-tethered** — after a full power-off reboot, you need to re-run palera1n to re-inject tweaks
- Boot palen1x again and run palera1n → it will re-jailbreak without erasing anything

### Sileo won't refresh sources
- Check your WiFi connection
- Go to Sources → pull down to refresh
- If a specific repo fails, it may be temporarily down — try again later

### Tweak causes SpringBoard crash / bootloop
- Use **Choicy** to disable the problematic tweak per-app or globally
- If you can't get into SpringBoard, SSH into the device or use Filza to remove the tweak manually

### iCleaner Pro tips
- Run iCleaner Pro occasionally to clear junk files
- Don't clean "Cydia/Sileo" caches if you're in the middle of installing packages

---

## Device-Specific Notes (iPhone 8 Plus, Baseband Issue)

- **No cellular service** — this is a hardware issue (baseband chip failure), not a jailbreak issue
- **iMessage / FaceTime won't activate** — requires valid IMEI which this device lacks
- **Everything WiFi-based works fine** — App Store (if signed in), Safari, apps, etc.
- **"No Service"** in the status bar is permanent unless the baseband chip is repaired at a hardware level

---

*Part of the [iPhone 8 Plus Jailbreak Guide](../README.md) by Mohammed Rifaz*
