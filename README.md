# MathCell Helper – Prototype 2.1

MathCell Helper is an independent, browser-based prototype for capturing, displaying, storing and reusing mathematical formulas. Prototype 2.1 separates display formulas from executable spreadsheet formulas, adds a bilingual German/English interface, a light/dark switch and a small information menu for users.

MathCell Helper ist ein unabhängiger, browserbasierter Prototyp zum Erfassen, Anzeigen, Speichern und Wiederverwenden mathematischer Formeln. Prototyp 2.1 trennt Anzeigeformeln und ausführbare Tabellenformeln, ergänzt eine deutsch/englische Oberfläche, einen Hell-/Dunkel-Umschalter und ein kleines Informationsmenü für Nutzer:innen.

## Project structure / Projektstruktur

- `index.html` – HTML structure and linked resources
- `styles.css` – layout, colors, spacing, responsive UI, theme tokens and info menu styles
- `mathjax-config.js` – MathJax configuration
- `app.js` – application logic for preview, library, mapping, translation, import, export and copy functions
- `starter-library.json` – structured starter formulas with bilingual display labels
- `starter-library.csv` – tabular overview of the starter formulas

## Prototype 2.1 changes

- Version label changed to **Prototype 2.1 / Prototyp 2.1** in the interface and documentation.
- Starter formula names and categories are displayed bilingually where possible.
- Target program labels switch between German and English while keeping stable internal values.
- A new **Info** button opens a compact explanation menu.
- The menu includes workflow guidance, a short LaTeX explanation with common examples, limits of the prototype, a homepage link and a PayPal support link.

## Interface

The UI supports German and English via the small `DE` / `EN` buttons. A light/dark switch is included. The dark theme uses the green-black glass style from the existing project direction.

Die Oberfläche unterstützt Deutsch und Englisch über kleine `DE` / `EN`-Buttons. Ein Hell-/Dunkel-Umschalter ist enthalten. Das dunkle Theme nutzt den grün-schwarzen Glasstil aus der bestehenden Projektlinie.

## LaTeX help in the info menu

The info menu now includes a compact LaTeX section. It explains that LaTeX is used for the visible display formula, while the spreadsheet template remains responsible for executable cell formulas. The section also shows common examples such as `\frac{a}{b}`, `\sqrt{x}`, `x_1`, `x^2` and `\pm`.

Two external learning links are included for users who need more context:

- LaTeX overview: https://en.wikipedia.org/wiki/LaTeX
- Common LaTeX symbols: https://www.overleaf.com/learn/latex/List_of_Greek_letters_and_math_symbols

Die Hilfe enthält jetzt einen kurzen LaTeX-Abschnitt. Er erklärt, dass LaTeX für die sichtbare Anzeigeformel genutzt wird, während das Spreadsheet-Template für ausführbare Zellformeln zuständig bleibt. Außerdem werden typische Beispiele wie `\frac{a}{b}`, `\sqrt{x}`, `x_1`, `x^2` und `\pm` gezeigt.

## Starter library

On first launch, the app prepares a small starter library directly in the browser. It includes:

- `pq_formula_x1` / p-q formula x₁ / p-q-Formel x₁
- `pq_formula_x2` / p-q formula x₂ / p-q-Formel x₂
- `circle_area` / Circle area / Kreisfläche
- `margin_ratio` / Margin ratio / Marge / Deckungsquote
- `percentage_change` / Percentage change / Prozentuale Veränderung

These formulas can be selected with **Load / Laden** and transferred into the input fields. The generated spreadsheet formula can then be copied into another program.

Beim ersten Start legt die App eine kleine Starter-Bibliothek lokal im Browser an. Die Formeln können über **Laden** ausgewählt und in die Eingabefelder übertragen werden. Danach kann die erzeugte Tabellenformel kopiert und in ein anderes Programm eingefügt werden.

## Formula workflow

1. Enter or load a formula reference.
2. Use a display formula / LaTeX expression for visual rendering and SVG export.
3. Use a spreadsheet formula template with placeholders such as `{{p}}`, `{{q}}`, `{{Revenue}}` or `{{Cost}}`.
4. Map each placeholder to a cell reference or fixed value.
5. Generate a spreadsheet formula for Excel English, Excel German, Google Sheets or Apple Numbers.
6. Copy the result or save the reference to the local library.

## JSON and CSV export

The library is stored locally in the browser. **JSON export** is the main backup and transfer format because it preserves all structured fields: name, bilingual display labels, category, LaTeX, template, target app, mapping and notes.

A **CSV export** is also available for spreadsheet-oriented workflows. CSV is useful for overview tables or documentation, but JSON remains the better format for importing the full library back into MathCell Helper.

Die Bibliothek wird lokal im Browser gespeichert. **JSON** ist das Hauptformat für Backup und Transfer, weil alle strukturierten Felder erhalten bleiben. **CSV** ist zusätzlich für Tabellenübersichten oder Dokumentation vorhanden, eignet sich aber weniger gut für einen vollständigen Re-Import.

## Import

Use **Import** to load a previously exported JSON library. Import currently replaces the local library with the imported file.

Über **Import** kann eine zuvor exportierte JSON-Bibliothek geladen werden. Der Import ersetzt aktuell die lokale Bibliothek durch die importierte Datei.

## MathJax

MathJax is loaded through jsDelivr. An internet connection is required when loading the app for the first time or when the CDN resource is not cached.

## Limitation

This prototype does not directly modify Excel, Google Sheets, Numbers or other Office programs. Direct writing into active spreadsheet cells would require a later Excel Add-in, Google Sheets Add-on or browser/desktop integration. This version provides a controlled copy/paste and export workflow.

## Links

- Homepage: https://jerdogan.art/
- Support: https://www.paypal.com/ncp/payment/CNJYL8TXEZYPY

## Copyright

© 2026 Jeremias Erdogan  
Contact: Jeremiaserdogan@gmail.com
