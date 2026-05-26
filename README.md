🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

Turn awkward small talk into a game.

Soc Ops is a fast, social bingo app for in-person mixers, workshops, and team events. Players find people who match the prompts, mark their board, and race to 5 in a row.

[Play Live Demo](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) | [Read the Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)

---

## Why Soc Ops?

- Breaks the ice in minutes with easy conversation starters
- Works great for onboarding, hackathons, and conference meetups
- Simple rules: match a prompt, mark a square, get bingo
- Built with Blazor WebAssembly and ready for GitHub Pages deployment

## Project At A Glance

- Framework: Blazor WebAssembly (.NET 10)
- App path: `SocOps/`
- Prompt data: `SocOps/Data/Questions.cs`
- Game logic: `SocOps/Services/BingoLogicService.cs`
- State + persistence: `SocOps/Services/BingoGameService.cs`

## Quick Start

### Prerequisite

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

### Run locally

```bash
cd SocOps
dotnet run
```

### Build

```bash
cd SocOps
dotnet build
```

The app deploys automatically to GitHub Pages when changes are pushed to `main`.

## Workshop Track

Use this repository as an agent-focused workshop with step-by-step labs:

| Part | Topic |
|------|-------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview and Checklist |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup and Context Engineering |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Build a Quiz Master Agent |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development |
| [**05**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=05-complete) | Complete Experience |

Offline versions are available in `workshop/`, including localized guides in `workshop/es/` and `workshop/pt_BR/`.

## Open In Codespaces (Optional)

After creating your own repo from this template:

1. Open your repo on GitHub.
2. Select **Code** > **Codespaces** > **Create codespace on main**.
3. Wait for the devcontainer setup to complete.
4. From the repository root, run:

```bash
cd SocOps
dotnet run
```
