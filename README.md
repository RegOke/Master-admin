# Advoc8 master admin prototype

[Open the prototype](https://regoke.github.io/Master-admin/)

Anthony Albanese's master person edit page, based on Advoc8 staging and updated to Figma frame 438:4982 in Custom contact details. Contact Details now has repeatable email and phone rows, selectable or custom names, direct red trash buttons, and compact address cards. The rest of the page retains the captured product CSS, fonts, fields and supporting cards.

## Local interactions

- Edit fields, unlock or clear first/last names, and add/remove name rows.
- Search/select existing admin dropdown choices and clear selections.
- Add/remove email and phone rows, select a contact name, or use Add new email/phone name and Choose existing to enter a custom name.
- Use address three-dot menus to edit/delete addresses and the copy control to copy their text.
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
