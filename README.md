# Accessibility Baseline Reference

A comprehensive, unified accessibility baseline reference for **PDF, Word, Excel, PowerPoint, HTML, and CSS** — designed for use as an AI/LLM knowledge base.

## What's in This Repository

### [`Unified-Accessibility-Baseline-Reference.md`](./Unified-Accessibility-Baseline-Reference.md)

A single, self-contained Markdown file combining all **24 baselines** from the ICT Testing Baseline Portfolio. For each baseline it includes:

- **WCAG 2.2 Success Criteria** covered (with SC numbers and names)
- **Universal test checks** — the pass/fail items that apply across all formats
- **Format-specific implementation techniques** for:
  - **PDF** (using PDF-specific WCAG techniques: PDF1, PDF3, PDF4, PDF6, PDF9, PDF11, PDF16, PDF18, PDF21, etc.)
  - **Microsoft Word** (built-in Word accessibility features)
  - **Microsoft Excel** (built-in Excel accessibility features)
  - **Microsoft PowerPoint** (built-in PowerPoint accessibility features)
  - **HTML/CSS** (semantic HTML elements, ARIA, CSS techniques)
- **Exceptions** — where certain baselines don't apply to certain formats
- **Limitations and assumptions** from the source baselines

The document also includes:
- A quick-reference table mapping all WCAG 2.2 Level AA SCs to baseline numbers and applicable formats
- A format-specific exceptions summary table (which baselines apply to which formats)
- A PDF WCAG techniques reference table (PDF1–PDF22)
- An accessibility checker tools reference

## Source and Attribution

All baseline content is sourced from the **[ICT Testing Baseline Portfolio](https://github.com/atbcb/ICTTestingBaseline)** maintained by the **U.S. Access Board** (atbcb):

- **[Baseline for Electronic Documents v1.0](https://github.com/atbcb/ICTTestingBaseline/tree/main/_baselines/document-baselines)** — published September 30, 2024. Sets the standard for testing PDF, Word, Excel, PowerPoint, and all non-web electronic documents for Section 508 conformance.
- **[Baseline for Web v3.1](https://github.com/atbcb/ICTTestingBaseline/tree/main/_baselines/web-baselines)** — published April 1, 2024. Sets the standard for testing web content (HTML/CSS) for Section 508 conformance. Recognized as a Best Practice by the Federal CIO Council's Accessibility Community of Practice (ACOP).

The ICT Testing Baseline Portfolio establishes the minimum requirements for evaluating conformance with the [Revised Section 508 of the Rehabilitation Act of 1973](https://www.access-board.gov/ict) (29 U.S.C. 794d). Section 508 incorporates WCAG 2.0 Level A and AA by reference.

## Intended Use

This repository is designed to be ingested into AI/LLM knowledge bases (such as Palantir Vantage AI FDE) to enable:

- **Automated accessibility review** of documents and web content
- **AI-assisted remediation guidance** for specific document types and formats
- **Compliance checking** against Section 508 and WCAG 2.2 Level AA requirements
- **Training data** for accessibility-aware AI models

## Key Scoping Notes

- **Section 508 E205.4** exempts non-web documents from WCAG SCs 2.4.1 (Bypass Blocks), 2.4.5 (Multiple Ways), 3.2.3 (Consistent Navigation), and 3.2.4 (Consistent Identification)
- **WCAG SC 4.1.1 Parsing** is deprecated in WCAG 2.2 and auto-passes for all formats
- **Baselines 4, 19, and 23** (Repetitive Content, Frames/iFrames, Multiple Ways) are web-only and marked N/A for documents

## License and Use

This reference file is compiled from publicly available U.S. Government accessibility standards. The source ICT Testing Baseline Portfolio is published by the U.S. Access Board and is in the public domain. Attribution to the U.S. Access Board is appreciated.
