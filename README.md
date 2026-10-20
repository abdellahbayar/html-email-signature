# HTML Email Signature

A compact email signature I made for my personal emails, with a browser preview and a button to copy the formatted signature into Gmail.

**HTML · CSS · Vanilla JavaScript**

![Email signature preview](preview.png)

## What it does

- Shows my name, role, areas of interest and contact details.
- Links directly to my phone number, email, portfolio and LinkedIn profile.
- Copies the signature as rich HTML, alongside a plain-text clipboard version.
- Keeps the signature itself image-free, using a table layout and inline styles.
- Opens locally without a build step, external libraries, fonts or tracking scripts.

## Use it

1. Download this repository using **Code → Download ZIP** and extract it.
2. Open **index.html** in your browser.
3. Click **Copy signature**.
4. In Gmail, go to **Settings → See all settings → General → Signature**.
5. Create a signature and paste into the editor using **Ctrl + V**.
6. Select the default signature for new emails and replies, then save the settings.

If copying is blocked by the browser, select only the signature inside the white preview and copy it manually. Use **Cmd** instead of **Ctrl** on macOS.

Gmail setup reference: [Google's signature instructions](https://support.google.com/mail/answer/8395?hl=en).

## Personalize it

Edit the signature table in **index.html**. The copy button reads that table directly.

| Item | What to change |
| :--- | :--- |
| Name and role | Visible text in the first rows |
| Focus areas | The Systems / Networking / Cybersecurity line |
| Phone | Both the visible number and its `tel:` link |
| Email | Both the visible address and its `mailto:` link |
| Portfolio and LinkedIn | Link destinations and visible labels |
| Accent color | The `#2563eb` values in the signature's inline styles |

If you use the standalone HTML fragment or plain-text version, update **signature.html** and **signature.txt** too.

## Files

| File | Purpose |
| :--- | :--- |
| `index.html` | Local preview, Gmail instructions and copy button |
| `signature.html` | Only the email signature HTML fragment |
| `signature.txt` | Plain-text alternative |
| `preview.png` | Screenshot used in this README |

## Design notes

The preview page uses normal page CSS. Only the signature table is copied into the email editor; its styling is inline and does not depend on the preview page or its JavaScript.

The blue divider and text links keep the layout small enough for everyday emails. The preview image is documentation, not an image embedded in the signature.

## Verification and limits

Checked locally in desktop Chrome: contact links, the copy button and the preview at a 390px viewport. The HTML and plain-text clipboard formats are checked in the local verification.

This is not a full email-client compatibility test. Gmail, Outlook and other clients may adjust spacing, fonts, link colors or dark-mode rendering. Send yourself a test email after installing the signature. The clipboard helper uses the browser's legacy copy command with a manual-selection fallback.

---

**Abdellah Bayar** · [Portfolio](https://abdellahbayar.com) · [LinkedIn](https://www.linkedin.com/in/abdellah-bayar/)
