# PDF Title Metadata

This directory contains PDF files for the portfolio site. To ensure browser tabs display "David Weinflash" as the title when PDFs are opened directly, the PDF metadata needs to be updated.

## Updating PDF Titles

### Install exiftool

```bash
brew install exiftool
```

### Update all PDFs in this directory

```bash
cd /Users/dweinflash/Developer/dweinflash.github.io/assets/pdf
exiftool -overwrite_original -Title="David Weinflash" *.pdf
```

### Update a single PDF

```bash
exiftool -overwrite_original -Title="David Weinflash" filename.pdf
```

## What this does

- Sets the internal PDF title metadata to "David Weinflash"
- This title appears in the browser tab when the PDF is opened directly
- The `-overwrite_original` flag prevents creating `.pdf_original` backup files

## When to use this

Run this command whenever you add new PDFs to this directory to ensure consistent browser tab titles.
