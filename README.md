# bindchat-support

Support page and privacy policy for **bindchat**, an offline AI chat app for iPhone (Ofuchi Daichi).
Static HTML/CSS for GitHub Pages; no build step, no JavaScript, no analytics.

| Page | URL |
| --- | --- |
| Support (Japanese) | https://daichiofuchi.github.io/bindchat-support/ |
| Privacy policy (Japanese) | https://daichiofuchi.github.io/bindchat-support/privacy.html |
| Support (English) | https://daichiofuchi.github.io/bindchat-support/en/ |
| Privacy policy (English) | https://daichiofuchi.github.io/bindchat-support/en/privacy.html |

The app opens the English pages when its UI is in English (`Support/AppLinks.swift` in the app project).

## Files

- `index.html`, `privacy.html` — Japanese pages
- `en/index.html`, `en/privacy.html` — English pages
- `style.css` — shared styles (white / black / sky blue `#0EA5E9`)
- `assets/` — icons generated from the app icon (`AppIcon-1024.png`)
- `.nojekyll` — serve files as-is (no Jekyll processing)

## Publish

```sh
gh repo create daichiofuchi/bindchat-support --public --source=. --push
gh api -X POST repos/daichiofuchi/bindchat-support/pages -f "source[branch]=main" -f "source[path]=/"
```

Pages may take a minute or two to go live after the first push.

## Updating the privacy policy

Edit both `privacy.html` and `en/privacy.html`, and update the effective date in both.

Contact: dai1011q@gmail.com
