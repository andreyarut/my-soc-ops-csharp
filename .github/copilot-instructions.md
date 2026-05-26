# Soc Ops — Agent Instructions

## Mandatory Dev Checklist

Before every commit, all steps must pass:

- [ ] **Lint** — no unused `using` directives or dead variables
- [ ] **Build** — `dotnet build SocOps/SocOps.csproj` with zero errors or warnings
- [ ] **Test** — `dotnet test` passes (when tests exist)

## Project

Blazor WebAssembly (.NET 10) social bingo game. Players mark squares matching icebreaker questions; first to 5 in a row wins.

## Architecture

| Path | Purpose |
|------|---------|
| `Components/` | UI — board, square, modal, game/start screens |
| `Services/BingoGameService.cs` | State management + localStorage persistence |
| `Services/BingoLogicService.cs` | Board generation, win detection, square toggling |
| `Data/Questions.cs` | Question pool — add/edit questions here |
| `Pages/Home.razor` | Root routable page |
| `wwwroot/css/app.css` | Custom utility classes (Tailwind-like) |

## Conventions

- PascalCase public / `_camelCase` private; nullable enabled
- Call `NotifyStateChanged()` after every state mutation in `BingoGameService`; never mutate from components
- `_ = SaveGameStateAsync()` fire-and-forget is intentional
- Styling: utility classes from `app.css` only — no inline styles, no Tailwind, no Bootstrap
- New components must be added to `_Imports.razor`
- New questions use lowercase strings matching existing format in `Questions.cs`

## Commands

```bash
dotnet build SocOps/SocOps.csproj         # Build
dotnet run --project SocOps/SocOps.csproj # Dev server → http://localhost:5166
```
