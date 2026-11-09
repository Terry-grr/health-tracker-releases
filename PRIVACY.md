# Privacy Policy – Health Tracker

Last updated: November 2026

Health Tracker is an offline-first, private personal health management application designed to track symptoms, medications, nutrition, hydration, sleep, and steps.

## Data Collected & Accessed

1. **Android Health Connect**:
   - **Steps**: Read strictly to calculate daily step totals and populate your daily check-in.
   - **Sleep**: Read strictly to record bedtime, wake time, and sleep duration in your personal sleep history.
   - Health Tracker does not write data back to Health Connect.

2. **Personal Health Logs**:
   - Symptoms, pain locations, severity, medications, meals, beverages, sleep notes, and check-in scores entered by you.

## How Your Data Is Stored & Transferred

- **Local-First Storage**: All data is stored directly on your device using IndexedDB (and native documents storage for backups).
- **Private Server Synchronization**: If you configure a self-hosted Docker server (e.g. on your local home network / port 3030), data synchronizes directly with your private server.
- **Zero Third-Party Sharing**: No health data, step counts, sleep records, or personal metrics are ever sent to external cloud analytics, advertising networks, or third-party servers.
- **No Account Required**: The app operates standalone without external accounts or trackers.

## Contact & Control

You can disconnect Health Connect permissions at any time via Android Settings → Privacy → Health Connect → Permissions → Health Tracker, or via the integration settings in the app.
