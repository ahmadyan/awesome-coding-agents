# Awesome Coding Agents [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of terminal coding agents and agent harnesses, with the maker, license, and install command for each.

Every entry is an agent you can run against your own checkout from a terminal. Sections group agents by who builds them, entries are alphabetical within each section, and install commands follow each project's own documentation. Read an install script before you pipe it into a shell.

## Contents

- [Model-lab agents](#model-lab-agents)
- [Open-source agents](#open-source-agents)
- [General-purpose agents](#general-purpose-agents)
- [Editor and tool-vendor agents](#editor-and-tool-vendor-agents)
- [Review agents](#review-agents)
- [Cloud and background agents](#cloud-and-background-agents)
- [Run several at once](#run-several-at-once)
- [Related lists](#related-lists)

## Model-lab agents

Agents from companies that also train the models behind them.

- [Antigravity CLI](https://antigravity.google/docs/cli/overview) - Google's terminal-first client for its Antigravity agent platform, with subagents, artifacts, and code search. Proprietary. Install: `curl -fsSL https://antigravity.google/cli/install.sh | bash`.
- [Claude Code](https://code.claude.com/docs/en/overview) - Anthropic's agentic coding tool for the terminal, extensible with subagents, hooks, skills, plugins, and MCP servers. Proprietary. Install: `curl -fsSL https://claude.ai/install.sh | bash`.
- [Codex CLI](https://github.com/openai/codex) - OpenAI's local coding agent, written in Rust, with sandboxed command execution, built-in code review, and a non-interactive `codex exec` mode. Open source (Apache-2.0). Install: `npm install -g @openai/codex`.
- [Gemini CLI](https://github.com/google-gemini/gemini-cli) - Google's terminal agent for Gemini models, with Google Search grounding and MCP support. Open source (Apache-2.0). Install: `npm install -g @google/gemini-cli`.
- [Grok Build](https://docs.x.ai/build/overview) - Terminal coding agent from SpaceXAI, the maker of Grok, with plan mode, subagents, worktrees, hooks, and a headless mode for scripts. Proprietary. Install: `curl -fsSL https://x.ai/cli/install.sh | bash`.
- [Kimi Code CLI](https://github.com/MoonshotAI/kimi-code) - Moonshot AI's single-binary terminal agent, tuned for Kimi models and configurable for other compatible providers. It replaces the archived Python `kimi-cli`. Open source (MIT). Install: `curl -fsSL https://code.kimi.com/kimi-code/install.sh | bash`.
- [MiMo Code](https://github.com/XiaomiMiMo/MiMo-Code) - Xiaomi's terminal coding assistant with persistent project memory, Git management, and streaming voice input. Open source (MIT). Install: `curl -fsSL https://mimo.xiaomi.com/install | bash`.
- [Mistral Vibe](https://github.com/mistralai/mistral-vibe) - Mistral AI's lightweight terminal coding assistant, extensible with skills and custom slash commands. Open source (Apache-2.0). Install: `curl -LsSf https://mistral.ai/vibe/install.sh | bash`.
- [Muse Code](https://dev.meta.ai/docs/muse-code) - Meta's agent for its Muse Spark model, usable in a terminal or a CI job, with sandboxing, approval policies, resumable sessions, and multi-agent runs. Proprietary. Install: `curl -fsSL https://dev.meta.ai/install.sh | bash`.
- [Poolside Agent CLI](https://docs.poolside.ai/cli/pool) - Poolside's `pool` command for interactive sessions, one-shot `pool exec` automation, and serving its agent to ACP-compatible editors. Proprietary. Install: `curl -fsSL https://downloads.poolside.ai/pool/install.sh | sh`.
- [Prime Agent](https://github.com/PrimeIntellect-ai/prime-agent) - Prime Intellect's coding and research agent built on recursive language models, with recursive subagents and a harness that keeps memories and skills between long-running tasks. Open source (MIT). Install: `curl -fsSL https://app.primeintellect.ai/prime-agent/install.sh | sh`.
- [Qwen Code](https://github.com/QwenLM/qwen-code) - Alibaba's agent for Qwen models, with subagents and automatic memory, plus IDE, desktop, and chat-app editions alongside the terminal. Open source (Apache-2.0). Install: `npm install -g @qwen-code/qwen-code`.

## Open-source agents

Provider-flexible harnesses whose source you can read, fork, and run with your own model keys.

- [Aider](https://github.com/Aider-AI/aider) - Pair-programming agent from Aider AI that builds a map of your repository, edits code in many languages, and commits each change to Git. Open source (Apache-2.0). Install: `curl -LsSf https://aider.chat/install.sh | sh`.
- [Ante](https://github.com/AntigmaLabs/ante) - Antigma Labs' self-contained agent, shipped as a single Rust binary that runs with hosted models or fully offline local ones. Open source (Apache-2.0). Install: `curl -fsSL https://ante.run/install.sh | bash`.
- [Autohand Code](https://github.com/autohandai/code-cli) - Autohand AI's terminal agent with skills, approval prompts for risky operations, provider switching, and a CI mode. Open source (Apache-2.0). Install: `curl -fsSL https://autohand.ai/install.sh | bash`.
- [Cline CLI](https://github.com/cline/cline) - Cline's agent in the terminal, with the same plan and act modes and approval controls as its IDE extension. Open source (Apache-2.0). Install: `npm install -g cline`.
- [Code Puppy](https://github.com/mpfaffenberger/code_puppy) - Mike Pfaffenberger's Python agent, built on Pydantic AI, that works with many model providers from the terminal. Open source (MIT). Install: `uvx code-puppy`.
- [Codebuff](https://www.codebuff.com) - Multi-agent terminal coding tool with paid plans, whose orchestration framework and SDK are published in the Freebuff repository. Open source (Apache-2.0). Install: `npm install -g codebuff`.
- [Crush](https://github.com/charmbracelet/crush) - Charmbracelet's terminal agent with mid-session model switching, LSP-powered context, and MCP extensions. Source-available (FSL-1.1-MIT). Install: `npm install -g @charmland/crush`.
- [Every Code](https://github.com/just-every/code) - Just Every's community fork of OpenAI's Codex CLI that adds browser integration, multi-agent commands, and theming while staying compatible with upstream. Open source (Apache-2.0). Install: `npm install -g @just-every/code`.
- [ForgeCode](https://github.com/tailcallhq/forgecode) - Tailcall's terminal development environment that puts one agent interface in front of 300+ models. Open source (Apache-2.0). Install: `curl -fsSL https://forgecode.dev/cli | sh`.
- [Freebuff](https://github.com/CodebuffAI/freebuff) - Free, ad-supported sibling of Codebuff, with a terminal CLI and desktop, web, and cloud editions. Open source (Apache-2.0). Install: `npm install -g freebuff`.
- [fx](https://github.com/vercel-labs/fx) - Vercel Labs' small coding agent written in Zig, with a shell-like interface, a one-shot `fx ask` command, and an embeddable library. Open source (Apache-2.0). Install: `curl -fsSL https://fx.sh/setup.sh | bash`.
- [Goose](https://github.com/aaif-goose/goose) - Extensible agent with a CLI, desktop app, and API, started at Block and now part of the Agentic AI Foundation at the Linux Foundation. Open source (Apache-2.0). Install: `curl -fsSL https://github.com/aaif-goose/goose/releases/download/stable/download_cli.sh | bash`.
- [Jcode](https://github.com/1jehuang/jcode) - Jeremy Huang's Rust coding-agent harness focused on low memory use, with durable memory, background tasks, and agent swarms. Open source (MIT). Install: `curl -fsSL https://jcode.sh/install | bash`.
- [Kilo CLI](https://github.com/Kilo-Org/kilocode) - Terminal edition of Kilo Code, the agent that also runs inside VS Code and JetBrains IDEs. Open source (MIT). Install: `npm install -g @kilocode/cli`.
- [Letta Code](https://github.com/letta-ai/letta-code) - Memory-first harness from Letta whose agents keep and rewrite their own memory, skills, and prompts across sessions. Open source (Apache-2.0). Install: `npm install -g @letta-ai/letta-code`.
- [mini-SWE-agent](https://github.com/SWE-agent/mini-swe-agent) - Deliberately tiny agent from the SWE-agent team that acts only through bash, useful for experiments and for learning how agents work. Open source (MIT). Install: `uv tool install mini-swe-agent`.
- [Nanocoder](https://github.com/Nano-Collective/nanocoder) - The Nano Collective's community-built terminal agent that runs on local models through Ollama or on any OpenAI-compatible API. Open source (MIT). Install: `npm install -g @nanocollective/nanocoder`.
- [Octofriend](https://github.com/synthetic-lab/octofriend) - Synthetic Lab's small, zero-telemetry assistant that can switch models mid-conversation and optionally use custom-trained helper models. Open source (MIT). Install: `npm install --global octofriend`.
- [Oh My Pi](https://github.com/can1357/oh-my-pi) - Stencil Labs' fork of Pi that adds subagents, plan mode, LSP and debugger integration, and a native Rust core. Open source (MIT). Install: `curl -fsSL https://omp.sh/install | sh`.
- [Open Interpreter](https://github.com/openinterpreter/openinterpreter) - Coding agent from the Open Interpreter team, tuned for low-cost and open-weight models. Open source (Apache-2.0). Install: `curl -fsSL https://www.openinterpreter.com/install | sh`.
- [OpenCode](https://github.com/anomalyco/opencode) - Provider-agnostic agent from Anomaly with a terminal UI and a beta desktop app. Open source (MIT). Install: `curl -fsSL https://opencode.ai/install | bash`.
- [Pi](https://github.com/earendil-works/pi) - Minimal agent from Earendil Works that leaves out subagents and plan mode and lets extensions and packages add what you need. Open source (MIT). Install: `curl -fsSL https://pi.dev/install.sh | sh`.
- [YOLOP](https://github.com/everruns/yolop) - Everruns' Rust terminal agent that runs routine workspace actions without per-tool prompts and reserves approvals for the shell boundary. Open source (MIT). Install: `brew install everruns/tap/yolop`.
- [Zero](https://github.com/Twigpine/zero) - Go terminal agent from Twigpine (formerly Gitlawb) with 25+ model providers, a sandbox and permission policy, and a scriptable `zero exec` mode. Open source (MIT). Install: `npm install -g @gitlawb/zero`.

## General-purpose agents

Agents built for everyday tasks that also take on coding work.

- [gptme](https://github.com/gptme/gptme) - Terminal agent with shell, code-execution, file, and browser tools for programming and other tasks. Open source (MIT). Install: `pipx install gptme`.
- [Hermes Agent](https://github.com/NousResearch/hermes-agent) - Nous Research's self-improving agent that writes its own skills and memory, reachable from a terminal UI or from Telegram, Discord, Slack, and other chat apps. Open source (MIT). Install: `curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash`.
- [OpenClaw](https://github.com/openclaw/openclaw) - Self-hosted personal agent that answers on the chat apps you already use and includes a local terminal UI. Open source (MIT). Install: `curl -fsSL https://openclaw.ai/install.sh | bash`.

## Editor and tool-vendor agents

Agents from companies whose main product is an editor, IDE, terminal, or developer platform.

- [Agentastic](https://www.agentastic.dev/docs/features/agentastic-agent) - The coding agent made by Agentastic.dev; the macOS app downloads it on first launch, and it also installs as a standalone CLI on macOS and Linux. Proprietary. Install: `brew install agentasticai/tap/agentastic`.
- [Amp](https://ampcode.com/docs/cli) - Multi-model agent with a CLI, macOS and iOS apps, and remote machines that keep threads running; it began at Sourcegraph. Proprietary. Install: `npm install -g @ampcode/cli`.
- [Auggie](https://docs.augmentcode.com/cli/overview) - Augment Code's terminal agent, backed by the same codebase context engine as its IDE extensions. Proprietary. Install: `npm install -g @augmentcode/auggie`.
- [CoCo CLI (Cortex Code)](https://docs.snowflake.com/en/user-guide/cortex-code/cortex-code-cli) - Snowflake's terminal agent for data engineering and application work against a Snowflake account; the executable is `cortex`. Proprietary. Install: `curl -LsS https://ai.snowflake.com/static/cc-scripts/install.sh | sh`.
- [CodeBuddy Code](https://www.codebuddy.ai/docs/cli/overview) - Tencent's terminal coding agent, part of the CodeBuddy family that also includes an IDE. Proprietary. Install: `npm install -g @tencent-ai/codebuddy-code`.
- [Command Code](https://commandcode.ai/docs) - Langbase's agent geared toward open-weight models, with tool-call repair and a model that learns your coding preferences. Proprietary. Install: `npm install -g command-code`.
- [Cursor CLI](https://cursor.com/docs/cli/overview) - Anysphere's `agent` command, which runs Cursor's agent in any terminal, script, or GitHub Actions job. Proprietary. Install: `curl https://cursor.com/install -fsS | bash`.
- [Devin CLI](https://docs.devin.ai/cli) - Cognition's local command-line agent, connected to Devin's cloud sessions. Proprietary. Install: `curl -fsSL https://cli.devin.ai/install.sh | bash`.
- [Droid](https://docs.factory.com/droid-cli/overview) - Factory's terminal agent, with adjustable autonomy levels and a headless `droid exec` mode for scripts and CI. Proprietary. Install: `curl -fsSL https://app.factory.ai/cli | sh`.
- [GitHub Copilot CLI](https://github.com/github/copilot-cli) - GitHub's terminal agent, with built-in access to your repositories, issues, and pull requests and support for several model families. Proprietary. Install: `npm install -g @github/copilot`.
- [Junie CLI](https://junie.jetbrains.com/docs/junie-cli.html) - JetBrains' model-agnostic agent for terminals and CI pipelines, a companion to its IDE plugin. Proprietary. Install: `curl -fsSL https://junie.jetbrains.com/install.sh | bash`.
- [Kiro CLI](https://kiro.dev/cli/) - AWS's terminal companion to the Kiro IDE and the successor to the Amazon Q Developer CLI. Proprietary. Install: `curl -fsSL https://cli.kiro.dev/install | bash`.
- [Qoder CLI](https://docs.qoder.com/cli/overview) - Qoder's terminal agent, which asks for permission before sensitive operations, from the makers of the Qoder IDE. Proprietary. Install: `curl -fsSL https://qoder.com/install | bash`.
- [Rovo Dev CLI](https://support.atlassian.com/rovo/docs/use-rovo-dev-cli/) - Atlassian's development agent, run through the Atlassian CLI and able to act on Jira work items and Confluence pages. Proprietary. Install: `brew install atlassian/acli/acli`.
- [Warp Agent CLI](https://docs.warp.dev/agents/cli/) - Standalone `warp` command that runs Warp's agent in any terminal, with inline approvals and handoff to cloud agents. Open source (AGPL-3.0). Install: `curl -fsSL https://app.warp.dev/download/agent-cli | bash`.

## Review agents

Agents that review a diff instead of writing one.

- [CodeRabbit CLI](https://docs.coderabbit.ai/cli/) - CodeRabbit's reviewer for uncommitted and branch changes, usable by a person or by another coding agent before a pull request exists. Proprietary. Install: `curl -fsSL https://cli.coderabbit.ai/install.sh | sh`.
- [Greptile CLI](https://www.greptile.com/cli) - Runs Greptile's repository-aware review against a local branch before you open a pull request. Proprietary. Install: `curl -fsSL https://greptile.com/cli/install | bash`.
- [PR-Agent](https://github.com/The-PR-Agent/pr-agent) - Community-maintained pull-request reviewer, originally from Qodo, that runs from the command line, CI, or a webhook with your own model keys. Open source (MIT). Install: `pip install pr-agent`.

## Cloud and background agents

Command-line clients for agents that run on someone else's machines.

- [GitHub CLI agent-task](https://cli.github.com/manual/gh_agent-task) - Preview `gh agent-task` commands that start, list, and follow Copilot cloud agent tasks from the terminal. The CLI is open source (MIT); the agent is a proprietary service. Install: `brew install gh`.
- [Jules Tools](https://jules.google/docs/cli/reference/) - Command-line client for Jules, Google's asynchronous coding agent that works on GitHub repositories in cloud virtual machines. Proprietary. Install: `npm install -g @google/jules`.
- [Orbi](https://github.com/orbi-build/orbi) - Self-hosted autonomous coding agent that turns labeled GitHub Issues into reviewed pull requests; also available as a managed cloud at [orbi.build](https://orbi.build/?ref=gh-ahmadyan-aca). Open source (AGPL-3.0). Install: `docker run orbi/orbi` or the installer in the repo README.

## Run several at once

Most of these agents assume one task per checkout. These resources cover running several side by side.

- [Agentastic agent directory](https://www.agentastic.dev/agents) - Lists which of the agents above Agentastic.dev, a proprietary macOS multi-agent IDE, can launch side by side in isolated Git worktrees.
- [Awesome Agentic IDEs: multi-agent IDEs](https://github.com/ahmadyan/awesome-agentic-ides#multi-agent-ides-and-ades) - Desktop apps, terminals, and orchestrators that run many of these agents in parallel, each in its own branch or worktree.

## Related lists

- [Awesome Agentic IDEs](https://github.com/ahmadyan/awesome-agentic-ides) - Agentic IDEs, multi-agent development environments, agent terminals, and remote-control apps.
- [Awesome Personal Agents](https://github.com/ahmadyan/awesome-personal-agents) - Always-on personal agents, memory layers, runtimes, and messaging bridges.
- [Awesome Software Factory](https://github.com/ahmadyan/awesome-software-factory) - Tools, patterns, and essays for taking work from issue to merged pull request with coding agents.

## Contributing

Contributions are welcome. Read the [contribution guidelines](CONTRIBUTING.md) first.

---

Maintained by [Adel Ahmadyan](https://github.com/ahmadyan), who builds [Agentastic.dev](https://www.agentastic.dev).
