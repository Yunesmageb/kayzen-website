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

## App architecture
- Use the shared site Logo for header/footer branding and the shared WHATSAPP constant for contact destinations so updates remain consistent.
- Keep page content in TanStack leaf routes and navigation/footer in the shared site module so public URLs and layout stay consistent.
- Keep portfolio category filtering and image collections in the shared data module; render the same accessible gallery on home and work pages so each service supports multiple images.
- Use CSS animation with reduced-motion support for the advertising illustration and intersection-triggered counters; do not add a 3D runtime for a bitmap composition.
- Treat uploaded mockup brands, statistics, and prior generated work as demo content until the owner confirms them; never turn them into verified client claims.

- Keep service descriptions and matching portfolio categories in the shared data module; service dialogs link to a validated work search category so samples match the selected service.
- Build partner marquees from two identical nonshrinking groups and animate by half the track width so the loop remains seamless at every breakpoint.
