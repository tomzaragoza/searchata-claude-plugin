# Searchata for Claude

Use your Searchata data to analyze search performance, find SEO priorities, and prepare page improvements. SEO means search engine optimization. This plugin connects to Searchata and adds four workflows for Claude.

## Requirements

Create a [Searchata account](https://searchata.com). Connect Google Search Console or Bing Webmaster Tools for source-specific reports. Searchata data tools require an active trial or paid plan. Discovery and saved content guidelines do not require a paid plan. Claude access and Searchata billing are separate. See [current plans](https://searchata.com/pricing).

## Install and connect

This release is being prepared for directory review. A public directory listing is not yet available.

For Claude Code users with access to the distribution repository, install with:

```text
/plugin install searchata --marketplace tomzaragoza/searchata-claude-plugin
```

For a local test in Claude Code, start Claude from the plugin folder's parent:

```sh
claude --plugin-dir ./searchata
```

Open `/mcp`, select the Searchata connection, and complete sign-in in your browser. Approve the Searchata workspace that contains the data you want to use.

For a private test in Claude chat or Cowork, upload the plugin ZIP from **Customize > Plugins > Add > Upload plugin**. Open the plugin's **Connectors** tab and connect Searchata. These applications need separate runtime checks before this release is listed as tested on them.

The connector URL is `https://searchata.com/mcp`. Keep this exact URL if you already use a manual Searchata connection. If duplicate tools appear, verify the plugin connection first, then remove the redundant manual connection in Claude settings.

## Workflows

| Workflow | Example request |
| --- | --- |
| Setup | “Help me connect Searchata and check which sites I can use.” |
| Performance | “Compare my site's last 28 completed reporting days with the previous 28 days.” |
| Roadmap | “Which SEO tasks should I investigate first for this site?” |
| Improve page | “Use search data to prepare an update for this page.” |

In Claude Code, the commands are `/searchata:setup`, `/searchata:performance`, `/searchata:roadmap`, and `/searchata:improve-page`. Claude chat can select the matching workflow from a normal request.

Searchata tools provide Google and Bing search reports, Bing keyword research and backlink data, private site crawls, PageSpeed Insights, Chrome UX Report, SEO analysis, and saved search-content guidelines. Call the discovery tool for the current catalog. Available reports depend on source permissions and source data.

## Actions and limits

Google and Bing source tools read data. Starting a crawl creates a Searchata job and reserves crawl credits. Cancelling a crawl changes that job. Performance tests use a separate allowance. These actions must match your request. The plugin does not edit a website through MCP. If you request a file edit, Claude uses its available file tools and your workspace permissions.

Search Console query rows can omit data. Missing rows do not mean zero traffic. SEO findings identify investigations; they do not prove a cause or guarantee rankings. SEO analysis tools do not fetch page text. Read the page before making content claims. Saved content guidelines include retrieval dates and can become outdated.

## Privacy Policy

The plugin contains instructions and one remote connector configuration. It has no local server, hooks, install script, or separate telemetry. Claude sends the selected tool arguments to Searchata. Searchata returns the requested reports to Claude. Provider requests can send the selected URL, property, dates, and filters to Google or Microsoft. Requested crawls fetch public pages. PageSpeed audits can contribute de-identified, grouped script measurements as described in the privacy policy.

Searchata stores account and connection records, encrypted credentials and report caches, private crawl records, and usage records. Tool-call records expire after 30 days; daily summaries can remain for 400 days. Source caches expire within 24 hours. Read the [Searchata Privacy Policy](https://searchata.com/privacy) for the full service practices and retention rules. Claude's own terms and privacy policy apply to data processed by Claude.

Never paste passwords, access tokens, or authorization codes into chat. Use the browser sign-in flow. Reconnect from Claude settings if access expires. Source access is managed on the [Searchata Sources page](https://searchata.com/dashboard/sources).

## Support and license

See the [connector guide](https://searchata.com/docs/connectors) and [troubleshooting guide](https://searchata.com/docs/troubleshooting). Contact [support@searchata.com](mailto:support@searchata.com). Send security reports to [security@searchata.com](mailto:security@searchata.com).

The plugin files use the [MIT License](LICENSE). Searchata service access is governed by the [Searchata Terms](https://searchata.com/terms).
