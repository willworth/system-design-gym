# Interview Prep Tools

Interactive tools for system design interview preparation. Focus: tradeoffs, not trivia.

## Tools

### `tradeoff-cards.html`
Split-card layout for 7 core tradeoff pairs. Three modes:
- **Study** — full details visible
- **Quiz** — content blurred, click to reveal
- **Scenarios** — real-world prompts, pick the right side

### `whiteboard.html`
Architecture design simulator. Pick a challenge, work through the 5-step answer shape:
1. Clarify requirements
2. Propose architecture
3. Identify bottlenecks
4. Discuss tradeoffs
5. Describe evolution

Features:
- 35-minute countdown with phase markers
- Guided hints (blurred, reveal on click)
- Notes panel for writing your answer
- Diagram canvas for sketching architecture
- Coverage checklist to track what you've addressed
- Session review summary

### `bottleneck-spotter.html`
Interactive architecture diagrams with stress scenarios. Apply a condition (traffic spike, DB failure, cache loss), then click the component that breaks first. Get detailed explanations of why and how failures cascade.

Architectures included:
- Standard Web Application (LB → app → DB + cache)
- Event Processing Pipeline (producers → queue → workers → storage)
- Microservices with API Gateway (gateway → services → DBs + external APIs)

### Challenges included (whiteboard):
- Notification System
- URL Shortener
- Social Feed / Timeline
- Chat / Messaging System
- File Upload & Processing Pipeline
- Search System

## Usage

Just open in a browser:
```
open tradeoff-cards.html
open whiteboard.html
```

No build step. No dependencies. Just HTML.

## Context

Built as part of KAL-1252. Strategy doc: `INTERVIEW-PREP-STRATEGY.md` in Slate.
