# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Content Creation System

## System Overview
This workspace transforms ideas into multi-format content:
1. Raw notes → Theme extraction → Research → Long-form article → Platform-specific versions
2. All brand/voice guidelines live in @context/
3. Agents handle platform optimization

## Workflow Commands
- `/extract-themes` - Analyze raw notes in /rawnotes to identify patterns and content opportunities
- `/research [topic]` - Develop and refine ideas from themes or new topics
- `/write` - Create comprehensive article
- Auto-generates: LinkedIn, Newsletter, Twitter/X, Podcast Q&A

## Context Architecture
Always reference these for consistency:
- @context/writing-examples.md - Real examples across platforms that demonstrate voice and style
- @context/research-sources.md - Priority newsletters and sources to check first during research

## Agent Specializations
- `linkedin-repurposer`: Professional networking optimization
- `newsletter-repurposer`: Email engagement specialist  
- `conversational-repurposer`: Social media posts and podcast Q&A scripts

## Working From Rough Notes
When the user shares rough notes, voice-note transcripts or background stories:
1. Do not build anything yet. First turn the notes into a short structured brief (goal, audience, output format, scope, key content) and ask clarifying questions.
2. Treat background stories (where an idea came from, who inspired it, conversations with other people) as private context. Never put them in the deliverable unless the user explicitly asks.
3. Build only after the user confirms the brief.

## Development Guidelines
- Never duplicate context information - always reference source files
- Maintain consistency across all generated formats
- Each agent should specialize in their platform's unique requirements
- Content quality gates should validate against brand guidelines before output