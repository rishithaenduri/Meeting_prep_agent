<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Meeting data lives in browser localStorage via src/lib/store.ts (useSyncExternalStore) — no login needed; move to Lovable Cloud if multi-device sync is required.
- AI briefings run in a server function (briefing.functions.ts -> briefing.server.ts) so the AI key stays server-side.
