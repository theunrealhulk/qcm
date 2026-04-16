# QCM - Coding Quiz Test

A web-based multiple-choice quiz application for testing programming knowledge across various topics and difficulty levels.

## Features

- 10 programming topics: JavaScript, TypeScript, Node.js, React, Angular, C#, ASP.NET, PHP, Laravel, and Git
- 7 difficulty levels per topic
- Configurable quiz length (5-60 questions)
- Per-question countdown timer
- Single and multiple-answer questions
- Dark/light theme toggle
- Detailed answer explanations
- Score tracking and results breakdown

## Quick Start

No installation required. Open `index.html` in any modern browser.

```bash
# Option 1: Direct open (Linux)
xdg-open index.html

# Option 2: Local server
python3 -m http.server 8000
# Visit http://localhost:8000
```

## Usage

1. Select a topic from the dropdown menu
2. Adjust difficulty (1 = easy, 7 = hard)
3. Set number of questions
4. Configure timer per question (seconds)
5. Click "Start Quiz"
6. Answer questions before time runs out
7. Review results at the end

## Project Structure

```
qcm/
  index.html          # Main application
  questions/          # Question banks
    javascript/
    typescript/
    nodejs/
    react/
    angular/
    C#/
    ASP.net/
    PHP/
    laravel/
    git/
```

## Question Format

Questions are stored as JSON files (`questions/<topic>/<difficulty>.json`):

```json
{
  "question": "Question text here",
  "options": ["Option A", "Option B", "Option C", "Option D"],
  "correctOptions": ["Correct answer"],
  "time": 25,
  "details": "Explanation of the answer"
}
```

## Browser Support

Any modern browser (Chrome, Firefox, Safari, Edge).
