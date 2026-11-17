# WorkBridge – Prototype

Platform that connects skilled workers (electrician, plumber, welder, fitter, carpenter...) with nearby customers.
Hackathon prototype: plain HTML + CSS + JavaScript, no build step, sample data only.

## Run locally (VS Code)
1. Open this folder in VS Code.
2. Install the **Live Server** extension, right-click `index.html`, choose **Open with Live Server**.
   (You can also just double-click `index.html`.)

## Logins
| Role | Access | Demo username | Demo password |
|------|--------|---------------|---------------|
| Customer | Open, no login | – | – |
| Worker | Login required | `ramesh` | `worker@123` |
| Admin | Login required | `admin` | `admin@123` |

**New workers:** open the Worker tab and click **New worker? Create your profile**. Fill the form (name, work domain, location, experience, mobile, username, password). The profile is created and the worker is logged in. The worker can then upload a certificate and work photos, and the admin can approve the certificate.

> These credentials are demo-only and sit in `app.js` (the `CRED` object). A real product must check logins on a server with hashed passwords.

## Features
- Customer: search, location and work-domain filters, sort, favourites, worker profile with portfolio, certificates, reviews, service request.
- Worker: sign up with a new profile, availability toggle, profile edit, add work photo, upload certificate, view requests.
- Admin: certificate approve/reject, complaints, platform stats.
- Languages: English, Hindi, Marathi.
- Future: AI worker recommendations, voice search, real messaging and database.

## Publish on GitHub and get a live link
```bash
git init
git add .
git commit -m "WorkBridge prototype"
git branch -M main
git remote add origin https://github.com/<your-username>/workbridge.git
git push -u origin main
```
Then on GitHub: **Settings > Pages > Build and deployment > Deploy from a branch > main / (root) > Save**.
Your live link will be `https://<your-username>.github.io/workbridge/`.
