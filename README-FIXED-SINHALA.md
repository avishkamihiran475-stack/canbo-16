# Hotel Canbo Fixed Version - Sinhala Notes

මෙම zip එකේ folders දෙකක් වැදගත්:

## 1. `dist/`
මෙය Vite දැනුමක් නැතුව upload කරන්න පුළුවන් static website version එකයි. Hosting වලට upload කරනවා නම් `dist` folder එක ඇතුළේ තියෙන files upload කරන්න.

Main pages:
- `index.html`
- `rooms.html`
- `gallery.html`
- `restaurant.html`
- `attractions.html`
- `about.html`
- `contact.html`

## 2. `src/`
මෙය source code එකයි. Vite use කරන developer කෙනෙකුට මේකෙන් rebuild කරන්න පුළුවන්.

## Applied fixes

- `/pages/rooms.html` routing issue එක වෙනුවට root-level pages (`/rooms.html`, `/contact.html`, etc.) හැදුවා.
- Home page fake availability alert එක ඉවත් කරලා WhatsApp inquiry flow එකක් දැම්මා.
- Contact form fake “sent” message එක ඉවත් කරලා WhatsApp/Email send options දැම්මා.
- Contact form labels වල `for`/`id` accessibility fix කළා.
- Navbar active page detection bug fix කළා.
- Mobile menu `aria-expanded` update කළා.
- Escape key එකෙන් mobile menu close වෙන්න හැදුවා.
- Modal/lightbox z-index issue fix කළා.
- Loader artificial 1.5s delay එක 0.35s කළා.
- Gallery lightbox items keyboard accessible කළා.
- `target="_blank"` links වල missing `rel="noopener noreferrer"` fix කළා.
- Attractions page එකේ unfinished placeholder text ඉවත් කළා.
- Footer year dynamic/current-year compatible කළා.
- `robots.txt` සහ `sitemap.xml` add කළා.
- “Online Booking” wording misleading නිසා “Booking Inquiry” ලෙස වෙනස් කළා.

## Important note

මෙය තවම static website එකක්. Backend/database/real booking engine එකක් නැහැ. Booking/contact messages userගේ WhatsApp හෝ email app එකෙන් send වෙනවා.

Real booking system එකක් අවශ්‍ය නම් පසුව backend/API හෝ Formspree/Netlify Forms/Google Sheets integration එකක් add කරන්න.

## Latest UI fixes applied in this version

- Home page footer එකට උඩින් තියෙන CTA section එකේ **Book Now** button එකට white border + soft gold hover style add කළා.
- Navbar active page color එක green වලින් luxury gold/gold-light style එකකට update කළා.
- Navbar links වල font එක luxury feel එකක් ඇති කරන්න `Cormorant Garamond` style එකට update කළා.
- Page load වෙද්දී plain HTML විදිහට flash වෙන FOUC problem එකට CSS direct load වෙන `site.css` link එක add කළා.
- Mobile menu overlay එකට clear **X close button** එකක් add කළා.
- Mobile view එකේ **Back to Top** button එක hide වෙන issue එක fix කරලා bottom-center position එකට දාලා තියෙනවා.
- Mobile footer text only mobile view එකේ center align කළා.
- Footer credit එක **Design By Growth Code Studio** ලෙස update කරලා clickable Facebook link එකක් add කළා.
- Growth Code Studio link එකට shining orange color/glow style එකක් add කළා.
- Website headings/titles වලට luxury `Playfair Display` font එක add කළා. Body/description text එක readable Inter font එකෙන්ම තියෙනවා.
- Home hero section එක single image වෙනුවට existing images use කරන smooth fade slideshow එකක් කළා.
- Mobile navbar එකේ Book Now button spacing/right alignment improve කළා.
- Home hero buttons දෙකට hover වෙද්දී light gold border/glow/lift effect add කළා.

## Local PC එකේ open කරන විදිහ

VS Code terminal එකේ:

```bash
npm install
npm run dev
```

Browser URL එක සාමාන්‍යයෙන්:

```text
http://localhost:5173/
```

Vite install කරලා build කරන්න බැරි වුණත්, `dist/` folder එක static version එකක් විදිහට browser/server එකෙන් open කරන්න පුළුවන්.


## Latest mini update

- Added `wedding.html` page with 3 wedding/event package options.
- Removed floating phone button; Back-to-top is now left and WhatsApp is right.
- Mobile menu now has a solid green background and centered Hotel Canbo logo.
