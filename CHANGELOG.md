# Changelog

## Unreleased — Local Acceptance

- Add current, searchable text-model catalogs with explicit provider refresh, offline suggestions, preserved saved IDs, and manual model/deployment entry.
- Add DeepSeek direct, Azure text, and multiple named OpenAI-compatible connections with independent translation/search/comparison assignments and Keychain credentials.
- Update native request policies, OpenAI search routing, Perplexity Agent presets/citations, OpenRouter supported parameters, and compatible Gemini 3.8 TTS.
- Add a per-model Reasoning setting that lists only the levels each model documents and shows the exact request fields it sends; QuickBar's Thinking button now raises reasoning for chat only on every supported model.
- Test a custom model ID with one short request before saving it, show the provider's error when it fails, and allow saved custom IDs to be removed. Custom IDs no longer disappear when the API key or sampling settings change.
- Show DeepSeek's API aliases with their model generation (`deepseek-flash` is DeepSeek V4.1 Flash).
- Add Inception (Mercury) as a direct provider: Mercury 2.5 and Mercury 2 come from Inception's model list, translations use the documented `instant` reasoning level, and Reasoning also offers Low, Medium and High.
- Match the translation dialog's model selector to the provider chip beside it, and widen the Settings provider pickers so longer provider names are not cut off.
- Add General → Startup → Open Settings at Launch (on by default). Onboarding and missing-permission screens still open at launch when needed.
- Fix the menu bar's Settings… command (⌘,) opening an empty window instead of Settings, and the menu bar icon not closing its panel while Settings was open.
- Reject incomplete/error Chat Completions and Responses streams instead of treating partial output as a completed answer; keep reasoning out of displayed translations and retain citation source numbers.
- Add Azure Live Translation with lightweight A/B captions and a resizable C meeting workspace, independent original/translation lanes, paused scroll following, local SQLite history, and complete copy/export.
- Keep text-provider settings separate from Live Translation; no automatic recording, deployment, model-list inference probes, or billing eligibility promises.

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
