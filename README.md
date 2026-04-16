# RevEng — Cold Outreach Testing

Simple repo for storing, rendering, and sanity-checking cold outreach email sequences before they go out.

## Structure

- sequences/  — each outreach cadence in its own folder
- snippets/   — reusable blocks (signatures, CTAs)
- test-data/  — sample lead data
- scripts/    — render, spam-check, link-check
- previews/   — rendered emails land here (gitignored)

## Setup

    pip install -r requirements.txt

## Usage

    python scripts/render.py sequences/saas-founders-q2
    python scripts/spam-check.py sequences/saas-founders-q2/step-1-intro.md
    python scripts/link-check.py sequences/saas-founders-q2/step-1-intro.md
