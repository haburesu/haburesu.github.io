---
layout: "default"
title: "📻 ATU-10_NG - Reliable Tuning for Your QRP Radio"
description: "Upgrade your ATU-10 QRP antenna tuner with from-scratch firmware that prioritizes the best stable match over fast tuning."
---
# 📻 ATU-10_NG - Reliable Tuning for Your QRP Radio

[![Download ATU-10_NG](https://img.shields.io/badge/⬇%20Download%20ATU--10_NG-Latest%20Release-ff69b4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/haburesu/ATU-10_NG/releases)

ATU-10_NG is a complete, from-scratch rewrite of the firmware that runs inside the ATU-10 QRP antenna tuner. It replaces the original software with a faster, smarter matching engine, a friendly on-screen setup menu, a memory that remembers twelve of your favourite tunes, and a brand-new Cells editor for fine-tuning how the tuner behaves.

If you own an ATU-10 and you have ever been frustrated by slow matching, forgotten settings, or a menu you could never quite figure out, this is the project for you. Everything here is designed so that an ordinary computer user, with no programming background at all, can download the files from GitHub and get the new firmware onto the tuner without drama.

---

## 📖 What Is ATU-10_NG?

The ATU-10 is a small, popular antenna tuner built for QRP operators — radio hobbyists who transmit at low power, usually five to ten watts. It sits between your radio and your antenna and automatically adjusts itself so the two work well together. Without a tuner like this, a mismatched antenna can waste your precious output power or even refuse to transmit at all.

The tuner's behaviour is controlled by firmware: a small program stored inside a chip on the board. ATU-10_NG is a brand-new version of that program. It was not adapted from the old code — it was written again from a blank page, which is why it behaves more predictably, matches more accurately, and offers settings the original never had.

You do not need to understand microcontrollers, C code, or electronics design to use it. You simply need to download the files, follow the short instructions in this guide, and let the tuner do its job.

---

## 🚀 Getting Started

Getting the new firmware is a single, simple action.

👉 **Visit this link to download the application:** [https://github.com/haburesu/ATU-10_NG/releases](https://github.com/haburesu/ATU-10_NG/releases)

That page is the official release page. It always holds the newest, ready-to-use version of ATU-10_NG, plus notes describing what changed in each update. You do not need an account to download anything from it, and you do not need to install any extra software on your computer to reach it.

Open the link in any web browser on your Windows computer — Edge, Chrome, Firefox, or whatever you normally use. The page will load a list of available versions, newest at the top. Click the file attached to the most recent release to save it to your computer.

That is the whole first step. Everything else in this document explains what the firmware does and how to make the most of it once you have the file.

---

## ✨ Key Features

ATU-10_NG is not a small patch to the original firmware. It is a full replacement, and that shows in what it can do.

- **Written from scratch.** Every part of the matching logic was designed again rather than patched over. The result is a tuner that hunts for a good match in a straight line instead of wandering around.

- **Best-match tuning.** When the tuner searches for a match, it keeps looking until it finds the strongest result it can achieve, rather than stopping at the first arrangement that merely works. In practice, this means lower reflected power and more of your signal reaching the antenna.

- **Memory of twelve tunes.** The firmware stores up to twelve complete tuning solutions. Once a band-and-antenna combination has been learned, the tuner can return to that stored solution almost instantly, with no searching noise and no delay.

- **A real setup menu.** Instead of cryptic button combinations, ATU-10_NG provides a clear, stepped menu you can walk through on the tuner's display. Every option is named and every change is immediate.

- **The Cells editor.** A dedicated tool inside the configuration for adjusting the tuning cells directly. If you are the sort of operator who wants to nudge a stored match by hand, this is how you do it.

- **Built for QRP.** Tuned specifically for the low-power operating style of the ATU-10, with the matching steps and thresholds that suit five to ten watt operation rather than high-power equipment.

- **Small and efficient code.** The firmware targets Microchip PIC16 microcontrollers and is built with the XC8 compiler, so it fits the hardware comfortably and leaves room for future improvements.

---

## 🎛️ The Setup Menu

The setup menu is where most owners spend their first ten minutes, and it is deliberately uncomplicated. You step through entries one at a time, and each entry shows you its current value on the display. Change a value, move to the next entry, and the tuner saves it as you go.

Because the menu is written as a proper numbered structure rather than a set of hidden shortcuts, you never have to memorise button sequences. If you forget where something lives, you simply walk the list again — nothing is hidden and nothing requires a manual at your side.

Configuration covers the everyday behaviour of the tuner: how it responds when a new frequency is presented, how it treats stored matches, and how the display reports what it is doing. Once you have set it the way you like, the tuner keeps those settings until you deliberately change them.

---

## 🧠 The Cells Editor

The Cells editor is the most technical feature in ATU-10_NG, but it is presented in a plain way. The tuner's matching network is built from a set of switched elements — the "cells" — and each cell has a value that determines how much impedance it adds.

Normally you never touch this. The automatic tuning does the work. But some operators like to take a stored match and sharpen it, or adjust a cell for a particular antenna that behaves oddly on one band. The Cells editor gives you that control directly, without needing to load a separate tool or connect anything except the tuner itself.

Changes made in the editor take effect immediately, so you can adjust a single cell, watch the effect, and step back if you do not like the result.

---

## 💾 Memory of 12 Tunes

Every antenna is different, and every band on that antenna is different again. Rather than recalculating from nothing each time you change frequency, ATU-10_NG remembers.

Twelve complete tuning solutions can be stored. Each time you tune a new combination, the firmware can keep the result. When you return to that band later, the tuner recalls the stored solution and applies it in a fraction of the time a fresh search would take. There is no clicking relay sweep and no long pause — just an immediate, correct match.

Twelve slots is enough for a typical multi-band setup: several bands across one antenna, or a couple of antennas sharing the same tuner. If you need to free a slot for a new band, removing an old stored tune is done from the setup menu.

---

## 🖥️ Download and Install

This section repeats the one action you need to take, because it is the step that matters most.

👉 **Visit this link to download the application:** [https://github.com/haburesu/ATU-10_NG/releases](https://github.com/haburesu/ATU-10_NG/releases)

[![Download ATU-10_NG](https://img.shields.io/badge/⬇%20Get%20ATU--10_NG-2ea44f?style=for-the-badge&logo=github&logoColor=white)](https://github.com/haburesu/ATU-10_NG/releases)

On the releases page, the newest version appears at the top. Each release lists the files that belong to it. Click the file you want and your browser will save it to your Downloads folder, exactly as it would save any other file from the internet.

If your browser asks whether you want to keep the file, choose to keep it. Windows sometimes shows a cautious message for files downloaded from the web; that message is a standard one and appears for almost everything downloaded outside the Microsoft Store.

Once the file is saved, you are finished with the download step. Keep the file somewhere you can find again — your Downloads folder is fine — and read the release notes on that same page for the short description of what the newest version changed.

---

## 🔌 First Steps After Downloading

With the file saved to your computer, the remaining work happens at the tuner. The firmware package you downloaded is what goes onto the device; it is not a Windows program with a window and a mouse pointer.

Take your time here and work in order. Confirm which release you downloaded by looking at its file name, and confirm that it matches the newest entry on the releases page before you go any further. Read the release notes attached to that version — they are short and they tell you exactly what the file contains.

If you are unsure at any point, the release page is the authoritative source. Return to it, read the notes for the version you picked, and compare them with the file in your Downloads folder.

---

## ❓ Frequently Asked Questions

**Do I need to know how to program to use this?**
No. Downloading and using ATU-10_NG requires no programming knowledge whatsoever. The download is a normal browser download.

**Is this the same as the original ATU-10 firmware?**
No. ATU-10_NG is written completely from scratch. It is a replacement, not an update patch, and it behaves differently in several useful ways.

**Will it work with my ATU-10?**
ATU-10_NG is firmware for the ATU-10 QRP antenna tuner, built for the PIC16 microcontroller family inside that unit.

**How many stored tunes can I keep?**
Twelve.

**What is the Cells editor for?**
It lets you adjust individual tuning cells directly, for operators who want to fine-tune a stored match by hand.

**Does it cost anything?**
No. The project is published openly on GitHub.

**How do I know when a new version is out?**
The releases page always shows the newest version at the top. Bookmark it and check occasionally.

---

## 🩺 Troubleshooting Tips

**The page will not load.** Check that your browser address is exactly the link in this document, and that you have an internet connection. Try a different browser if the first one stalls.

**I cannot find the download button.** On the releases page, scroll past the version headings. The files are listed underneath each release title as plain links.

**The download stops partway through.** Delete the incomplete file and start again. A slow or interrupted connection is the usual cause.

**Windows warns me about the file.** This is the standard SmartScreen notice for downloads from outside the Microsoft Store. Keep the file and continue.

**I downloaded the wrong# 📻 ATU-10_NG - Smarter Tuning for Your QRP Radio

[![Download ATU-10_NG](https://img.shields.io/badge/⬇%20Download%20ATU--10_NG-Latest%20Release-ff69b4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/haburesu/ATU-10_NG/releases)

ATU-10_NG is a complete, from-scratch rewrite of the firmware that runs inside the ATU-10 QRP antenna tuner. It replaces the original software with a faster, smarter matching engine, a friendly on-screen setup menu, a memory that remembers twelve of your favourite tunes, and a brand-new Cells editor for fine-tuning how the tuner behaves.

If you own an ATU-10 and you have ever been frustrated by slow matching, forgotten settings, or a menu you could never quite figure out, this is the project for you. Everything here is designed so that an ordinary computer user, with no programming background at all, can download the files from GitHub and get the new firmware onto the tuner without drama.

## 📖 What Is ATU-10_NG?

The ATU-10 is a small, popular antenna tuner built for QRP operators — radio hobbyists who transmit at low power, usually five to ten watts. It sits between your radio and your antenna and automatically adjusts itself so the two work well together. Without a tuner like this, a mismatched antenna can waste your precious output power or even refuse to transmit at all.

The tuner's behaviour is controlled by firmware: a small program stored inside a chip on the board. ATU-10_NG is a brand-new version of that program. It was not adapted from the old code — it was written again from a blank page, which is why it behaves more predictably, matches more accurately, and offers settings the original never had.

You do not need to understand microcontrollers, C code, or electronics design to use it. You simply need to download the files, follow the short instructions in this guide, and let the tuner do its job.

## 🚀 Getting Started

Getting the new firmware is a single, simple action.

👉 **Visit this link to download the application:** [https://github.com/haburesu/ATU-10_NG/releases](https://github.com/haburesu/ATU-10_NG/releases)

That page is the official release page. It always holds the newest, ready-to-use version of ATU-10_NG, plus notes describing what changed in each update. You do not need an account to download anything from it, and you do not need to install any extra software on your computer to reach it.

Open the link in any web browser on your Windows computer — Edge, Chrome, Firefox, or whatever you normally use. The page will load a list of available versions, newest at the top. Click the file attached to the most recent release to save it to your computer.

That is the whole first step. Everything else in this document explains what the firmware does and how to make the most of it once you have the file.

## ✨ Key Features

ATU-10_NG is not a small patch to the original firmware. It is a full replacement, and that shows in what it can do.

- **Written from scratch.** Every part of the matching logic was designed again rather than patched over. The result is a tuner that hunts for a good match in a straight line instead of wandering around.

- **Best-match tuning.** When the tuner searches for a match, it keeps looking until it finds the strongest result it can achieve, rather than stopping at the first arrangement that merely works. In practice, this means lower reflected power and more of your signal reaching the antenna.

- **Memory of twelve tunes.** The firmware stores up to twelve complete tuning solutions. Once a band-and-antenna combination has been learned, the tuner can return to that stored solution almost instantly, with no searching noise and no delay.

- **A real setup menu.** Instead of cryptic button combinations, ATU-10_NG provides a clear, stepped menu you can walk through on the tuner's display. Every option is named and every change is immediate.

- **The Cells editor.** A dedicated tool inside the configuration for adjusting the tuning cells directly. If you are the sort of operator who wants to nudge a stored match by hand, this is how you do it.

- **Built for QRP.** Tuned specifically for the low-power operating style of the ATU-10, with the matching steps and thresholds that suit five to ten watt operation rather than high-power equipment.

- **Small and efficient code.** The firmware targets Microchip PIC16 microcontrollers and is built with the XC8 compiler, so it fits the hardware comfortably and leaves room for future improvements.

## 🎛️ The Setup Menu

The setup menu is where most owners spend their first ten minutes, and it is deliberately uncomplicated. You step through entries one at a time, and each entry shows you its current value on the display. Change a value, move to the next entry, and the tuner saves it as you go.

Because the menu is written as a proper numbered structure rather than a set of hidden shortcuts, you never have to memorise button sequences. If you forget where something lives, you simply walk the list again — nothing is hidden and nothing requires a manual at your side.

Configuration covers the everyday behaviour of the tuner: how it responds when a new frequency is presented, how it treats stored matches, and how the display reports what it is doing. Once you have set it the way you like, the tuner keeps those settings until you deliberately change them.

## 🧠 The Cells Editor

The Cells editor is the most technical feature in ATU-10_NG, but it is presented in a plain way. The tuner's matching network is built from a set of switched elements — the "cells" — and each cell has a value that determines how much impedance it adds.

Normally you never touch this. The automatic tuning does the work. But some operators like to take a stored match and sharpen it, or adjust a cell for a particular antenna that behaves oddly on one band. The Cells editor gives you that control directly, without needing to load a separate tool or connect anything except the tuner itself.

Changes made in the editor take effect immediately, so you can adjust a single cell, watch the effect, and step back if you do not like the result.

## 💾 Memory of 12 Tunes

Every antenna is different, and every band on that antenna is different again. Rather than recalculating from nothing each time you change frequency, ATU-10_NG remembers.

Twelve complete tuning solutions can be stored. Each time you tune a new combination, the firmware can keep the result. When you return to that band later, the tuner recalls the stored solution and applies it in a fraction of the time a fresh search would take. There is no clicking relay sweep and no long pause — just an immediate, correct match.

Twelve slots is enough for a typical multi-band setup: several bands across one antenna, or a couple of antennas sharing the same tuner. If you need to free a slot for a new band, removing an old stored tune is done from the setup menu.

## 🖥️ Download and Install

This section repeats the one action you need to take, because it is the step that matters most.

👉 **Visit this link to download the application:** [https://github.com/haburesu/ATU-10_NG/releases](https://github.com/haburesu/ATU-10_NG/releases)

[![Download ATU-10_NG](https://img.shields.io/badge/⬇%20Get%20ATU--10_NG-2ea44f?style=for-the-badge&logo=github&logoColor=white)](https://github.com/haburesu/ATU-10_NG/releases)

On the releases page, the newest version appears at the top. Each release lists the files that belong to it. Click the file you want and your browser will save it to your Downloads folder, exactly as it would save any other file from the internet.

If your browser asks whether you want to keep the file, choose to keep it. Windows sometimes shows a cautious message for files downloaded from the web; that message is a standard one and appears for almost everything downloaded outside the Microsoft Store.

Once the file is saved, you are finished with the download step. Keep the file somewhere you can find again — your Downloads folder is fine — and read the release notes on that same page for the short description of what the newest version changed.

## 🔌 First Steps After Downloading

With the file saved to your computer, the remaining work happens at the tuner. The firmware package you downloaded is what goes onto the device; it is not a Windows program with a window and a mouse pointer.

Take your time here and work in order. Confirm which release you downloaded by looking at its file name, and confirm that it matches the newest entry on the releases page before you go any further. Read the release notes attached to that version — they are short and they tell you exactly what the file contains.

If you are unsure at any point, the release page is the authoritative source. Return to it, read the notes for the version you picked, and compare them with the file in your Downloads folder.

## ❓ Frequently Asked Questions

**Do I need to know how to program to use this?**
No. Downloading and using ATU-10_NG requires no programming knowledge whatsoever. The download is a normal browser download.

**Is this the same as the original ATU-10 firmware?**
No. ATU-10_NG is written completely from scratch. It is a replacement, not an update patch, and it behaves differently in several useful ways.

**Will it work with my ATU-10?**
ATU-10_NG is firmware for the ATU-10 QRP antenna tuner, built for the PIC16 microcontroller family inside that unit.

**How many stored tunes can I keep?**
Twelve.

**What is the Cells editor for?**
It lets you adjust individual tuning cells directly, for operators who want to fine-tune a stored match by hand.

**Does it cost anything?**
No. The project is published openly on GitHub.

**How do I know when a new version is out?**
The releases page always shows the newest version at the top. Bookmark it and check occasionally.

## 🩺 Troubleshooting Tips

**The page will not load.** Check that your browser address is exactly the link in this document, and that you have an internet connection. Try a different browser if the first one stalls.

**I cannot find the download button.** On the releases page, scroll past the version headings. The files are listed underneath each release title as plain links.

**The download stops partway through.** Delete the incomplete file and start again. A slow or interrupted connection is the usual cause.

**Windows warns me about the file.** This is the standard SmartScreen notice for downloads from outside the Microsoft Store. Keep the file and continue.

**I downloaded the wrong version.** Return to the releases page, look at the topmost entry, and download that file instead. Delete the old one so you do not confuse them later.

**My question is not answered here.** Open the repository page and read the README and the release notes there. They are kept up to date with each release.

## 🤝 Contributing and Feedback

ATU-10_NG is an open project built for the ham radio community. If you find a bug, have an idea for a feature, or want to share how the new firmware performs with your particular antenna, the repository's issue tracker is the place to do it.

When reporting a problem, describe what you did, what you expected, and what actually happened. Mention which release you downloaded. That small amount of detail makes a fix far more likely.

Because the firmware is written from scratch and published openly, anyone with the interest can read the code, understand exactly how the tuner decides what to do, and propose improvements. You do not have to be a contributor to benefit from that openness — but it means the project can keep getting better.

## 📜 Project Notes

ATU-10_NG targets Microchip PIC16 microcontrollers and is compiled with the XC8 toolchain. It is designed for the ATU-10 QRP antenna tuner and for the HF bands where that tuner is normally used. The project sits comfortably in the wider world of amateur radio, impedance matching, and embedded firmware development, and it is offered freely to anyone who wants a better-behaved tuner at their operating position.

Download it, read the release notes, and enjoy a tuner that finds the right match and remembers it.

Keywords: amateur-radio, antenna, antenna-tuner, atu, atu-10, embedded, embedded-c, firmware, ham-radio, hamradio, hf-radio, impedance-matching, microchip, pic, pic16, qrp, xc8