# Security Policy

## Scope

IR Academy Pro is a single, self-contained static HTML file (`index.html`) with no backend server, no database, no user accounts, and no network calls beyond loading the page itself (enforced by a strict Content-Security-Policy: `default-src 'self'; connect-src 'self'`). This significantly limits the attack surface compared to a typical web application, but the following are still in scope for security reports:

- Cross-site scripting (XSS) or HTML/script injection via any input field (e.g. the search box)
- Any way the page's Content-Security-Policy can be bypassed
- Any way client-side data (theme preference, active tab, stored only in `localStorage`/`sessionStorage`) could be exfiltrated
- Supply-chain concerns, if this project ever adds external dependencies (it currently has none)

## Supported versions

This is a single-file application with a linear version history in [CHANGELOG.md](./CHANGELOG.md). Only the current version published at the live site (https://shadirawa-ship-it.github.io/IR-Academy-Pro/) and in the `main` branch of this repository is supported. There are no older maintained release branches.

## Reporting a vulnerability

Please report suspected security issues privately, not as a public GitHub issue, by emailing:

**shadirawa@gmail.com**

Include:
1. A description of the issue and its potential impact
2. Steps to reproduce (a minimal example is ideal)
3. The URL or file version where you observed it

There is currently no guaranteed response SLA (this is a small, independently maintained project), but security reports are treated as the highest priority and will be acknowledged as soon as possible.

## Reporting a clinical-content or accuracy issue

This is not a traditional "security" issue, but for an educational medical reference, an inaccurate procedure step, device specification, or (especially) a medication dose is a safety-relevant defect. Please report these the same way — email **shadirawa@gmail.com** with the specific page/procedure, the issue, and ideally a citation to a current guideline or primary source — rather than filing them as generic bugs.

## Disclosure

Given the small scope and audience of this project, coordinated disclosure timelines will be worked out directly with the reporter on a case-by-case basis rather than a fixed policy.
