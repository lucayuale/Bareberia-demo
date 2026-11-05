# OBSIDIAN — Barber Studio · Booking Demo

**A premium barbershop website concept by VYB.**  
**Demo project · Fictional brand · English / Español**

Obsidian is an interactive example of a website VYB can build for barbershops: editorial visual design, responsive layout, services and pricing, gallery, contact area, and an appointment-booking experience powered by **Setmore**.

> **Please note:** Obsidian is **not a real barbershop**. The brand, address placeholders, sample hours, services and prices are illustrative. This repository is a **portfolio demo** and does not represent an active business.

## What's included

| Feature | Description |
| --- | --- |
| **Booking version** | Appointment buttons open an embedded Setmore booking page, with a link to open it separately. |
| **Responsive design** | Desktop and mobile layouts with a mobile navigation menu. |
| **Two languages** | English and Spanish, selectable from the header. |
| **Services and pricing** | Editable example services, durations and prices. |
| **Visual gallery** | Photo gallery with an interactive image viewer. |
| **Accessible interactions** | Keyboard-friendly booking dialog, Escape-to-close, and accessible page landmarks. |
| **Static website** | HTML, CSS and vanilla JavaScript; no backend or package installation needed. |

## Live demo

Once GitHub Pages is enabled, open the website using the **Pages URL shown in the repository's GitHub settings**. No public deployment URL is included here until one is actually configured.

### Booking demonstration

The Booking interface connects to the demonstration Setmore account configured in [`config.js`](config.js). **This is a testing connection, not a real barbershop's reservation service.** Interacting with Setmore could create an appointment in the demo calendar: use it only with permission from the owner of that account. Setmore controls availability, booking confirmation, cancellation and notifications; this static site does not store appointment data.

If Setmore or the embedding is unavailable, the booking window offers an external opening option. External services and remote images require internet access.

## Project structure

```text
.
├── index.html       # The published Booking website
├── styles.css       # Layout, colors and responsive styles
├── app.js           # Interactions, languages, booking and gallery
├── config.js        # Public demo content and Setmore URL
├── favicon.svg      # Demo icon
├── .nojekyll        # GitHub Pages static-site compatibility
└── README.md        # Documentation shown on GitHub
```

**Only the Obsidian Booking build is included here.** The Basic build, other example businesses and the private source/template tools are not part of this publication package.

## Publish with GitHub Pages

This folder is already arranged with `index.html` at its root. No build step is required.

1. Open the **existing repository** on GitHub.
2. Extract the ZIP on your computer; **upload the contents of the extracted folder**, not the ZIP itself or an enclosing folder.
3. Commit the files to your repository's default branch (typically `main`).
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**, then select the branch containing the files and **`/(root)`**. Save.
6. Once GitHub shows the public Pages URL, open it and check desktop, mobile, both languages and the Booking button.

If the repository already contains unrelated files or a different Pages workflow, inspect it before replacing anything. GitHub Pages may require the relevant repository settings and permissions to be enabled.

## Run locally

From the extracted folder:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080` in your browser. On Windows, `py -m http.server 8080` is also available if Python is installed.

## How to customize for a real client

Edit the public values in [`config.js`](config.js) and test again:

- `business`: name, tagline and demo notice.
- `brand`: design colors and logo settings.
- `images`: hero, lookbook and gallery assets.
- `businessDetails`: address, hours and notes.
- `contact`: public email, phone, WhatsApp and social accounts.
- `services`: prices, durations and descriptions.
- `booking.url`: the **client's own** Setmore booking page, not the VYB demo account.
- `seo`: page title and description.

For ongoing template development, use the original VYB Obsidian source project and regenerate the Booking build rather than editing the deployed build as your only copy.

**Never commit passwords, Setmore API credentials, private tokens or personal customer data to a public repository.** Remove sample content and the demo notice only after replacing it with real, confirmed business information. Also review image usage rights before commercial deployment.

## Technology and dependencies

HTML5 · CSS3 · JavaScript (no framework) · Setmore Booking (third-party) · Google Fonts (remote) · Unsplash image URLs (remote).

This demo includes a `noindex, nofollow` directive because it represents a fictional business rather than a public local barbershop. Remove or revise that directive, and configure the real business SEO and canonical URL, only when publishing a genuine client website.

---

## Español — Sobre este proyecto

**Obsidian** es una demostración de una página **Booking** para barberías desarrollada por **VYB**. Incluye diseño adaptable, servicios y precios de ejemplo, galería interactiva, selector de español/inglés y reservas integradas con Setmore.

**No es una barbería real.** La información comercial es ficticia. La cuenta Setmore corresponde a pruebas y no debe utilizarse para turnos de clientes reales. Las imágenes y fuentes externas necesitan conexión a internet.

Para subirla a GitHub, descomprimí el ZIP y colocá **los archivos directamente en la raíz del repositorio que ya tienen**. En **Settings → Pages** elegí **Deploy from a branch**, la rama correspondiente y **`/(root)`**. No hace falta ejecutar Node ni compilar nada.

Cuando tengan una barbería cliente, hay que reemplazar datos de prueba, imágenes, contacto y cuenta de Setmore por información autorizada. No se deben subir credenciales.

*VYB · Website concept and development · 2026*
