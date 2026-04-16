# RevEng — Cold Outreach Testing

Simple repo for storing, rendering, and sanity-checking cold outreach email sequences before they go out.

## Structure

- sequences/  — each outreach cadence in its own folder
- test-data/  — A/B Test data and findings
- previews/   — rendered emails land here (gitignored)

## Setup

    pip install -r requirements.txt

## Usage

    python scripts/render.py sequences/generate.py-q2
    python scripts/spam-check.py sequences/generate.py-q2/step-1-intro.md
    python scripts/link-check.py sequences/generate.py-q2/step-1-intro.md
