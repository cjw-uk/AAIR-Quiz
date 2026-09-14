# CLAUDE.md

Guidance for AI assistants working in this repository.

## Project Overview

Single-page **ISACA AAIR (Advanced in AI Risk)** exam prep quiz. Standalone HTML application with dark/light mode, domain selection, quiz length control, explanations, and results breakdown.

**Unofficial study aid** — original questions only; not affiliated with ISACA.

## Architecture

### Single-File Application
- **File**: `index.html` — HTML structure, CSS, JavaScript engine, and embedded `questionBank`
- **Pattern**: Vanilla JS SPA with global state
- **No build step**: open directly in a browser

### Application State
- `currentExam` (always `AAIR` in practice)
- `selectedObjectives`, `quizQuestions`, `userAnswers`, `currentQuestionIndex`
- Flow: Setup → Quiz → Results → Setup

### Question Bank
```js
questionBank['AAIR'] = {
  objectives: [
    'AI Risk Governance and Framework Integration (37%)',  // objective 0
    'AI Life Cycle Risk Management (21%)',                 // objective 1
    'AI Risk Program Management (42%)'                     // objective 2
  ],
  questions: [ /* { objective, difficulty, scenario?, question, options, correct, explanation, learnMore } */ ]
}
```

### Key Functions
- `startQuiz()`, `displayQuestion()`, `submitAnswer()`, `finishQuiz()`
- `calculateResults()`, `generateStudyRecommendations()`
- `toggleTheme()`, `shuffleArray()`, `arraysEqual()`

## Content Rules
- AAIR only — **no SC-100 / SC-200 / Microsoft branding**
- Original questions; do not copy paid ISACA QAE
- Keep `learnMore` URLs authoritative (NIST, EU AI Act, OECD, ISO, ISACA, ATLAS, OWASP, etc.)
- Target ~37/21/42 domain weighting; maintain beginner/intermediate/advanced coverage per subtopic

## Local Development
```bash
python3 -m http.server 8000
```

## Related
UX/architecture reference: https://github.com/cjw-uk/SC-100-200-Quiz
