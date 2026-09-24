<a href="https://svetlecereklame3dart.rs/"><img src="media/cover.jpg" alt="3D Art Kragujevac, home page on a laptop and a phone" width="100%"></a>

# 3D Art Kragujevac

Eight-page site for a Kragujevac sign workshop, with over a hundred photos of finished signs and the materials explained in plain words.

**[svetlecereklame3dart.rs](https://svetlecereklame3dart.rs/)** · [Case study (in Serbian)](https://svilenkovic.com/radovi/3d-art-kragujevac) · [Srpski](README.sr.md)

> [!NOTE]
> Client project. The source code belongs to the client and stays in a private repository. This page describes what I built and how.

<table>
  <tr><td><b>Client</b></td><td>3D Art Kragujevac</td></tr>
  <tr><td><b>Industry</b></td><td>Illuminated signs, 3D letters, CNC and laser cutting</td></tr>
  <tr><td><b>Location</b></td><td>Kragujevac, Serbia</td></tr>
  <tr><td><b>Type</b></td><td>Multi-page website</td></tr>
  <tr><td><b>My role</b></td><td>Design, development, SEO, hosting and maintenance</td></tr>
  <tr><td><b>Stack</b></td><td>PHP 8.3, PHPMailer, nginx, FastCGI cache, AVIF/WebP</td></tr>
</table>

## About the project

3D Art Kragujevac builds and installs illuminated signs all over Serbia. It also cuts and engraves for anyone who brings a file, on a 200 x 130 cm CNC router and a 130 x 100 cm laser. People choose a sign maker by looking at work already done, and most of them have never heard of alubond or Styrodur. The site had to show a lot of finished signs and explain the materials in plain words.

I split the content into eight pages, one per product group plus the CNC and laser service, so each has its own title and a link the owner can send to a customer. The illuminated signs page alone covers eight types, each with a short description, a feature list and its own gallery. Four pages of the live site had canonical tags pointing to another domain, left over from the template the site started from. I fixed them, and a search for that domain now runs before every deploy.

## What I built

- Galleries with more than a hundred photos, in a lightbox that works with the arrow keys, Esc and a screen reader
- A quote form with seven subjects behind a shared spam gate; if the gate is unavailable, the form stops and shows the phone number
- Images re-encoded as WebP from about 9.4 to 7.4 MB in total, with nginx serving AVIF to browsers that accept it
- A call, Viber and WhatsApp bar at the bottom of phone screens, recoloured until it passed the contrast check
- LocalBusiness, Service and FAQ structured data, without the unsupported five-star rating the site used to carry
- Stylesheet and script URLs versioned by file modification time, so returning visitors get new CSS without clearing their cache

## Results

| | Performance | Accessibility | Best practices | SEO |
| :-- | :-: | :-: | :-: | :-: |
| Mobile | 99 | 100 | 100 | 100 |
| Desktop | 98 | 100 | 100 | 100 |

PageSpeed Insights, lab test of the live site, September 2026. Security headers: 6 of 6. HTML validator: no errors. axe accessibility check: no violations. Structured data: `FAQPage`, `ItemList`, `LocalBusiness`.

## Screenshots

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="3D Art Kragujevac, home page on a 1440 px screen"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="3D Art Kragujevac, home page on a phone"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="Two buttons right below the headline, then the &quot;Zašto izabrati 3D Art?&quot; (Why choose 3D Art?) section begins">
<sub>Two buttons right below the headline, then the "Zašto izabrati 3D Art?" (Why choose 3D Art?) section begins</sub>

<img src="media/inner-2.webp" alt="Four reasons in one row, leading into &quot;Naši proizvodi&quot; (Our products)">
<sub>Four reasons in one row, leading into "Naši proizvodi" (Our products)</sub>

---

<sub>Built by [D. Svilenković](https://svilenkovic.com).</sub>
