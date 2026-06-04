# MathCell Helper – Prototype for Math Formula Workflows

MathCell Helper is an independent browser-based prototype for capturing, displaying, saving and reusing mathematical formulas.

Formulas can be used as LaTeX, as plain formula text or as rendered SVG files for document-based workflows.

Live version: https://mathcell-helper.netlify.app

## Purpose

The project supports a lightweight workflow for working with mathematical notation across browsers, documents and presentation tools.

It is intended as a practical helper for:

* writing and previewing LaTeX formulas
* rendering formulas with MathJax
* saving reusable formula references locally in the browser
* copying formula text into other programs
* exporting rendered formulas as SVG files
* supporting document-oriented workflows without a complex software environment

## Project structure

This version separates structure, styling, configuration and behavior into individual files:

* `index.html` – HTML structure and resource links
* `styles.css` – layout, colors, spacing, responsive presentation and help box
* `mathjax-config.js` – MathJax configuration
* `app.js` – application logic for preview, local storage, import, export and copy functions

## Usage

1. Open `index.html` directly in a browser or use the live version.
2. Enter a formula name, category, LaTeX formula and optional note.
3. Use **“Update preview”** to check whether the formula is rendered correctly.
4. Use **“Save formula”** to store the formula reference locally in the browser.
5. Use **“Load”** to bring a saved formula back into the input fields.

## Using formulas in other programs

* **“Copy formula text”** copies the text / LaTeX version of the formula. It can be pasted into documents, spreadsheets, notes or other working environments.
* **“Download SVG”** creates an image file of the rendered formula. This file can be inserted into programs such as Pages, Keynote, Numbers, Word or PowerPoint.

## Exporting and importing the formula library

The entered formulas are stored locally in the browser.

With **“Export library”**, a JSON file containing all saved formula references can be downloaded. This file can be used as a backup or transferred to another device.

With **“Import library”**, a previously exported JSON file can be loaded again. During import, the current local library is replaced by the imported file.

## MathJax

MathJax is loaded via jsDelivr. An internet connection is required when loading the application for the first time.

## Limitations

This prototype does not directly modify other programs and is not an official extension for any external software.

It demonstrates an independent workflow for collecting, rendering, copying and exporting mathematical formulas in a reusable way.

## Context

MathCell Helper is part of Jeremias Erdogan’s broader interdisciplinary practice between digital tools, web prototypes, document workflows and accessible interface development.

Website: https://jerdogan.art

## Author

© 2026 Jeremias Erdogan
