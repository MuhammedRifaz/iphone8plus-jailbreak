# DFU Mode Guide — iPhone 8 Plus

DFU (Device Firmware Update) mode is required for palera1n to work. It's the deepest low-level mode an iPhone can enter, bypassing the bootloader.

---

## iPhone 8 Plus — DFU Entry Steps

Follow these steps **exactly as shown on the palen1x screen** when prompted:

1. Make sure your iPhone is **connected to the PC via USB**
2. Press and hold **Volume Down + Side (Power) button** together for **10 seconds**
3. After 10 seconds, **release only the Side button** — keep holding **Volume Down**
4. Hold **Volume Down** for another **5 seconds**
5. The screen should go **completely black** — that's DFU mode ✅

> If the Apple logo appears, you went too fast or too slow. Try again from Step 1.

---

## How to Tell You're in DFU Mode

- Screen is **completely black** (no Apple logo, no text)
- 3uTools or iTunes will show **"iPhone in recovery mode"** or **"DFU mode detected"**
- palen1x will detect the device automatically

---

## Common Problems

### Cable Issues (Most Common)
Cheap Lightning cables frequently fail DFU entry. If you keep failing:
- Try a different, higher-quality cable
- Try a different USB port (USB 2.0 ports sometimes work better than USB 3.0)
- Avoid USB hubs — connect directly to the PC

### Timing Issues
- The timing needs to be precise — not too fast, not too slow
- Practice the button combo a couple times before actually running palera1n
- Some people find it easier to count out loud: "1, 2, 3... 10, release Side, 1, 2, 3, 4, 5"

### Device Reboots Into Normal Mode
- You held the Side button too long in Step 3
- Start over from Step 1

### Screen Flashes Apple Logo Then Goes Black
- That's normal — keep holding, DFU mode is being entered

---

## Recovery Mode vs DFU Mode

| | Recovery Mode | DFU Mode |
|---|---|---|
| Screen | Shows iTunes/cable logo | Completely black |
| Used for | iTunes restore | palera1n jailbreak |
| How to exit | Hold Side + Volume Down until Apple logo | Same |

palera1n requires **DFU mode**, not Recovery mode.

---

*Part of the [iPhone 8 Plus Jailbreak Guide](../README.md) by Mohammed Rifaz*
