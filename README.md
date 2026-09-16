# sandbox-orchestrator

Provisions per-session containers — powers both the VSCode test and the DSA round.

Full plan: see the `platform` repo's README (sibling folder).

**Build order:** #3.

**Lift from:**
- `open-web-agent/src/lib/docker.ts` — per-session `code-server` container + a "runner" container serving a live preview (iframe-header handling already solved here); swap "clone GitHub repo" for "seed a test template," drop the AI agent container
- `open-web-agent/src/components/workspace/WorkspaceClient.tsx` — tab UI pattern (VSCode / Preview) for `web-frontend` to copy

**Note:** same mechanism serves DSA round and VSCode test — different starter template, not a separate system.
