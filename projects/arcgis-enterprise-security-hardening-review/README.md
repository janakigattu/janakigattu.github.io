# ArcGIS Enterprise Security Hardening Review

Your Portal is on the internet whether you meant it to be or not. Answer fourteen questions drawn from Esri's own security best practices, and this review names the gaps ranked by severity, the three fixes that matter most, and the score your deployment earns.

## What it does

Answer fourteen checks, each Yes, No, or Not sure, across three severity groups: Critical (HTTPS only, CA-signed certificate, proxy restricted to approved hostnames, token requests with credentials in the URL disabled), Important (anonymous access, services directory, enterprise logins, patches current, WebGISDR backups tested), and Recommended (self sign-up, LDAPS, password policy, named service accounts, Monitor or audit log review). Press Review my deployment.

You get a hardening score out of 100, a verdict (Locked down at 85 and above, Fix the critical gaps first at 60 to 84, Hardening overdue below 60), the three fixes that matter most in the order to work in, every open gap with the fix for it, the checks you answered Not sure that still need a real answer, and a ten-item printable checklist. One open Critical check drops the verdict a full band, whatever the score says.

## The facts it stands on

- The checks are Esri's own: the security best practices documentation for ArcGIS Enterprise, and the portalScan.py script Esri ships with Portal, which reports the same ground as Critical, Important, and Recommended findings (PS01 proxy restrictions, PS02 token requests with credentials in the URL, PS03 services directory, PS04 HTTPS only, PS05 built-in account sign-up, PS06 anonymous access, PS07 LDAP identity store encryption, PS08 self-signed SSL certificate).
- Severity weights (Critical 10, Important 8, Recommended 4), the verdict bands, the one-band downgrade for an open Critical check, and the fix wording are planning rules from practice, not vendor numbers, and the page says so. Run portalScan.py after this review and treat its output as the authority over this page.

## Run it

Open `index.html` in any browser. No backend, no API key, no account. Nothing you type is sent or stored anywhere. Print gives a clean summary.

## Try it with Janaki

Email Janaki with your score and your three biggest gaps: [gjanaki360@gmail.com](mailto:gjanaki360@gmail.com?subject=ArcGIS%20Enterprise%20Security%20Hardening%20Review). Or book a session at [janakigattu.github.io](https://janakigattu.github.io/).
