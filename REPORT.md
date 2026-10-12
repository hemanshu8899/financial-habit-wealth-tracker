# Financial Habit Builder & Wealth Growth Tracker

**Intern:** Hemanshu Pachange
**Role:** Fullstack Web Development Intern
**Live app:** https://hemanshu8899.github.io/financial-habit-wealth-tracker/
**Source code:** https://github.com/hemanshu8899/financial-habit-wealth-tracker

## 1. Problem statement
Many people want to save money but fail because saving is not a daily habit and they cannot see how small amounts grow over time. This project turns saving into a daily habit and shows the long-term effect of those habits.

## 2. Objectives
- Let users create daily money-saving habits with a rupee value.
- Track daily completion, streaks and total savings.
- Let users set a savings goal and log manual deposits.
- Project future wealth using monthly saving, expected return and time.

## 3. Features
1. **Daily money habits:** add a habit (for example "Skip takeaway", ₹150/day), tick it each day, see a 7-day history and a streak counter, and delete habits.
2. **Total saved:** automatically adds the value of every completed habit day and every deposit.
3. **Savings goal and deposits:** set a goal in ₹, see a progress bar, and log or remove deposits with notes.
4. **Wealth growth projection:** sliders for monthly saving, yearly return (0–20%) and years (1–30), with a chart comparing growth against savings without returns.
5. **Responsive and accessible design:** works on phones and desktops, supports light and dark mode, and has labelled inputs and keyboard focus.

## 4. Tech stack
| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, flexbox, grid, media queries) |
| Logic | Vanilla JavaScript (ES6) |
| Data storage | Browser localStorage |
| Charts | Inline SVG |
| Version control | Git and GitHub |
| Hosting | GitHub Pages |

## 5. How it works
- App state (habits, deposits, goal, monthly saving) is kept in one JavaScript object and saved to localStorage after every change.
- Total saved = (completed habit days × habit amount) + all deposits.
- Streak = consecutive days ending today (or yesterday) with the habit completed.
- Projection uses monthly compounding: `value = value × (1 + rate/12) + monthly saving`, repeated for each month.
- The default monthly saving is estimated from the last 30 days of activity.

## 6. How to run
1. Open the live link above, or
2. Download the repository and open `index.html` in any browser. No installation is needed.

## 7. Challenges and solutions
- **File naming on Windows:** the file was saved as `index.html.html` because extensions were hidden. Fixed by showing file extensions and renaming.
- **Repository name conflict:** the first name was already taken, so a new repository name was used.
- **Deployment:** enabled GitHub Pages on the `main` branch to get a live link.

## 8. Limitations and future scope
- Data is stored only in the user's own browser, so it does not sync between devices.
- Planned upgrades: a Node.js and Express backend, a database (MongoDB or PostgreSQL), user login, cloud sync, monthly reports and spending categories.

## 9. Learnings
- Building a full interface with HTML, CSS and JavaScript only.
- Managing state and persisting data in the browser.
- Using Git and GitHub Desktop, and deploying with GitHub Pages.
- Designing for mobile screens and accessibility.
