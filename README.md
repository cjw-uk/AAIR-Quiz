# ISACA AAIR Exam Prep Quiz

Unofficial interactive study quiz for **ISACA Advanced in AI Risk (AAIR)**.

> **Disclaimer:** This is an independent study aid. It is **not affiliated with, endorsed by, or sponsored by ISACA**. Questions are original practice items and are **not** copied from ISACA QAE or official exams. Always verify against the [official AAIR exam content outline](https://www.isaca.org/credentialing/aair/aair-exam-content-outline).

## Live quiz

- **GitHub Pages:** https://cjw-uk.github.io/AAIR-Quiz/
- **Repository:** https://github.com/cjw-uk/AAIR-Quiz

## Exam snapshot

| Item | Detail |
|------|--------|
| Credential | ISACA Advanced in AI Risk (AAIR) |
| Exam length | 90 questions, 150 minutes |
| Domains | 3 (governance, lifecycle, program management) |

### Domains (official weighting)

1. **AI Risk Governance and Framework Integration** — 37%
2. **AI Life Cycle Risk Management** — 21%
3. **AI Risk Program Management** — 42%

## Question bank

| Domain | Questions | Share of bank |
|--------|-----------|---------------|
| 0 — Governance & Framework Integration | 150 | ~39% |
| 1 — Life Cycle Risk Management | 76 | ~20% |
| 2 — Risk Program Management | 157 | ~41% |
| **Total** | **383** | 100% |

Coverage includes beginner / intermediate / advanced items, knowledge and scenario stems, and some multi-select questions. Subtopics span 1A–1F, 2A–2D, and 3A–3F, plus ISACA’s “other skills tested” themes (ERM integration, risk appetite, contracts/IP, shadow AI, human oversight, AI-for-risk, change management, etc.).

## Features

- Dark / light mode
- Domain (objective) selection
- Configurable quiz length (up to 90)
- Progress tracking
- Explanations + authoritative `learnMore` links
- Results with objective breakdown and study recommendations

## Authoritative learnMore sources (examples)

- [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework)
- [NIST.AI.100-1 PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)
- [NIST AI RMF Playbook](https://www.nist.gov/itl/ai-risk-management-framework/nist-ai-rmf-playbook)
- [EU AI Act overview](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
- [OECD AI Principles](https://oecd.ai/en/ai-principles)
- [ISO/IEC 42001](https://www.iso.org/standard/81230.html)
- [ISACA AAIR](https://www.isaca.org/credentialing/aair)
- [AAIR exam content outline](https://www.isaca.org/credentialing/aair/aair-exam-content-outline)
- [MITRE ATLAS](https://atlas.mitre.org/)
- [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [NIST SP 800-61](https://csrc.nist.gov/pubs/sp/800/61/r2/final)

## Local use

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Architecture

Single-file SPA (`index.html`) with embedded CSS, quiz engine, and question bank — same pattern as [SC-100-200-Quiz](https://github.com/cjw-uk/SC-100-200-Quiz), adapted for AAIR only (no SC-100/SC-200 content).

## License

Study aid for personal use. Official ISACA materials remain ISACA property; do not confuse this quiz with official QAE.
