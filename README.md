# MagaCircle™ Version 1 — Full Visitor Test Prototype

This is the first complete visitor-flow prototype for the MagaCircle™ launch site.

## Included flow
1. Landing page with **POWER TO THE PEOPLE**
2. Name + email capture
3. 10-question quiz, one question per screen
4. Three quiz sections: WHO ARE YOU? / WHAT DO YOU WANT? / WHAT WOULD YOU BUILD?
5. Section transition screens after Q3 and Q7
6. Back navigation during the quiz
7. Personalized MagaCircle™ Profile (5 prototype profile types)
8. 5-person invitation/referral step
9. Text / email / copy-link / native share options
10. Prototype referral controls so you can test 0/5 → 5/5 without real users
11. Launch waitlist confirmation
12. Launch membership teaser — actual membership levels are intentionally deferred until the next strategy pass

## How to test locally
Open `index.html` in a browser. For the most realistic behavior, serve the folder with a simple local web server (for example, VS Code Live Server or `python -m http.server`).

## GitHub Pages
Upload `index.html`, `styles.css`, `app.js`, and this README to a GitHub repository. Enable GitHub Pages from the repository settings. No build step is required.

## Important prototype notes
- Email collection is currently browser-only. It is **not connected to a CRM/email service**.
- Referral tracking is currently simulated in the browser with LocalStorage. The "Prototype testing controls" let you add one test referral at a time.
- Production referral verification should be server-side and tied to unique referral links/accounts before launch.
- The profile scoring is a first-version scoring model intended for testing the experience. We can refine the scoring after you test how the results feel.
- Membership levels/pricing are intentionally not finalized in this build.
- The visual treatment follows the current direction: stronger flag imagery on landing/profile/final screens and cleaner quiz screens, while keeping the **POWER TO THE PEOPLE** slogan primarily on key brand moments rather than every quiz question.

## Resetting your test
The final screen's **RETURN TO HOME** button clears the prototype LocalStorage state and reloads the site.
