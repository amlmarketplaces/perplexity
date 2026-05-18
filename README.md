# amlmarketplaces/perplexity

Claude Code marketplace federating all `@amlplugins/perplexity-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-perplexity": {
      "source": { "source": "github", "repo": "amlmarketplaces/perplexity" }
    }
  },
  "enabledPlugins": {
      "perplexity-search@aml-perplexity": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/perplexity`, cached under `~/.claude/plugins/cache/aml-perplexity/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (1 total)

- `perplexity-search` — [@amlplugins/perplexity-search](https://github.com/amlplugins/perplexity-search)

## Related

- npm packages: `@amlplugins/perplexity-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
