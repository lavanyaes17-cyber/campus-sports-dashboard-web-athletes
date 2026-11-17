# Campus Sports Tournament Dashboard (Phase 1)

Pages: index, schedule, register, sports, live-scores, results, admin (HTML5 + CSS3 + JavaScript, no framework).

## Run locally
Open `index.html` in a browser (or run `python -m http.server` in this folder and visit http://localhost:8000).

## How Admin connects to the other pages
All pages share `js/storage.js`, which keeps data in the browser's localStorage.
- Admin > Publish Announcement         -> Home > Announcements
- Admin > Update Live Score / events   -> Home > Live Now and Live Match Center (auto-refreshes)
- Admin > Finish match / Record result -> Schedule (standings, completed fixtures), Home > Latest Results, Results page
- Admin > Add Fixture                  -> Schedule > Fixtures
- Admin > Awards & Final Results       -> Results page and Home champion line
- Register page                        -> Admin > Registration Review (Approve / Reject) -> status shows on Register page

Limit: localStorage is per browser and device. Posts made on your laptop are visible on your laptop only.
Sharing updates with every visitor needs a backend/database (planned for a later phase).
Use "Reset demo data" at the bottom of the Admin page to clear everything.

## Deploy to GitHub Pages
Replace the files in your repo folder (Campus_Sports_Tournament_Dashboard_4) with these, commit and push,
then hard-refresh the site (Ctrl+Shift+R).
