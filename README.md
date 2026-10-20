# BASTA! — the public pages

The three pages the outside world needs from BASTA!:

| file | what it is | why it exists |
|---|---|---|
| `index.html` | the landing page | what the app is |
| `privacy.html` | the privacy policy | **required** by App Store Connect |
| `support.html` | support and contact | **required** by App Store Connect |

**The source of truth for these files is the app repository**, in
`site/` — they are versioned with the app they describe. This repository is
published, and it is generated from that folder.

To publish a change:

```bash
content/tools/publish_site.sh
```

**Nothing here may load anything from another company.** No web fonts, no
scripts, no CDN, no analytics, no cookies. The privacy policy of a privacy
app is not the place to introduce a tracker.
