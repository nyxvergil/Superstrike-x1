<div align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/bannerstrike.png" alt="SuperStrike Banner" width="800" height="auto">
  </picture>

  <p>
    <a href="https://github.com/nyxvergil/Superstrike-x1/releases">
      <img src="https://img.shields.io/badge/RELEASE-v1.0.1-5B21FF?style=for-the-badge&logo=windows11&logoColor=white" alt="Release v1.0.1">
    </a>
    <img src="https://img.shields.io/badge/WINDOWS-10%20%2F%2011-0d0d10?style=for-the-badge&logo=windows11&logoColor=white" alt="Windows">
    <img src="https://img.shields.io/badge/ARCH-AMD64-5B21FF?style=for-the-badge" alt="Architecture">
    <img src="https://img.shields.io/badge/ANTI--CHEAT-VANGUARD%20READY-0d0d10?style=for-the-badge&logo=riotgames&logoColor=5B21FF" alt="Anti-Cheat">
    <a href="https://discord.gg/StrikeOS">
      <img src="https://img.shields.io/badge/Discord-StrikeOS-0d0d10?style=for-the-badge&logo=discord&logoColor=white&labelColor=5B21FF" alt="Discord">
    </a>
    <a href="https://strikeos.site">
      <img src="https://img.shields.io/badge/Site-strikeos.site-0d0d10?style=for-the-badge&logo=cloudflare&logoColor=5B21FF" alt="Site">
    </a>
  </p>
</div>

---

<div align="center">

<table align="center" width="85%">
<tr>
<td width="65%" align="center">

<h2>Windows, without Microsoft's bullshit.</h2>

SuperStrike X1 is an open Windows optimization playbook for <strong>AME Wizard</strong>.

<br>

Built for <strong>rock-solid frametimes and competitive latency</strong>:
zero-placebo kernel tuning, driver interrupt balancing, and modular revert scripts.

<br>

100% opt-in. Check only what you need, uncheck what you want to keep.
Windows Defender, Riot Vanguard (CFG/DEP), and Windows Update servicing remain fully functional.
A single reboot is required after completion.

<br>

<strong>Low Latency · Frametime Consistency · Anti-Cheat Ready · Fully Reversible</strong>

</td>
<td width="35%" align="center">

<img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/playbook_cube.png" width="200" alt="SuperStrike Playbook">

</td>
</tr>
</table>

</div>

---

> [!NOTE]
> **Zero-Placebo Guarantee.** No broken registry cache tricks or forced MPO disabling. Every tweak is targeted at measurable DPC latency and background thread contention.

---

## 1. Verified Telemetry & Benchmark

Tested on identical hardware across a repeatable 60-second capture loop in **GTA5VN / FiveM (`GTASVN_GameProcess.exe`)**:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/benchmark.png" width="820" alt="Frame-Time Analysis Benchmark Data">
</p>

| Telemetry Metric | Stock Windows (Before) | SuperStrike X1 (After) | Improvement |
| :--- | :---: | :---: | :---: |
| **Average FPS** | 174.61 FPS | **253.61 FPS** | **+45.2%** |
| **1% Low FPS (Stutter Metric)** | 20.66 FPS | **173.88 FPS** | **+741.6%** (Eliminated hitching) |
| **Minimum FPS** | 16.98 FPS | **83.81 FPS** | **+393.5%** |
| **Frametime Deviation (StDev)** | 32.18 ms | **27.19 ms** | **-4.99 ms** (Tighter pacing) |
| **Total Frames Rendered (60s)** | 10,478 frames | **15,217 frames** | **+4,739 frames** |
| **Idle Process Count** | 160–180+ | **~70–85** | ~55% reduction |

---

## 2. Core Optimizations

- **SvcHost Memory Consolidation:** Groups 160+ fragmented background services into shared host processes, sharply reducing CPU context-switching overhead.
- **Hardware & Network Latency:** Disables network card power throttling (EEE, Green Ethernet) and packet coalescing (LSO, RSC) for instant packet delivery. Sets dedicated High-Priority MSI vector interrupts on GPU and NIC.
- **Dynamic Memory Gating:** Safely locks the kernel executive on systems with $\ge$ 12GB RAM to eliminate sudden paging pauses; keeps stock paging safe on low-RAM systems.
- **DirectFlip & WDDM 3.0+ Compliant:** Retains Hardware-Accelerated GPU Scheduling (HAGS) and native DirectFlip presentation. Zero broken MPO overrides.
- **Managed Defender Impact:** Retains Defender protection while capping scanning CPU factor to 15% and excluding common game archive packages.

---

## 3. Desktop & Visual Preset

Trims unnecessary window animations and slide transitions while keeping high-DPI text readability and explorer usability:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/visual_effects_preset.png" width="380" alt="Visual Effects Configuration">
</p>

*Preserves ClearType font smoothing, media thumbnails, and icon shadows. Eliminates UI render lag.*

---

## 4. Configuration Pages (AME Wizard)

All checkboxes are **unchecked by default**. Nothing is removed without your explicit choice:

| Page | Section | Options | Default |
| :---: | :--- | :--- | :---: |
| **1** | Optimization Profile | `Performance` / `Standard` | Performance |
| **2** | System App Removals | `Microsoft Edge`, `Microsoft OneDrive`, `Xbox & Game Bar` | Opt-in |
| **3** | Modern AI & Feeds | `Widgets & News Feed`, `Copilot, Recall & Windows AI` | Opt-in |
| **4** | Desktop & UI | `Disable Transparency`, `Classic Context Menu (Win 10)` | Opt-in |
| **5** | Peripherals & Services | `Search Indexing`, `Bluetooth`, `Print Spooler`, `Touch Keyboard` | Opt-in |
| **6** | Web Browser | `None`, `Brave`, `Mozilla Firefox`, `Google Chrome` | Brave (Selectable) |

