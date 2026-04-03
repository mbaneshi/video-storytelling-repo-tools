# Prompt: AI Agent Workflow for Video Production

## Context

I'm a developer exploring how AI agents can automate or assist in video production workflows — specifically for short technical demo videos. I want to understand what's possible today with multi-agent systems, LLM tool-use, and existing video APIs. I work with Python, Rust, and TypeScript.

## Research Questions

1. **Agent architecture for video production**: Design a multi-agent system where:
   - **Script Agent**: takes project README + code and generates a narration script
   - **Recording Agent**: orchestrates screen recording (trigger record, navigate UI, execute CLI commands)
   - **Edit Agent**: takes raw footage + script, produces edited video
   - **Review Agent**: watches the output and suggests improvements
   - What LLM capabilities does each agent need? What tools do they call?

2. **Available building blocks**:
   - Computer-use APIs (Claude, OpenAI) — can they drive a demo recording?
   - Video understanding models — can they review a demo video and give feedback?
   - Code-to-video tools — anything that generates video from code/markdown?
   - Screen automation on macOS (AppleScript, Hammerspoon, cliclick, Accessibility API)

3. **Realistic assessment**:
   - What parts of this pipeline work well with current AI (mid-2025)?
   - What parts are too unreliable to automate?
   - Where does human-in-the-loop make sense?
   - Cost estimate for generating one 3-minute video with AI assistance

4. **Framework choices**:
   - Claude Agent SDK vs. LangGraph vs. CrewAI vs. custom orchestration
   - For video-specific tasks, which framework gives best tool integration?
   - How to handle long-running video processing tasks in an agent loop?

5. **Practical next steps**:
   - What's the simplest agent I can build today that provides real value?
   - Example: an agent that watches my screen recording, generates a script, and creates subtitles
   - Minimal code to get started

## What I Want Back

- Multi-agent architecture diagram
- Assessment of what's realistic vs. aspirational
- Code skeleton or pseudocode for the simplest useful agent
- Comparison of agent frameworks for this use case
- Links to relevant APIs, models, and tools
