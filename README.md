# Scanner Code-barres Textile

Web app to scan textile barcodes and redirect to their Ecobalyse environmental impact page.

## Setup

```bash
cd barcode-scanner
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run

```bash
python app.py
```

Then open http://localhost:5000 in your browser.

## Usage

1. Allow camera access when prompted
2. Point your camera at a textile barcode (EAN-13, EAN-8, UPC, etc.)
3. The app automatically redirects to the Ecobalyse page for that product

You can also enter barcodes manually if camera access isn't available.

## Tech Stack

- **Backend**: Flask (Python)
- **Barcode scanning**: [html5-qrcode](https://github.com/mebjas/html5-qrcode) (open source)
