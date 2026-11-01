# NEBB — North East Bodyboarding Club

A minimal, responsive **demo homepage** for the North East Bodyboarding Club, centred on Northumberland and the North Sea.

**Tech:** HTML + CSS + SVG only. No WordPress, JavaScript, framework, package manager or build step required.

## Files

- `index.html` — all page content, sections and navigation
- `styles.css` — colours, layout, typography and mobile/tablet styles
- `assets/north-sea-wave.svg` — minimal line-art hero illustration (replaceable)
- `assets/northumberland-coast.svg` — minimal line-art coast illustration (replaceable)
- `assets/favicon.svg` — browser tab icon

## Preview locally

Open `index.html` in your browser. Or use the VS Code **Live Server** extension if you prefer automatic refresh.

## Edit the website

1. **Text:** open `index.html` and edit text between the HTML tags.
2. **Colours:** change the CSS variables in `:root` at the top of `styles.css`.
3. **Sections:** main page sections are labelled `id="about"`, `id="coast"`, `id="sessions"` and `id="membership"`.
4. **Imagery:** replace the SVG files in `assets/` with your own photos, then update the `src` and descriptive `alt` text of the matching `<img>` elements.
5. **Navigation:** each menu item points to a matching section ID; keep them in sync when renaming IDs.
6. **Membership:** the membership section currently says *coming soon*. It does **not** collect names, emails, passwords or payment details.
7. **Events:** listed activities are concepts, **not** real scheduled events. Replace the content when actual club plans exist.

## Deploy with Cloudflare Pages

Once this folder is in a GitHub repository:

1. In Cloudflare, open **Workers & Pages → Create → Pages → Connect to Git**.
2. Select your NEBB GitHub repository.
3. Choose **None** as the framework preset, set **Build command** to `exit 0` (or leave blank if the dashboard permits), and set the **Build output directory** to `.` (the repository root containing `index.html`).
4. Deploy. Cloudflare gives you a `*.pages.dev` address.
5. Open the Pages project's **Custom domains** and add `nebb.club`; follow the DNS prompts. Since the domain is already registered with Cloudflare, this is straightforward.

Cloudflare changes its dashboard labels occasionally; follow the current on-screen prompts if the wording differs.

## Before launching publicly

- Replace demo copy with confirmed club details and actual contact channels.
- Provide a privacy notice before collecting personal information.
- Keep member sign-in, password storage and payments on an established secure service when membership opens.
- Test mobile layouts, keyboard navigation, alt text and working links.
- Do not present proposed sessions as confirmed bookings.

Artwork in `assets/` is custom-created for this demo and can be freely edited as part of the project.