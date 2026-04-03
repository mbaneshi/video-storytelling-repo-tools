# Prompt: AI-Powered Video Demo Automation

## Context

I'm a developer who frequently participates in hackathons and needs to produce narrated demo videos (2–5 minutes) showcasing software projects. I work on macOS (Apple Silicon). I currently have: OBS, Screen Studio, Loom, CapCut, DaVinci Resolve. I want to automate or semi-automate the video creation pipeline using AI.

## Research Questions

1. **AI narration & voiceover**: What are the best tools/APIs for generating natural developer-style voiceover from a script? (e.g., ElevenLabs, OpenAI TTS, Google Cloud TTS, Coqui). Compare quality, latency, cost, and how natural they sound for technical content.

2. **Auto-editing & assembly**: Are there AI tools that can take raw screen recordings + a script and automatically assemble a polished video? (e.g., Descript, Runway, CapCut AI features, Pictory, Synthesia). Which ones support developer demo style (terminal, code, UI walkthroughs)?

3. **Agentic video pipeline**: Can I build an agentic workflow where:
   - Input: markdown script + raw screen recording(s)
   - Agent: segments the recording, matches segments to script sections, adds transitions, generates voiceover, composites final video
   - Output: ready-to-submit MP4
   - What frameworks/libraries would I use? (FFmpeg, MoviePy, whisper for alignment, TTS APIs)

4. **Cursor/action detection**: Are there tools that can auto-zoom on cursor or detect key UI interactions in a screen recording and add emphasis (zoom, highlight, callout) programmatically?

5. **Existing open-source projects**: Any GitHub repos or open-source tools that already do parts of this pipeline? Especially anything that takes a screenplay/script and automates video assembly.

## What I Want Back

- Comparison tables where possible
- Links to tools, APIs, repos
- Architecture sketch for a minimal agentic pipeline I could build myself
- Realistic assessment of what's automatable today vs. what still needs manual work
