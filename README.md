# Allocator Pitch Deck Analyzer Demo

A tool for quickly screening pre-seed pitch decks against investment criteria. Upload a PDF, get pass/fail verdicts per criterion, and draft a response email — all in one view.

## What it does

- Upload any pitch deck as a PDF
- Evaluates the deck against configurable criteria (editable before each run)
- Returns a per-criterion **PASS / FAIL** with a short explanation
- Shows an overall **PASS / FAIL** verdict
- Auto-generates a draft email to the founder — ready to review and send

## Default criteria

1. Is the founder(s) US-based?
2. Does the thesis align with AI in the resilience economy (climate resilience, supply chain resilience, grid modernization, food & health sustainability)?
3. Is the funding stage pre-seed, seed, or Series A?

You can edit, add, or remove criteria directly in the UI before analyzing.

## Setup

**Requirements:** Python 3 and an [Anthropic API key](https://console.anthropic.com/)

```bash
# 1. Clone the repo
git clone https://github.com/brandonyuen111/pitch-deck-analyzer
cd pitch-deck-analyzer

# 2. Start the local server
python3 server.py

# 3. Open in your browser
open http://localhost:8765
```

Then paste your Anthropic API key into the **API Key** field at the top of the left panel.

## Usage

1. Enter your Anthropic API key
2. Upload a pitch deck PDF (drag & drop or browse)
3. Edit the criteria if needed
4. Click **Analyze Deck**
5. Review the results — a draft email modal opens automatically
6. Edit the email if needed and click **Send**
