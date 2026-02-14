# Changelog

## 1.0.0
Initial release.

### Translate Anywhere
- Menu bar app + global shortcuts for instant translations.
- QuickBar (Spotlight-style) and a dedicated result dialog.
- Output modes: show dialog, paste directly, or clipboard-only.
- Auto language detection, direction cycling, tones, duel mode, diff view, and history.
- Streaming mode, cancellation, and a disk-backed translation cache (LRU + TTL).

### Ask AI & AI Search
- Selection Bar appears next to selected text with: Translate, Replace, Ask AI, Explain, Summarize, AI Search.
- AI Search aggregates web/news/video/image results with streaming summaries and citations, plus a built-in YouTube preview.
- Dedicated provider routing for AI Search (separate from the main translation provider).
- Unified Image Search fallback chain: Brave Pro -> Brave Free -> DataForSEO (Google Images) -> Pexels.

### Providers (Local + Cloud)
- Local engines: Ollama and LM Studio (headless server control + model management).
- Cloud providers: OpenAI, Anthropic, Gemini, xAI, OpenRouter, Perplexity.

### OCR & Rich Rendering
- Screen-to-Translate OCR (Cmd+Shift+X) with improved capture accuracy and paragraph reflow.
- Rich Markdown rendering with syntax highlighting and one-click code copy.

### Integrations
- PopClip extension + URL scheme actions (`localtranslator://translate`, `localtranslator://ai-search`) for external workflows.
