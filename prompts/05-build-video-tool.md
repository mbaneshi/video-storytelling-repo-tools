# Prompt: Building a Custom Video Demo Tool

## Context

I'm a developer (Rust, Python, TypeScript) who wants to build a CLI or lightweight app that automates hackathon demo video creation. I want to either build from scratch or extend existing open-source tools. I'm on macOS (Apple Silicon) and prefer working with brew-installable tools and CLI workflows.

## Research Questions

1. **Existing tools to build upon**: What open-source projects come closest to automating demo video creation?
   - Anything that takes a script/markdown + recordings and produces video
   - CLI tools for video editing (FFmpeg wrappers, MoviePy alternatives)
   - Programmatic video generation (Remotion, Motion Canvas, Manim, RevealJS + recording)
   - Screen recording libraries with API access

2. **Architecture for a demo-video CLI**:
   - Input: `demo.md` (script with timestamps/sections) + screen recording files
   - Processing: segment matching, voiceover generation, auto-zoom, transitions
   - Output: MP4 ready for submission
   - What's the simplest architecture that delivers value?
   - Rust vs. Python vs. TypeScript for this — tradeoffs?

3. **Key libraries and APIs**:
   - FFmpeg bindings (Rust: `ffmpeg-next`, Python: `ffmpeg-python`)
   - TTS APIs for voiceover (which has the best developer voice?)
   - Whisper for transcript alignment
   - Auto-zoom/cursor tracking — any libraries for this?
   - Subtitle/caption generation

4. **MVP scope**: What's the smallest useful version of this tool?
   - What should v0.1 do?
   - What can wait for v0.2+?
   - How to make it useful for myself within a weekend of building?

5. **Integration with existing workflow**:
   - How to integrate with OBS/Screen Studio recordings?
   - Export formats that work with CapCut/DaVinci for manual touch-ups
   - CI/CD for video? (auto-generate demo on push?)

## What I Want Back

- Architecture diagram for the MVP
- Recommended tech stack with reasoning
- List of key libraries with links
- Step-by-step build plan for a weekend project
- Examples of similar tools that exist
