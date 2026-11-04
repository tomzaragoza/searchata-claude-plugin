# Searchata for Claude

Searchata connects Claude to search reports, website diagnostics, and SEO workflows. This repository contains the plugin distribution only.

Version 0.1.0 is a release candidate. It passes package validation. Claude account testing and directory review are still pending.

## Install in Claude Code

```text
/plugin install searchata --marketplace tomzaragoza/searchata-claude-plugin
```

Open `/mcp` and authorize Searchata in your browser. For local testing, run `claude --plugin-dir ./plugins/searchata`.

The plugin adds setup, performance, roadmap, and improve-page workflows. Read the [plugin guide](plugins/searchata/README.md) for requirements, examples, privacy information, and limits. Searchata service access and Claude access are separate.

## Validate

```sh
claude plugin validate .
claude plugin validate plugins/searchata
```

The GitHub workflow also runs these checks with Claude Code 2.1.318. Package validation does not replace live testing or directory review.

## Support

Visit [Searchata support](https://searchata.com/support) or email [support@searchata.com](mailto:support@searchata.com). The plugin files use the [MIT License](plugins/searchata/LICENSE).
