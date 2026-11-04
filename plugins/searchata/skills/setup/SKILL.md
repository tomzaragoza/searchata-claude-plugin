---
name: setup
description: Help connect Searchata to Claude, inspect available Searchata tools, or resolve Searchata setup and source-access errors.
---

# Set up Searchata

Use the Searchata connection declared by this plugin. Its URL is `https://searchata.com/mcp`.

If tools are unavailable, direct the user to the plugin's Connectors tab in Claude chat or Cowork, or `/mcp` in Claude Code. Browser authorization selects the Searchata account and workspace. Never request credentials in chat.

Current browser authorization requires a Google sign-in and a connected Google Search Console account. Connect Bing separately for Bing reports. Call `get_tools` for the current capabilities. Once authorized, discovery and saved content guidelines require no active plan and do not read connected source reports. Data tools require an active trial or paid plan. Do not describe a billing requirement as a missing source.

For Google data, use `google_search_console_list_properties`. For Bing site data, use `bing_webmaster_tools_list_sites`. Select an existing authorized property that matches the user's site. Ask when multiple properties remain plausible. Bing keyword research requires a Bing connection but no property ID.

For a setup error, report the returned requirement and Searchata action URL. Retry after that requirement is resolved. Finish with the connection state, available source, and one useful next request.
