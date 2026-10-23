# Scholarship Eligibility Scout — Hackathon Prototype

## Run locally
1. Extract the ZIP.
2. Open `index.html` in Chrome/Edge/Firefox.
3. Click **Run all 4 test cases**.
4. Click **Export evidence JSON** to save the evidence report.
5. Click **Check schemes** and use **Save draft** to demonstrate draft IDs.

No installation or API key is required for this local prototype.

## Honest limitations
- This is a local browser prototype, not a deployed cloud service.
- Scheme rules are explicitly illustrative and the URLs are placeholders (`example.org`). Replace them with verified official scholarship source URLs and quoted rules before claiming real eligibility.
- TC3 intentionally reports FAIL because this prototype simulates file sizes but does not actually compress/upload a file or verify readability.
- TC4 demonstrates DOB mismatch detection logic but is not connected to a real portal.
- TC1/TC2 PASS statuses mean only that the local illustrative rule logic worked; they do not prove official scheme eligibility.
- Do not use real student personal data. Never bypass OTP/CAPTCHA. Require human approval before irreversible actions.

## Suggested deployment
Deploy `index.html` as a static site using a service you control (for example GitHub Pages or Netlify). Verify the live URL in a private/incognito window before submitting. Do not claim a deployment until it works.

## Suggested stack (implemented vs planned)
Implemented: HTML, CSS, JavaScript, local in-memory state, JSON evidence export, synthetic test simulations.
Planned/integration options: n8n, Gemini API, Python/Playwright, SQLite/Supabase. Do not list a tool as used unless you actually integrate it.

## Evidence IDs
- `INPUT-TC1` ... `INPUT-TC4`: synthetic test inputs
- `EVD-*`: demo rule evidence references
- `DR-*`: local draft identifiers
- `DOC-TC3-*`: simulated document references