---

## 5. Desktop vs Laptop Adaptation

SuperStrike automatically detects chassis type at setup time:

| Feature | Desktop Implementation | Laptop Implementation |
| :--- | :---: | :---: |
| **AC Power Plan** | High Performance (100% Unparked Cores) | Dynamic Gaming Scheme |
| **Battery (DC) Profile** | N/A | Balanced (Battery-Safe) |
| **D3Cold & USB Power Saving** | Disabled (Zero peripheral latency) | Preserved (Prevents idle drain) |
| **Display Acceleration** | HAGS + Dedicated GPU Focus | HAGS + Hybrid Switching Safe |

---

## 6. PostInstall Revert Tools

Every modification includes an instant one-click toggle script located in `C:\Users\Public\Desktop\PostInstall\`:

| Tool | Action |
| :--- | :--- |
| `Toggle-Power-Plan.bat` | Switch between Ultimate, High, and Balanced power schemes |
| `Toggle-VBS-Core-Isolation.bat` | Enable or disable Virtualization-Based Security (VBS / HVCI) |
| `Toggle-Windows-Defender.bat` | Toggle Real-time Protection and Cloud Sample Submission |
| `Toggle-Windows-Update.bat` | Toggle Windows Update and Delivery Optimization background tasks |
| `Toggle-MPO-HAGS.bat` | Inspect and toggle Multi-Plane Overlay (MPO) and HAGS states |
| `DirectFlip-CPU-Hybrid.bat` | Inspect DirectFlip presentation and CPU thread scheduling hooks |
| `Toggle-WiFi-Bluetooth.bat` | Instantly restore wireless, Bluetooth, and device pairing services |
| `Toggle-Print-Spooler.bat` | Instantly restore printer spooler service dependencies |
| `Restore-Visual-Effects.bat` | Reset all Windows animations and visual effects to default |

---

## 7. How to Install

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/1.PNG" width="410" alt="SuperStrike in AME Wizard">
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/2.PNG" width="410" alt="Options Selection">
</p>

1. Download `Superstrike-x1.apbx` from [Releases](https://github.com/nyxvergil/Superstrike-x1/releases) and [AME Wizard Beta](https://download.ameliorated.io/AME%20Beta.zip).
2. Launch `AME Wizard.exe` as Administrator.
3. Drag and drop `Superstrike-x1.apbx` into the window (password: `malte` if prompted).
4. Select your preferred options and click **Next**.
5. Reboot your system once the setup completes.

---

## 8. Anti-Cheat & System Compatibility

### 100% Anti-Cheat Certified
Operates purely on valid Windows configuration layers. Crucial security mechanisms (CFG, DEP, driver signing) remain intact:
- **Riot Vanguard** (VALORANT, League of Legends)
- **Easy Anti-Cheat** (Fortnite, Apex Legends, Rust)
- **BattlEye** (Rainbow Six Siege, PUBG, Destiny 2)
- **FACEIT Anti-Cheat** (CS2)
- **Ricochet** (Call of Duty: Warzone)

### Supported Builds (AMD64 / x64)

<p align="center">
  <img src="https://img.shields.io/badge/Windows%2010-22H2%20(Build%2019045)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 10 22H2">
  <img src="https://img.shields.io/badge/Windows%2011-23H2%20(Build%2022631)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 23H2">
  <img src="https://img.shields.io/badge/Windows%2011-24H2%20(Build%2026100)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 24H2">
  <img src="https://img.shields.io/badge/Windows%2011-25H2%20(Build%2026200)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 25H2">
</p>

---

## 9. Frequently Asked Questions

<details>
<summary><strong>Why is VBS (Virtualization-Based Security) disabled by default?</strong></summary>

Memory Integrity (HVCI) and VBS introduce CPU virtualization overhead, reducing 1% Low framerates by 5% to 15% in CPU-bound competitive games. It is turned off by default for maximum frametime smoothness, but can be restored anytime via `Toggle-VBS-Core-Isolation.bat`.
</details>

<details>
<summary><strong>Does SuperStrike break Windows Update?</strong></summary>

No. The Windows servicing stack is preserved. If you want to pause or disable background driver updates, use `Toggle-Windows-Update.bat` in PostInstall.
</details>

<details>
<summary><strong>What if I need Bluetooth, Wi-Fi, or Printing?</strong></summary>

Keep their checkboxes unchecked during setup. If already applied, run `Toggle-WiFi-Bluetooth.bat` or `Toggle-Print-Spooler.bat` from PostInstall to restore them instantly.
</details>

---

## Links & Verification

<p align="center">
  <a href="https://strikeos.site">
    <img src="https://img.shields.io/badge/Website-strikeos.site-5B21FF?style=flat-square&logo=googlechrome&logoColor=white" alt="Website">
  </a>
  <a href="https://discord.gg/StrikeOS">
    <img src="https://img.shields.io/badge/Discord-StrikeOS-5B21FF?style=flat-square&logo=discord&logoColor=white" alt="Discord">
  </a>
  <a href="https://github.com/nyxvergil/Superstrike-x1">
    <img src="https://img.shields.io/badge/GitHub-Superstrike--x1-0d0d10?style=flat-square&logo=github&logoColor=white" alt="GitHub">
  </a>
</p>

```
SHA256: 00B7EC7999CC0792D25EC5628F44AE3823ADE0B66546A1EA156EF5B74E884EA4  Superstrike-x1.apbx
```

<p align="center">
  <sub>© 2026 StrikeOS · SuperStrike X1 · Zero-Placebo Optimization Architecture</sub>
</p>
