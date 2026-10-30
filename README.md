# Citation

[Website](https://citation.co/) · [Setup](https://citation.co/docs/mcp) · [Support](https://citation.co/contact) · [Privacy](https://citation.co/privacy)

The Citation plugin connects compatible AI assistants to research saved in a Citation workspace. It includes four skills for drafting, research, reference formatting and citation review, and the remote MCP connection at `https://citation.co/mcp`.

## Connect

Install the plugin through your client, sign in to Citation, choose your workspace and review the requested permissions. OAuth authorization code with PKCE is supported. Every user authorizes their own workspace. No shared API key, reviewer credential or customer data is included.

## Capabilities

Find and read saved documents and sources. Create or revise drafts after a user request. Add and update source metadata, format references with CSL, inspect citation metadata, and export TXT, BibTeX or RIS. Permissions distinguish document reading and writing, source reading and writing, and exports. Users can revoke access in Citation MCP settings.

Citation checks inspect saved metadata and citation links. They do not perform plagiarism scanning or comprehensive factual verification. The MCP tools do not delete, invite, share, publish, send messages, execute payments or run arbitrary code. Write tools use idempotency keys and document version checks.

## Included files

The Cursor manifest is `.cursor-plugin/plugin.json`. The Claude ecosystem manifest is `.claude-plugin/plugin.json`, which is also accepted by Grok Build. Both use the same `skills/` content. Cursor uses `mcp.json`; the Claude manifest declares its MCP endpoint directly. No hooks, executables, package installers or telemetry are bundled.

## Network and credentials

The plugin configures only `https://citation.co/mcp`. Authentication discovery and consent use Citation HTTPS endpoints. Source URLs are saved metadata, not arbitrary fetch instructions. Credentials belong to the user and are kept by the client; never place them in a shared configuration file.

## License

The plugin configuration and skill content are provided under the MIT License. Citation service access remains governed by the [Citation Terms](https://citation.co/terms). The license does not grant rights to Citation trademarks or the hosted service implementation. Citation brand artwork is supplied only to identify the official integration.
