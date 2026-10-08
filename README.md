# Decision Maker

A tool that helps you make better decisions. Give it your options and what matters to you, and it helps you compare them and pick one with confidence.

Built for the **Hacktoberfest Hackday x Graphilla** hackathon.

## The Problem

Making choices is hard. We overthink, go back and forth, and lose time weighing options in our heads. Decision Maker gives that process a clear structure so you can decide faster and understand why you chose what you chose.

## Features

- Enter the decision you are trying to make
- Add multiple options to compare
- Define the criteria that matter and how important each one is
- Get a clear recommendation with the reasoning behind it
- Choose between two AI providers: Google Gemini or Groq

> This list will grow as the project does. Update it as features are completed.

## Tech Stack

- Frontend: HTML, CSS and JavaScript in a single file (`decision maker.html`), no install or build step
- Backend: none. The page runs in your browser and calls the AI provider directly
- APIs: Google Gemini API and Groq API (you bring your own free API key)

## Getting Started

### Prerequisites

- [Git](https://git-scm.com/)
- A modern web browser (Chrome, Firefox, Edge)
- A free API key from Gemini or Groq (see "Get an API Key" below)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Hacktoberfest-Hackday-x-Graphilla/decision_maker.git

# 2. Move into the project folder
cd decision_maker
```

No dependencies to install.

### Running the project

Open `decision maker.html` in your browser (double-click the file). Then paste your API key into the "API key" box (see below) and start deciding.

## Get an API Key

This app has no server, so each person uses **their own** API key. There is no key in this repo.

| Provider | Where to get a free key |
|----------|-------------------------|
| Google Gemini | https://aistudio.google.com/apikey |
| Groq | https://console.groq.com/keys |

Steps:

1. Sign in at one of the links above and create a key.
2. Open the app and choose the same provider in the provider menu.
3. Paste the key into the "API key" box.
4. Add your options and criteria and run the decision.

The key is sent only to the provider you picked.

## Keep Your Key Safe

- Never type your key into the code or commit it to GitHub.
- Do not share your key in screenshots, chats, or pull requests.
- If a key leaks, delete it on the provider's website and create a new one.

## Troubleshooting

- **"Paste your API key first"**: the key box is empty.
- **"Gemini is overloaded right now"**: wait a minute and try again, or switch to Groq in settings.
- **HTTP 401 or 403**: the key is wrong, expired, or from a different provider than the one selected.

## How It Works

1. The user describes the decision and lists their options.
2. The user sets the criteria and how much each one matters.
3. The app sends this to the AI model, which scores each option against each criterion.
4. The app shows the best choice and explains why.

## Team

| Name | Role | GitHub |
|------|------|--------|
| Member 1 | | |
| Member 2 | | |
| Member 3 | | |
| Member 4 | | |

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

Add a license here if you choose one (MIT is a common choice for hackathons).
