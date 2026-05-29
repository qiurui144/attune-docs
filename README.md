# attune-docs

> User-facing documentation for **Attune** — personal knowledge base +
> memory-augmentation system (local-first / privacy / hybrid intelligence).
>
> The product source lives at https://github.com/qiurui144/attune (public).
> This repo holds the **public wiki content**, mounted as a git submodule
> at `external/attune/` inside [wiki-portal](https://github.com/qiurui144/wiki-portal)
> and rendered at the corresponding tenant tab on the Docusaurus site.

## What's here

| Path | Purpose |
|------|---------|
| `wiki/` | The actual docs — Docusaurus-flavoured Markdown |
| `wiki.yaml` | Pattern A.5 tenant manifest (project_id / sidebar / doc_path) |
| `.github/workflows/dispatch.yml` | Triggers wiki-portal rebuild on push to main |

## How to contribute

```bash
git clone https://github.com/qiurui144/attune-docs.git
cd attune-docs
# edit wiki/*.md
git commit -m "docs: <what changed>"
git push origin main
# → dispatch fires → wiki-portal rebuilds within ~3 min
```

Preview locally is **not** required for prose edits; the wiki-portal CI
runs Docusaurus build and surfaces broken links + dead anchors in PR
checks.

## Layout (mirrors wiki-portal sidebar)

- `wiki/index.md` — landing page
- `wiki/quickstart.md` — 5-min setup
- `wiki/wizard.md` — first-run wizard
- `wiki/chat.md` — chat + RAG
- `wiki/llm-setup.md` — LLM provider setup (membership / BYOK / Ollama)
- `wiki/plugins.md` — plugin packs (attune-pro verticals)
- `wiki/agents.md` — agents (memory / chat reliability / self-evolving skill)
- `wiki/sources/` — data sources (local files / WebDAV / email / RSS)
- `wiki/architecture.md` — ASCII data-flow for ingest / search / chat / privacy
- `wiki/benchmarks.md` — performance + accuracy baselines
- `wiki/privacy.md` — vault encryption / cost contract / data isolation
- `wiki/faq.md` — common questions

## License

Documentation under **CC BY 4.0**. See [LICENSE](./LICENSE).

Product code (the Attune repo) is open source; see that repo for its license.

## Project context

- **Product**: Attune — personal knowledge base + memory augmentation
- **Maintainer**: [@qiurui144](https://github.com/qiurui144)
- **Wiki portal**: https://wiki.engi-stack.com/attune/ (after deployment)
- **Issues / typos / suggestions**: this repo's Issues tab
- **Bug reports for the product itself**: report at the [attune repo](https://github.com/qiurui144/attune)
