# Easy Life Test Website

A small, real, single-page demo site that conforms to the
[Easy Life Content Installer](https://github.com/Trigve-Hagen/easy-life-content-installer)
standard — built to prove the standard and its tool work against a real
repo, not just synthetic test data.

Every piece of real, replaceable content on this page is marked with a
`<!-- @content-slot ... -->` comment, per that standard:

| key | type | constraint |
|---|---|---|
| `hero_headline` | title | max 60 characters |
| `hero_tagline` | body | max 150 characters |
| `hero_image` | image | 1200×600 |
| `about_paragraph` | body | max 600 characters |
| `feature_video` | video | max 60 seconds |

Try it yourself:

```
git clone https://github.com/Trigve-Hagen/easy-life-content-installer
git clone https://github.com/Trigve-Hagen/easy-life-test-website
python3 easy-life-content-installer/content_installer.py scan easy-life-test-website
```

See [easy-life-test-site-customizations](https://github.com/Trigve-Hagen/easy-life-test-site-customizations)
for a real, filled-in manifest that installs into this exact site.

## License

MIT — see `LICENSE`.
