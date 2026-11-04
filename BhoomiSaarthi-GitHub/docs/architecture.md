# BhoomiSaarthi — Architecture Notes

## Core workflow
1. Operator authenticates and obtains resident consent.
2. Documents are uploaded to private storage.
3. OCR/extraction service returns structured fields plus confidence.
4. Comparison workflow flags differences across documents.
5. Guidance retrieval uses verified official sources for the relevant state.
6. Human operator reviews results and explains them to the resident.
7. A summary/checklist is generated and the case is tracked.

## Design principles
- Human-in-the-loop for consequential interpretation.
- Show confidence and uncertainty; do not invent missing fields.
- Keep official procedural guidance jurisdiction-specific and source-linked.
- Minimize data collection and protect documents.
- Separate extracted facts, AI interpretation, and recommended next steps.
