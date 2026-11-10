# Advoc8 master admin prototype

[Open the prototype](https://regoke.github.io/Master-admin/)

Faithful baseline of Anthony Albanese's master person edit page, captured from Advoc8 staging on 10 November 2026. The original product CSS, fonts, navigation, fields, content and right-hand cards are preserved. Fixed email and phone fields remain as specified in the handover.

## Local interactions

- Edit fields, unlock or clear first/last names, and add/remove name rows.
- Search/select existing dropdown choices and clear selections.
- Create, edit and delete addresses, including after all addresses have been removed.
- Populate address fields from captured templates, choose or enter an address type, and set one primary address per type.
- Close dialogs with the header close button or Escape; keyboard focus stays within open dialogs.
- Update and archive show simulated feedback. Changes reset on refresh.

This prototype has no Advoc8 backend and never submits changes to staging. Sidebar destinations and other admin screens are outside scope. Supporting secondary dialogs are demonstration placeholders rather than verified implementations.

## Edit and preview

Unzip `source.zip` to get editable HTML, CSS, JavaScript and assets under `source/`, plus the build script. No dependencies are needed.

```sh
python3 -m http.server 6274
```

Open `http://127.0.0.1:6274/source/` for editable source or `http://127.0.0.1:6274/` for the built standalone page.

## Build and publish

```sh
python3 scripts/build.py
```

This builds root `index.html` with its fonts, images, CSS and JavaScript embedded, plus `source.zip` containing editable source and the build script. Publish the built `index.html`, `source.zip` and this README together. GitHub Pages serves `main` from the repository root; `.nojekyll` disables Jekyll processing.

See [HANDOVER.txt](HANDOVER.txt) for scope, product context, Figma references and future contact-details work.
