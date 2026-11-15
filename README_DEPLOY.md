# MEDSHUBH PWA — deployment notes

## Contents
- `index.html`: single-page MCQ practice prototype (NEET PG/FMGE demo bank and separate original INI-CET-pattern practice bank).
- `manifest.json`, `sw.js`, `icon.svg`, `icons/`: install metadata, offline app shell, and app icons.
- `vercel.json`: static deployment headers/configuration.

## Deploy with Vercel (no build step)
1. Extract this ZIP on a computer or upload the `medshubh_pwa` folder contents to a new GitHub repository.
2. Import that repository at Vercel and choose **Other** / static site if prompted.
3. Set the project root to the folder containing `index.html` (repository root if files are at root).
4. Leave Build Command empty; set Output Directory to `.`; deploy.
5. Open the HTTPS deployment URL and test an exam switch, a timed question, answer feedback, and reload/offline behavior.

## Install
- Android/Samsung: open the HTTPS URL in Chrome, open the browser menu, tap **Install app** (or **Add to Home screen**), and confirm.
- iPhone/iPad: open the HTTPS URL in Safari, tap **Share**, choose **Add to Home Screen**, then **Add**. iOS may not show the in-page install prompt; this is expected.

## Important limitations before public/student launch
- This is a front-end prototype. Progress is stored only in that browser/device using localStorage; there are no accounts, cloud sync, admin tools, database, or secure student records.
- The question sets are original demo/practice questions. They are not verified actual PYQs. Keep actual PYQs separately sourced and verified before labeling them as such.
- Confirm question accuracy, answer keys, explanations, accessibility, and device/browser behavior before publishing to students.
- Do not add personal/medical/student data until authentication, privacy notice, security controls, and data handling are designed.
