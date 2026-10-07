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

## Project rules
- HRMS hiring workflow (`/hrms`, `/hrms/$hrfId`) is a front-end mockup driven by `src/lib/hrms-mock.ts` with local state only — no persistence until the user asks for a real backend.

- Shared React context owns the connected HRMS demo and careers publication state; no browser storage or backend writes, so reload resets the demo.
- Candidate records and contextual joining forms live in reusable HRMS components; stage checks prevent premature joining actions.
