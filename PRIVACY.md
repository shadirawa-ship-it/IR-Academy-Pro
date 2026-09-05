# IR Academy Pro — Privacy Policy

**Last reviewed:** September 2026

## Summary

IR Academy Pro is a single, self-contained static HTML file. It has no backend server, no analytics or tracking SDK, and no native mobile app. **It does not collect, transmit, or store any data about you anywhere outside your own browser.**

An earlier version of this document described a data-collection pipeline (usage analytics, device/OS reporting, crash reporting via a third-party analytics service, an Android app with at-rest encryption, and related retention schedules). **That description did not match the actual application and has been removed.** No such pipeline exists, has ever existed, or is planned. We are correcting the record rather than leaving an inaccurate policy in place.

## What actually happens

- Opening `index.html` loads a page with a strict Content-Security-Policy (`default-src 'self'`, `connect-src 'self'`) that blocks the page from making any outbound network request.
- The only things saved anywhere are your **theme preference** (light/dark) and your **current tab**, stored via your browser's own `localStorage`/`sessionStorage`. This data:
  - never leaves your device,
  - is never sent to us or to any third party,
  - can be cleared at any time by clearing your browser's site data for this page.
- No cookies are set. No analytics or crash-reporting service is embedded. No third-party scripts are loaded.

## Third parties

None. There are no third-party services (analytics, ads, fonts loaded from a remote CDN, embeds, etc.) in this application.

## Your rights

Because no personal data is collected or processed by this application, there is no user data for us to provide access to, correct, delete, or port on your behalf — there simply isn't any. If you believe this is inaccurate for a specific deployment of this file (for example, a fork that adds analytics), that deployment's operator is responsible for its own privacy disclosures, not this document.

## Regulatory frameworks

Because this application does not collect personal data, GDPR/CCPA data-subject-request obligations and HIPAA's PHI-handling requirements generally do not attach to its own operation. This is a factual statement about this specific file's data flows, not a legal compliance certification — if you need a formal compliance determination for your organization's use of this software, obtain one from qualified privacy/legal counsel.

## Changes to this policy

If a future version of this application ever adds any data collection, this document will be updated first, and the change will be described plainly (what is collected, why, and how to opt out) before it ships.

## Contact

Questions or concerns: **shadirawa@gmail.com**
