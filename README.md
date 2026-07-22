# AI Reconciliation Tool

**By [VJ GST & Tax Consultancy](https://www.linkedin.com/in/vijaya-suryan)**
Govt. of India Certified GST Practitioner (Enrolment No. 332500009598GPC)

A free, browser-based reconciliation tool for GST (Portal vs. Books) and
Bank (Statement vs. Books) matching — built for tax practitioners and
accountants who need a fast, private way to reconcile records without
uploading client data anywhere.

**🔗 Live site:** `https://<your-github-username>.github.io/<repo-name>/`
*(update this link once GitHub Pages is live)*

The site has two pages:
- **`index.html`** — a landing page explaining what the tool does, how your data is handled, and how to use it
- **`app.html`** — the actual reconciliation tool, linked from the landing page

Visitors land on the explanation first and click through to the tool once they're comfortable with it.

---

## What it does

- **GST Reconciliation** — matches GSTR-2B/Portal data against your books
  by invoice number, GSTIN, date, and tax amount, and flags mismatches,
  missing invoices, and duplicates.
- **Bank Reconciliation** — matches bank statement entries against your
  books by date and amount.
- **Rule-based matching engine** — deterministic scoring, not a black box.
  Every match, partial match, and exception is explainable.
- **Optional AI observations** — bring your own Anthropic API key to get
  plain-English summary observations and suggested action items layered
  on top of the rule engine's results. Entirely optional — the tool is
  fully functional without it, and the report always tells you honestly
  whether AI was used or not.
- **Multiple export formats** — Excel, CSV, PDF audit report, or copy to
  clipboard.
- **Flexible input** — paste data directly, upload CSV/Excel, or drag and
  drop files.

## Privacy — how your data is handled

This tool runs **entirely in your browser**. There is no backend server
and no database.

- Uploaded files are parsed client-side using JavaScript. They are never
  transmitted anywhere.
- If you choose to enter an Anthropic API key for AI observations, only a
  small statistical summary and a sample of mismatched rows are sent
  directly from your browser to Anthropic's API — never the full dataset,
  and never through any server of ours.
- Nothing is logged, stored, or retained once you close the tab.

If you're a fellow practitioner using this for client work: treat this the
same as any spreadsheet on your own machine — the responsibility for
where you run it and what data you paste in is yours, but the tool itself
never phones home.

## How to use it

1. Open the landing page (link above) and skim what it does and how your data is handled.
2. Click **Launch the tool**.
3. Choose **GST Reconciliation** or **Bank Reconciliation**.
4. Load Source A (Portal/Bank Statement) and Source B (Books) — paste,
   upload CSV/Excel, or drag and drop.
5. Map your columns to the required fields.
6. (Optional) Enter an Anthropic API key if you want AI-generated
   observations alongside the rule-based results.
7. Run the reconciliation and review matched, partial, and unmatched
   entries.
8. Export as Excel, CSV, or a PDF audit report.

## Tech stack

Single self-contained HTML file — HTML, CSS, and vanilla JavaScript.
No build step, no dependencies to install. Uses SheetJS (bundled) for
Excel parsing/export.

## Disclaimer

This tool is provided as a productivity aid for reconciliation work. It
is **not** a substitute for professional judgment, and results should
always be verified against the GST portal (GSTR-2B) and your books of
account before filing or reporting. VJ GST & Tax Consultancy accepts no
liability for decisions made solely on the basis of this tool's output.
For anything with compliance or filing implications, consult a qualified
GST practitioner or chartered accountant.

## License

All rights reserved. The tool is free to use as hosted, but the source
code may not be copied, modified, or redistributed without permission.
See [LICENSE](./LICENSE) for details.

## Contact

**J. Vijayasuryan Jaisankar**
GST Practitioner · VJ GST & Tax Consultancy
📧 suryavijay3012@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/vijaya-suryan)
