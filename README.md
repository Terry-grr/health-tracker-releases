# Health Tracker: Android app releases

Health Tracker is a private, offline-first app for recording symptoms, food, drink, sleep, exercise and daily check-ins. It helps you build a clear, organised record you can take to a GP appointment, and it gives you simple tools to notice patterns and keep up healthy habits.

This repository only hosts the installable Android app. Go to the **[latest release](../../releases/latest)** to download it.

> **Not a medical device.** Health Tracker does not diagnose, treat or give medical advice. It records what you tell it and summarises it. Please talk to a doctor or other health professional about anything that concerns you. In an emergency, call your local emergency number.

---

## Why it exists

- **Appointments are short and memory is unreliable.** It is hard to remember when a headache started, how bad it was, what you had eaten, or how you had been sleeping. A running record turns "I think it's been a few weeks" into dates, severity and patterns.
- **A better conversation with your GP.** The app can produce a summary report, and a PDF, of what you recorded, so you can spend the appointment on the problem instead of trying to recall the details.
- **Everyday support for healthy habits.** Hydration targets and reminders, step counts, sleep tracking and a daily check-in make it easier to see how you are doing from day to day.

The app helps you *notice* patterns, such as symptoms that follow certain foods, poor sleep or low fluid intake. Those links are only suggestions from your own records. They are not proof of a cause, and a health professional should interpret them.

---

## What you can record

| Area | Examples |
|---|---|
| **Headache** | Severity, pain type, location on the head, associated symptoms, medication taken and whether it helped |
| **Digestion and bowel** | Upper and lower abdominal symptoms, bloating, reflux, bowel movements (Bristol scale) |
| **Custom symptoms** | Anything else you want to track, such as joint pain, fatigue or skin flares, with your own severity and location |
| **Food and drink** | Meals, ingredients, portion size, drinks, and a daily water target |
| **Exercise** | Activity and duration |
| **Sleep** | Bedtime, wake time, sleep quality, how you felt on waking, and naps |
| **Night check-in** | End-of-day rating, mood and steps |

Along the way you also get a history view, trend graphs, symptom heatmaps and a calendar view of how your days went.

---

## Reports and sharing

- **GP report:** a summary of how often things happened, average severity, medication use and possible triggers, for a chosen period.
- **PDF export:** overall, or focused on headache, digestive or sleep.
- **Export for AI (optional):** builds a text summary you can paste into an AI tool of your choice. You decide what to include, and dates can be replaced with relative days ("Day 1", "Day 3"). The app tries to remove email addresses, phone numbers and street addresses from your notes, but please **read the text before you share it**. Once you paste it into another service, that service's own privacy terms apply, and AI replies are not medical advice.

Your data only leaves the app when **you** choose to export or share it.

---

## Health Connect (optional)

If you allow it, Health Tracker can **read** your steps and sleep from Android Health Connect, for example from a watch or sleep app.

- **Read-only.** The app never writes to Health Connect and never reads other kinds of data.
- **Sleep form:** it can fill in last night's bedtime and wake time, plus a **suggested** quality of Restful, Restless or Broken. The suggestion comes from simple, measurable rules (time asleep, time awake in the night, how often your sleep stage changed). It is a rough estimate that you can change. It says nothing about how rested you actually felt.
- **How you felt is yours to log.** The app leaves that box for you to fill in.
- **If you don't log a night yourself,** the app saves the imported night automatically at midday, with how you felt left blank. A second sleep in the same day is treated as a nap only if you confirm it.
- **Turn it off any time** in Android Settings, under Privacy, Health Connect, App permissions, Health Tracker.

---

## Privacy

- **Your data stays on your phone.** Everything is stored locally on your device. There are no accounts, no logins, no analytics, no advertising and no trackers.
- **No health data is sent to the developer or to third parties.**
- **Optional private sync:** people who run their own home server can sync to it over their own network. This is not needed to use the app.
- **Update checks:** the app can look in this repository for newer versions. That is an ordinary web request to GitHub. It sends no health information, though GitHub can see the request, as with any website.
- **Backups:** in the standalone app you can turn on automatic backups to a folder you choose, and restore them later. You hold your own data.

The full privacy policy is inside the app, in Settings. It is also summarised in plain terms above.

---

## Install

1. On your Android phone, open the **[latest release](../../releases/latest)** and download `health-tracker.apk`.
2. Open the downloaded file. If Android asks, allow your browser or file manager to **install unknown apps**.
3. Open Health Tracker. Everything works offline from here.

Because the app is not on the Play Store, Android will warn you about installing from outside it. Only download the APK from this releases page.

## Updating

- The app checks this repository for new builds and shows an **update banner** when one is available. Tap it to download the new file, then open it to install over the top. Your data stays in place.
- You can choose where the app looks for updates in the **Android APK** screen in Settings.
- **Make a backup before updating**, in Settings under Data and Backup.

## Backups

Because the standalone app has no central server, turn on **Auto Backup** in Settings under Data and Backup. Pick how often it runs and where the file is saved, for example your Downloads folder or a cloud-synced folder. To restore, choose **Restore Backup** in the same place and select a `.zip` backup or a `health_data.json` file.

---

## Licence and terms of use

- Health Tracker is free to install and use for personal use.
- It is **not open source**. Please don't redistribute, modify or resell the app without permission.
- It is provided **"as is"**, without warranty of any kind. Use it at your own risk. The author is not responsible for lost data or for decisions made using what the app shows, so keep backups.

## Open-source software and licences

Health Tracker is built with the help of open-source software. Each component remains the property of its authors and is used under **its own licence**. Nothing in this README changes those licences.

The main components are:

- **App interface and data:** React, Dexie (local database), Recharts (graphs), Lucide (icons) and Motion (animations)
- **Reports and sharing:** jsPDF and jsPDF AutoTable (PDF export), JSZip (backups), html-to-image and QRCode
- **Styling and build tools:** Tailwind CSS and Vite
- **Android layer:** Capacitor (core, app, filesystem, share, local notifications and health-fitness plugins), plus Android platform libraries such as AndroidX, Kotlin and the Health Connect client

Many of these are published under permissive licences such as MIT or Apache 2.0, but the exact terms differ from project to project. The copyright notice and licence text for each one is available on that project's own repository or package page.

## Trademarks

Android and Health Connect are trademarks of Google LLC. All other product and company names are the property of their respective owners. Health Tracker is an independent project and is not affiliated with, or endorsed by, any of them.

---

## Please remember

- This is a personal record-keeping tool, not clinical software. It can be wrong, and it only knows what you or your watch tells it.
- Don't delay seeking care because of anything the app shows or doesn't show.
- If you leave feedback in this repository's **Issues** tab, please don't include personal health information, because it is public.

*Last updated: November 2026*
