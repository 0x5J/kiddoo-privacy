kiddoo-privacy
==============

Static GitHub Pages site for Kiddoo (iOS baby tracker): privacy policy,
legal notice (Impressum), and in-app support/FAQ.

Live site: https://0x5j.github.io/kiddoo-privacy

This repository does not contain the Kiddoo iOS app. It only hosts the
public HTML pages linked from the app / App Store listings.


Files
-----

README.md     Short repo title only ("kiddoo-privacy").
index.html    Datenschutz & Impressum (privacy policy and legal notice).
support.html  Support & Hilfe (contact and FAQ).
readme.txt    This file.


Pages
-----

1) index.html — Datenschutz & Impressum
   Title: "Datenschutz & Impressum – Kiddoo"
   Language: German (lang="de")
   Nav: Datenschutz (this page) | Support (support.html)
   Production nav uses absolute GitHub Pages URLs:
     https://0x5j.github.io/kiddoo-privacy
     https://0x5j.github.io/kiddoo-privacy/support.html

   Content sections:
   - Overview: entries stored locally on device; no operator-owned
     servers; no sharing of data with third parties.
   - Data processed: meals (breast / bottle / solids), sleep, diapers,
     growth (weight, length, head circumference), checkups; child
     profile (name, birth date, sex, optional photo); optional notes,
     timestamps, app settings. No registration / account with the
     operator.
   - Storage & iCloud: local-first; optional sync via the user's
     private iCloud / Apple CloudKit when signed into iCloud. Apple
     acts as processor; the operator has no access. Partner sharing
     only after an explicit invitation. Without sync, data never
     leaves the device.
   - No ads, no analytics/tracking (explicitly no Google Analytics,
     Firebase, Mixpanel), no third-party data sharing. The only
     transfer, if enabled, is to Apple iCloud for the sync features
     above.
   - Legal basis: Art. 6(1)(b) GDPR for core app functions;
     Art. 6(1)(a) GDPR consent for optional iCloud sync and partner
     sharing.
   - Retention / deletion: user can delete via "Alle Einträge löschen"
     in settings or by uninstalling the app; iCloud copies via the
     user's Apple account.
   - GDPR rights: Arts. 15, 16, 17, 18, 20, 21; complaint to a
     supervisory authority (Art. 77). Operator cannot inspect entry
     contents; access/erasure in practice is user-managed locally
     and in iCloud.
   - Children: app is for parents/guardians; does not collect data
     from children themselves; minors should use it only under
     guardian supervision.
   - Impressum / controller (DSGVO / § 5 DDG):
       Name:    Sören Jacobsen
       Address: Ringstr. 18a, 19067 Cambs
       Email:   support@kiddoo-app.de
       App:     Kiddoo – Baby-Tracker (iOS)
   - Policy may be updated when the app changes; current version is
     the page at this URL.
   - Footer date: 31 May 2026.

2) support.html — Support & Hilfe
   Title: "Support & Hilfe – Kiddoo"
   Language: German (lang="de")
   Nav: Datenschutz (index.html, relative) | Support (this page)

   Content:
   - Contact: mailto:support@kiddoo-app.de
     Users are asked to include iPhone model and iOS version.
   - FAQ:
     * How to log an entry (Heute tab: Trinken, Wickeln, Schlaf;
       sleep uses a timer).
     * Data sync: automatic via private iCloud when signed in; no
       third-party sharing.
     * Partner sharing: Mehr → Partner & Sync → Partner einladen;
       both parties need an iCloud account.
     * Pediatrician report: Mehr → Reports → pick a period → PDF.
     * Delete data: Mehr → Einstellungen → Alle Einträge löschen,
       or uninstall; details on the privacy page.
   - Footer date: 31 May 2026.


Local preview
-------------

These are self-contained static HTML files (inline CSS/JS; Google Fonts
loaded from fonts.googleapis.com / fonts.gstatic.com). No build step
and no backend.

Open in a browser:
  open index.html
  open support.html

Or serve the repo root over HTTP (avoids any file:// quirks):
  python3 -m http.server 8000
Then visit:
  http://localhost:8000/index.html
  http://localhost:8000/support.html

Note: index.html nav points at the live GitHub Pages URLs, so from a
local server those links go to production. support.html nav uses
relative paths (index.html / support.html).


Contact
-------

Support email used on both pages: support@kiddoo-app.de
Legal/privacy controller: Sören Jacobsen (see Impressum on index.html).
