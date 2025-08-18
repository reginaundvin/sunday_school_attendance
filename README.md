# sunday_school_attendance
A simple Sunday School Attendance web app with offline storage and one-click backup to Google Sheets.

Features:
- Add students and record attendance by date
- Works fully offline (saves data in your browser)
- Export reports to JSON / CSV / Print
- 🔄 Backup reports directly to Google Sheets (with Google login)

## 🚀 How to Use
1. Open the app in your browser (hosted via GitHub Pages).
2. Add students and mark attendance.
3. Go to **Reports** to view/export.
4. Click **Backup to Google Sheets** to sync data online.

## 🔑 Setup for Google Sheets
1. Enable **Google Sheets API** + **Google Drive API** in [Google Cloud Console](https://console.cloud.google.com/).
2. Create an **OAuth Client ID** (Web) and **API Key**.
3. Replace these in `sunday_school_attendance_with_sheets.html`:

```js
const API_KEY = "YOUR_API_KEY_HERE";
const CLIENT_ID = "YOUR_CLIENT_ID_HERE.apps.googleusercontent.com";
