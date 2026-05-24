# CodeBuddy – AI Code Assistant for Beginners

I built this project because I kept struggling to find simple answers to basic coding questions without getting lost in Stack Overflow rabbit holes. So I made my own tool that explains things like I'm 5.

It's a chatbot powered by the Claude API that helps beginners with coding — debugging, explanations, writing simple programs, etc.

> Still working on it. There are probably bugs lol

---

## What it does

- You type a question or paste your broken code
- It gives you an answer in plain English (no fancy jargon)
- You can pick which programming language you're working in
- There's a few quick buttons if you don't know what to ask first

Basically it's like having a patient tutor who doesn't judge you for asking dumb questions.

---

## How to run it

It's just plain HTML/CSS/JS so there's no installation needed.

**1. Clone or download this repo**
```bash
git clone https://github.com/YOUR_USERNAME/ai-code-assistant.git
```

**2. Get a Claude API key**

Go to https://console.anthropic.com, make an account, and grab an API key. They have a free tier.

**3. Paste your key into app.js**

Open `app.js` and find this line near the top:
```js
const API_KEY = "YOUR_API_KEY_HERE";
```
Replace the placeholder with your actual key.

**4. Open index.html in your browser**

That's it. Double click the file or drag it into Chrome/Firefox.

> ⚠️ Don't push your real API key to GitHub. Seriously. I learned that the hard way (not really but I've heard stories).

---

## Project structure

```
ai-code-assistant/
├── index.html     → the main page
├── style.css      → all the styling
├── app.js         → handles the API calls and chat logic
├── CHANGELOG.md   → what I changed and when
└── README.md      → you're reading it
```

---

## Tech used

- HTML, CSS, JavaScript (no frameworks — I wanted to keep it simple)
- Claude API by Anthropic for the AI responses
- Google Fonts (JetBrains Mono + Syne)

---

## Known issues / TODO

- [ ] API key is exposed in frontend — need to build a small backend for this eventually
- [ ] No syntax highlighting yet (tried highlight.js but it was breaking things)
- [ ] Mobile layout is a bit off on very small screens
- [ ] Would be cool to add copy-to-clipboard on code blocks
- [ ] Save chat history so it doesn't reset on refresh

---

## Why I made this

I'm learning web development and wanted to build something actually useful instead of another to-do app. Also wanted to practice working with external APIs for the first time — the fetch requests were confusing at first but I think I get it now.

If this helps even one person learn to code more easily, that's a win for me.

---

## License

MIT — do whatever you want with it, just don't blame me if something breaks 😅
