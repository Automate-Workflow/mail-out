# Contributing to MailOut AI

First off, thank you for considering contributing to **MailOut AI**!  
Whether you're fixing bugs, improving UI, optimizing prompts, or enhancing spam detection — contributions are always welcome.

---

# 📌 Project Overview

MailOut AI is a Chrome Extension that adds:

- AI-powered Gmail summarization
- Strict email categorization
- Hybrid spam detection
- Native Gmail UI integration

Tech stack includes:

- Chrome Extension (Manifest V3)
- JavaScript
- Gemini API
- Gmail DOM injection

---

# 🚀 Getting Started

## 1. Fork the Repository

Click the **Fork** button on GitHub.

Then clone your fork:

```bash
git clone https://github.com/YOUR_USERNAME/mail-out.git
cd mail-out
```

---

## 2. Load the Extension Locally

1. Open `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load unpacked**
4. Select the project folder

The extension should now appear in Chrome.

---

# 🛠 Development Guidelines

## Keep Changes Focused

Please avoid massive unrelated commits.

### Good examples
- Fix spam score bug
- Improve summary rendering
- Optimize Gmail DOM injection

### Bad example
- UI redesign + spam engine rewrite + README edits in one PR

---

## Code Style

### JavaScript
- Use clear variable names
- Prefer small reusable functions
- Avoid deeply nested logic
- Comment non-obvious logic

### UI
- Maintain Gmail-native appearance
- Avoid intrusive UI elements
- Keep overlays lightweight

### AI Prompting
- Keep outputs deterministic
- Avoid increasing token usage unnecessarily
- Preserve strict formatting guarantees

---

# 🧠 AI Constraints

Some outputs are intentionally strict.

## Summaries
- Exactly 3 bullet points
- Concise wording
- Deterministic structure

## Categorization

Must return ONLY one of:

```txt
Work
Personal
Promo
Urgent
Spam
```

Please preserve these constraints unless discussing a major redesign.

---

# 🛡 Spam Detection Contributions

If improving spam detection:

- Explain the heuristic clearly
- Avoid excessive false positives
- Test against legitimate promotional emails
- Keep scoring interpretable

### Example additions
- URL reputation logic
- Improved phishing phrase detection
- Sender anomaly scoring

---

# 🐞 Reporting Bugs

When opening an issue, include:

- Browser version
- Steps to reproduce
- Expected behavior
- Actual behavior
- Screenshots if relevant

---

# ✨ Feature Requests

Feature requests are welcome.

Please include:
- Problem being solved
- Proposed solution
- Possible drawbacks
- Example use case

---

# 🔀 Pull Request Process

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature/your-feature-name
```

3. Commit your changes

```bash
git commit -m "Add: improved phishing detection"
```

4. Push your branch

```bash
git push origin feature/your-feature-name
```

5. Open a Pull Request

---

# ✅ PR Checklist

Before submitting:

- [ ] Extension loads correctly
- [ ] No console errors
- [ ] Existing functionality still works
- [ ] Code is readable
- [ ] README updated if necessary

---

# 📂 Suggested Contribution Areas

- Gmail UI injection improvements
- AI prompt optimization
- Spam heuristics
- Performance optimization
- Accessibility improvements
- Manifest V3 compatibility
- Better onboarding UX
- Settings enhancements

---

# 🤝 Community Standards

Please be respectful and constructive.

By contributing, you agree to follow the project's `CODE_OF_CONDUCT.md`.

---

# ⭐ Final Note

Even small improvements matter.

Thanks for helping make MailOut AI smarter, safer, and cleaner. 🚀