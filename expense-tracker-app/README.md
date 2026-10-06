# Daily Expense Tracker

A simple calendar-based web app for tracking daily expenses and earnings. It runs in any browser and can be installed on a phone or computer as an app. No account or server is needed.

**Live app:** https://YOUR-USERNAME.github.io/expense-tracker/

## Features

- **Calendar view.** Click any day to see and add its entries. Each day shows what you earned and spent.
- **Expenses.** Record the item, type, amount each, and how many. The total is amount × quantity.
- **Expense types.** Food, Transport, School, Bills, Shopping, Health, Entertainment and Other.
- **Earnings.** Record money received from Salary, Allowance or Other.
- **Daily totals.** Spending and earnings are added up for the selected day.
- **Monthly totals.** Earnings, expenses and balance are added up for the month. They update when you change months.
- **Delete entries.** Remove any entry with one click.
- **Installable and offline.** Works as a Progressive Web App (PWA) once installed.
- **Light and dark mode.** Follows your device setting.
- **Mobile friendly.** The layout adjusts to small screens.

## How to use

1. Open the app and pick a day on the calendar.
2. Choose **Add expense** or **Add earning**.
3. Fill in the item, type and amount. For expenses, also enter how many.
4. Click the add button. The day and month totals update right away.
5. Use the `<` and `>` buttons to switch months.

## Install as an app

- **Android (Chrome) or desktop (Chrome/Edge):** open the live link and tap **Install app**.
- **iPhone (Safari):** open the live link, tap **Share**, then **Add to Home Screen**.

## Your data

Entries are saved in your browser's local storage on the device you use. They are not uploaded anywhere. This means:

- Your data stays private.
- Data is not shared between devices or browsers.
- Clearing your browser data will delete your entries.

## Project files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (HTML, CSS and JavaScript) |
| `manifest.webmanifest` | App name, icons and colors for installing |
| `sw.js` | Service worker that enables offline use |
| `icon-192.png`, `icon-512.png` | App icons |

## Run locally

Service workers need a web server, so opening the file directly will not enable install or offline mode. From the project folder, run:

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy on GitHub Pages

1. Push the files to a public GitHub repository.
2. Go to **Settings → Pages**.
3. Set the source to **Deploy from a branch**, choose **main** and **/ (root)**, then save.
4. Your app will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

After changing files, update the cache name in `sw.js` (for example `expenses-v1` to `expenses-v2`) so installed copies pick up the new version.

## Built with

Plain HTML, CSS and JavaScript. No frameworks or dependencies.

## License

MIT. Free to use and modify.
