# Decision Maker

A tool that helps you make better decisions. Give it your options and what matters to you, and it helps you compare them and pick one with confidence.

Built for the **Hacktoberfest Hackday x Graphilla** hackathon.

## The Problem

Making choices is hard. We overthink, go back and forth, and lose time weighing options in our heads. Decision Maker gives that process a clear structure so you can decide faster and understand why you chose what you chose.

## Features

- User-Bias / Critical Thinking Features
Bias Detection — identifies when an AI response may be overly agreeable to the user's claim.
Counterargument Generator — automatically provides reasonable opposing viewpoints.
Assumption Checker — highlights assumptions the user is making without evidence.
Fact vs. Opinion — separates objectively verifiable claims from opinions or interpretations.
Confidence Indicator — shows how certain the AI should be about its answer.
Evidence Check — asks whether a claim is actually supported by available evidence.


## Tech Stack

- Frontend: HTML, CSS and JavaScript (`index.html` and `style.css`), no build step
- Backend: none. The page runs in your browser and calls the AI provider directly
- APIs: Google Gemini API and Groq API (free keys, each user brings their own)

## Getting Started

### Prerequisites

- [Git](https://git-scm.com/)
- A modern web browser (Chrome, Firefox, Edge)
- A free API key from Google Gemini or Groq (see "Get an API Key" below)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Hacktoberfest-Hackday-x-Graphilla/decision_maker.git

# 2. Move into the project folder
cd decision_maker
```

There are no dependencies to install.

### Running the project

Open `index.html` in your web browser (double-click the file). Then open **AI settings**, choose a provider, and paste your API key.

## Get an API Key

The app has no server, so each person uses **their own** key. There is no key in this repo.

| Provider | Where to get a free key |
|----------|-------------------------|
| Google Gemini | https://aistudio.google.com/apikey |
| Groq | https://console.groq.com/keys |

Steps:

1. Create a key at one of the links above.
2. Open the app and expand **AI settings**.
3. Pick the same provider in the provider menu ("Google Gemini (free key)" or "Groq (free key)").
4. Paste the key into the **API key** box. Use **Show** to check what you pasted.
5. Run a decision. The status next to "AI settings" changes to "Key saved".

Your key is stored only in your own browser and sent only to the provider you picked.

## Keep Your Key Safe

- Never type your key into the code or commit it to GitHub.
- Do not share your key in screenshots, chats, or pull requests.
- If a key leaks, delete it on the provider's website and create a new one.

## Troubleshooting

- **"Paste your API key in AI settings first"**: the API key box is empty.
- **"Gemini is overloaded right now"**: wait a minute and try again, or switch to Groq in AI settings.
- **HTTP 400, 401 or 403**: the key is wrong, expired, or from a different provider than the one selected.

## How It Works

1. The user describes the decision and lists their options.
2. The user sets the criteria and how much each one matters.
3. The app scores and compares the options.
4. The app shows the best choice and explains why.

## Team

| Name        | Role.               | GitHub          |
|-------------|---------------------|-----------------|
| Sebak Kafle | UI and idea         | aquanovadev-ai  |
| Shivam karna| Documentation and UI| shivamkarna50-ai|
| Birat Poudel| Front end           | tsukii44.       |
| Rajat Tiwari| Documentation.      | aryanrajattiwari|

## Contributing (for teammates)

We follow a simple branch-based workflow so nobody overwrites anyone else's work:

1. Pull the latest code: `git checkout main && git pull`
2. Create your own branch: `git checkout -b yourname/feature-name`
3. Make your changes and commit them: `git add . && git commit -m "Describe your change"`
4. Push your branch: `git push -u origin yourname/feature-name`
5. Open a Pull Request on GitHub and ask a teammate to review and merge it

Please never commit directly to `main`.

## Roadmap

- [ ] Core decision logic
- [ ] User interface
- [ ] Results and explanation screen
- [ ] Demo and presentation

## License

This project is licensed under the GPL-3.0 license. See `LICENSE.txt`.
