# Video Storytelling Repo Tools

Recording tools, workflows, and storytelling frameworks for creating hackathon demo videos on Mac.

## Recording & Editing Tools

### Install via Homebrew

```bash
# Screen recording
brew install --cask obs                # Free, powerful, scene-based recording
brew install --cask screen-studio      # Auto-zoom, polished demo style
brew install --cask loom               # Screen + mic + webcam, cloud upload

# Video editing
brew install --cask capcut             # Free editor, good templates & effects
```

### Manual Install (no brew cask available)

| Tool | Install | Notes |
|------|---------|-------|
| **DaVinci Resolve** | [Download](https://www.blackmagicdesign.com/products/davinciresolve) | Pro-grade editor, free version is very capable |

### macOS Built-in (no install needed)

**Shift + Cmd + 5** — screen recorder with mic support. Zero setup, good enough for quick demos.

## Tool Comparison

| Tool | Best For | Webcam | Cloud | Editing | Cost |
|------|----------|--------|-------|---------|------|
| macOS built-in | Quick capture, no install | No | No | None | Free |
| OBS | Complex scenes, streaming | Yes | No | None (record only) | Free |
| Screen Studio | Polished dev demos | Yes | No | Auto-zoom, minimal | Paid |
| Loom | Fast narrated walkthroughs | Yes | Yes | Trim only | Freemium |
| CapCut | Post-production editing | N/A | Yes | Full editor | Free |
| DaVinci Resolve | Pro editing, color grading | N/A | No | Full editor | Free/Paid |

## Recommended Workflow

1. **Record** with Screen Studio (polished) or OBS (free) or macOS built-in (zero setup)
2. **Edit** in CapCut (quick) or DaVinci Resolve (pro)
3. **Export** as MP4, 1080p, H.264

---

## Storytelling Framework

Use a **Problem → Solution → Impact** structure. Two templates below.

### 2-Minute Template (Hackathon Standard)

| Section | Time | What to Say/Show |
|---------|------|------------------|
| **Hook** | 0:00–0:15 | One sentence: who you help + the painful problem. Show the "before" state. |
| **Solution demo** | 0:15–1:15 | Live walkthrough. Show 2–3 key moments only. Narrate with "you" language. |
| **Architecture** | 1:15–1:35 | Quick diagram or terminal tree. Name key tech choices. |
| **Results & close** | 1:35–2:00 | Concrete outcome (time saved, perf). One sentence future vision. |

**Script skeleton:**

> "If you've ever [painful thing], you know [why it hurts].
> We built [tool name] — here's how it works.
> [Demo: show the 2–3 critical steps]
> Under the hood, we use [tech A] for [reason] and [tech B] for [reason].
> The result: [concrete metric]. Next, we're adding [future feature]."

### 5-Minute Template (Deep Dive)

| Section | Time | What to Say/Show |
|---------|------|------------------|
| **Hook** | 0:00–0:20 | Problem statement with a real scenario or stat. |
| **User story** | 0:20–1:00 | Walk through a typical user's pain point before your tool. |
| **Core demo** | 1:00–3:00 | Full walkthrough from start to result. Show real data/output. |
| **Architecture** | 3:00–4:00 | Diagram, code structure, key design decisions. Why these choices matter. |
| **Results & vision** | 4:00–4:40 | Metrics, benchmarks, user feedback. |
| **Close** | 4:40–5:00 | Future roadmap. Call to action. |

### Narration Tips

- **Start recording, then wait 3 seconds** before speaking (gives clean trim point)
- **Use "you" language**: "You click here" not "I click here"
- **One take per section** — stitch in editor, don't try to nail it all at once
- **Show, don't tell**: if you can demonstrate it on screen, don't just describe it
- **Slow your cursor**: move deliberately, pause on key UI elements
- **Audio matters more than video**: use a decent mic or AirPods, record in a quiet room

### Demo Recording Checklist

- [ ] Close notifications (Focus mode on)
- [ ] Clean desktop, hide dock
- [ ] Increase font size in terminal/editor
- [ ] Prepare sample data / demo scenario
- [ ] Write bullet-point script per section
- [ ] Test mic audio level
- [ ] Do one dry run before recording

---

## Research Prompts

Ready-to-use prompts for cross-AI research (paste into Gemini, Perplexity, Claude, ChatGPT):

| # | Prompt | Focus Area |
|---|--------|------------|
| 01 | [AI Video Automation](prompts/01-ai-video-automation.md) | AI tools for automating video pipeline — TTS, auto-editing, agentic workflows |
| 02 | [Storytelling Frameworks](prompts/02-storytelling-frameworks.md) | Narrative structures for technical demos — frameworks, pacing, script templates |
| 03 | [Content Creation Strategy](prompts/03-content-creation-strategy.md) | Repurposing, platform strategy, sustainable content workflow for devs |
| 04 | [Personal Branding](prompts/04-personal-branding-devs.md) | Developer brand building — archetypes, portfolio, hackathon presence |
| 05 | [Build a Video Tool](prompts/05-build-video-tool.md) | Architecture for a custom CLI/app that automates demo video creation |
| 06 | [AI Agent Video Workflow](prompts/06-ai-agent-video-workflow.md) | Multi-agent system design for video production — frameworks, feasibility |

### How to Use

1. Copy the full content of a prompt file
2. Paste into your AI tool of choice
3. Compare responses across Gemini, Perplexity, Claude, ChatGPT
4. Collect findings back into this repo under `research/`

## License

MIT
