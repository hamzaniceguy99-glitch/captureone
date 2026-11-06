# Capture One — holiday accommodation · ostend

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `captureone.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/captureone.mjs`).
> To change the content, edit that file and run `node build.mjs captureone` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@captureone.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($Per night / $Fixed rent / $Declined) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
We are Capture One, a company based in Ostend on the Belgian coast, operating holiday flats and holiday homes since March 2024. Everything about how we are set up comes down to one question, and it is worth asking of anyone in this trade: whose name is on the contract with the guest? When a company lets accommodation in its own name, as the operator, it needs no professional authorisation to do so, and the guest knows exactly who is responsible for the stay. When a company instead manages a property for its owner in return for a commission, that is a regulated activity in Belgium, reserved to estate agents registered with the professional institute, and the protected titles that go with it. We do the first. Owners who want their property put to work lease it to us for a fixed rent and we operate it ourselves, which keeps the arrangement on the right side of that line and gives the owner one counterparty instead of a stream of guests. Every unit is notified to the regional tourism authority, holds a fire safety certificate from the mayor, and shows its registration number on every listing. Site: captureone.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
