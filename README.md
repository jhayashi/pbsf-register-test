# pbsf-register-test

DEVELOPMENT versions of the PBSF registration form, served by GitHub Pages at
**https://register-test.piedmontbaseball.org/**. Families use https://register.piedmontbaseball.org/.

`index.html` is **generated**: it is `frontend/registration.html` from a branch of the private
`jhayashi/pbsf-reg` repo (normally `dev`), pushed here by that repo's "Publish form (test site)"
workflow with `BACKEND_URL` pointing at the **DEV** Apps Script backend.

- Always Stripe **test mode**: the form refuses live mode on this host, and the DEV backend only
  has Stripe's test key. Card 4242 4242 4242 4242, any future date, any CVC.
- Registrations go to the DEV spreadsheet, never the live one. Evaluation invitations go only to
  the `[TEST]` calendar event.
