# Grace Abundance Member Portal

Clickable demo of the cooperative's member and officer app. It is a static PWA: no build step.

## Run
Open `index.html`, or serve the folder: `python3 -m http.server 8000`.

## Put it on GitHub Pages
1. Create a repository and upload every file and folder here.
2. Settings, Pages, Deploy from branch `main`, folder `/ (root)`.
3. Open the Pages link. Install prompts and offline support need HTTPS, which Pages provides.

## What is demo-only
Sign-in, balances, votes and approvals are stored in the browser (`localStorage`) and shared with nobody. A real launch needs a secure backend (see `lovable/schema.sql`).

## Files
`index.html` the app, `manifest.webmanifest` and `sw.js` install and offline, icon and PDF files sit in the same folder as index.html.

## Privacy
The app shows a consent gate, cookie notice and Privacy Notice. Have a Nigerian lawyer review `docs/Privacy_Notice.pdf` and confirm with the NDPC whether the Society must register as a data controller of major importance.

## Roles and access
Roles: Member, Chairman, Vice Chairman, Secretary General, Treasurer, Financial Secretary, Loan Committee, Supervisory Committee. Trustees are the Chairman, Secretary General and Treasurer by office. When an officer changes office, their tenure ends or they leave, the Chairman or Vice Chairman confirms and the account is deactivated or changed (People screen). Every change is logged.

## Excel
Data screen: download the data as Excel, edit, and upload to update Users, Members and News. A ready template is `Grace_Abundance_Data_Template.xlsx`. The Excel library loads from cdnjs, so the first load needs internet.
