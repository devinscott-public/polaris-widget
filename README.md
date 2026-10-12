# polaris-widget

The statement engine that draws the Polaris statements and ARR widget in a Claude chat. One generic JavaScript file, `statement_engine.min.js`, and the layout it follows (rows, labels, order), built into the same file.

- No data, no credentials, no company names. The figures a person sees are passed to the engine by the chat, from that person's own connection. Nothing here reads or sends them.
- The source of truth is Diversis's internal `polaris-plugin` repository. This repository only publishes a built copy so a chat widget can load it from a public CDN (jsDelivr). Do not edit the file here; it is replaced on each release.
- Each release has a tag (`v1.0.0`, `v1.1.0`, ...). The plugin pins one tag and the file's SHA-384 hash, so the browser refuses a file that has changed.
- Load it as `https://cdn.jsdelivr.net/gh/devinscott-public/polaris-widget@v1.0.0/statement_engine.min.js`.

Questions: devin@diversis.com.
