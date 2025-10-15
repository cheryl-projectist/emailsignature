
# Email Signature Template (Bulletproof HTML)

A minimal, table-based HTML email signature that renders cleanly across Gmail, Apple Mail, Outlook (Windows/Mac/Web), and more.

## Quick start

1. Open `signature.html` in a browser, select all, and copy.
2. Paste into your email client's signature editor (see tips below).

> Images are using placeholder URLs for demo purposes. Replace with your own hosted HTTPS image URLs.

## Edit the signature

- Replace text fields like **Your Name**, **Title**, **Phone**, etc.
- Swap the placeholder `via.placeholder.com` icons and logo with your assets, ideally at 2× resolution (retina) but displayed at normal size via `width`/`height`.
- Keep everything **table-based with inline styles** for maximum Outlook compatibility.

## Install in common clients

### Gmail (Web)
- Settings → *See all settings* → **General** → **Signature** → New.
- Paste from the browser-rendered `signature.html` for best fidelity.

### Apple Mail (macOS)
1. Mail → Settings → **Signatures** → select account → “+”.
2. Type a placeholder word and close Settings to force-create the file.
3. Quit Mail. Open `~/Library/Mail/V*/*/MailData/Signatures/` (version folder may vary).
4. Edit the newest `.mailsignature` and replace its body with the HTML from this repo.
5. Reopen Mail and uncheck **Always match my default message font**.

### Outlook
- **Windows desktop:** File → Options → **Mail** → **Signatures…**. If direct paste is imperfect, open `signature.html` in your browser, copy all, then paste.
- **Mac:** Outlook → Settings → **Signatures** → New → paste from browser.
- **Web (OWA):** Settings (gear) → Mail → **Compose and reply** → paste.

## Why this works
- Tables + inline styles ensure consistent rendering in Word-based Outlook.
- Safe fonts (Arial/Helvetica) avoid substitution issues.
- Fixed image dimensions avoid layout shift when images are blocked.
- Minimal CSS—no media queries required for desktop clients.

## Repo structure

```
email-signature-template/
├── signature.html      # Ready-to-copy signature
├── README.md           # Instructions & rationale
└── LICENSE             # MIT
```

## License
MIT © You
