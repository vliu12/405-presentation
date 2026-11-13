# Living Under the Hum

**The psychological toll of drone surveillance, and why it should count as civilian harm in future wars**

Final research presentation for *The Future of Warfare* (Carnegie Mellon University, Fall 2026).
Team: Cindy, Victoria, Evelyn, Pranav, Siddhanth.

The whole deck is one file, `index.html`. It needs no installs and no build step.

## Viewing the deck

- **On your computer:** download or clone the repo, then double-click `index.html` to open it in a browser.
- **Online:** turn on GitHub Pages (see below) and everyone gets a shareable link.

| Key | Action |
| --- | --- |
| → / Space / Page Down | Next slide |
| ← / Page Up | Previous slide |
| Home / End | First / last slide |
| N | Show or hide speaker notes |
| F | Full screen |
| E | Edit text in the browser (saved only in your own browser, so commit real changes in the file) |

Add `#slide-6` to the end of the address to jump straight to a slide.

## How the file is organised

Every slide is a `<section class="slide">` block with a banner comment above it, for example:

```html
<!-- ===================== 06 · CASE: WAZIRISTAN ===================== -->
<section class="slide" data-hud="Case 01 · North Waziristan, Pakistan">
    ...slide content...
    <aside class="notes">Speaker notes go here.</aside>
</section>
```

- **Slide text:** edit the words inside the `<p>`, `<h2>`, `<td>` tags.
- **Speaker notes:** edit the `<aside class="notes">` at the bottom of each slide.
- **Label in the top-left corner of a slide:** the `data-hud="..."` value.
- **Colours and fonts for the whole deck:** the `:root { ... }` block near the top of the `<style>` section.
- **Sources:** each content slide has a `<p class="source">` line; the full bibliography is slides 15–17.

Slide numbers (`01 / 17`), corner brackets and the HUD labels are added automatically by the script at the bottom, so you never need to renumber anything.

## Who owns which slides

Fill in names so that two people aren't rewriting the same slide at once.

| Slides | Section | Owner |
| --- | --- | --- |
| 01–03 | Cover, research question, thesis | Pranav |
| 04–05 | Why now, how the harm works | Evelyn |
| 06–09 | Case studies and comparison | Siddhanth |
| 10–11 | The law and objections | Victoria |
| 12–14 | At home, recommendations, conclusion | Cindy |
| 15–17 | Bibliography | everyone |

## Working together on GitHub

**Simplest way (no software needed):** open `index.html` on GitHub, click the pencil icon, edit your slide's block, and click **Commit changes**. If someone else committed first, GitHub will ask you to refresh; just redo your edit on the latest version.

**With branches (fewer collisions):**

```bash
git clone <repo-url>
cd living-under-the-hum
git checkout -b victoria-case-studies     # one branch per person or task
# ...edit index.html, only inside your own slide blocks...
git add index.html
git commit -m "Tighten Gaza case slide"
git push -u origin victoria-case-studies
```

Then open a pull request on GitHub and ask a teammate to look it over before merging.

Ground rules:
1. Edit only inside your own `<section>` blocks; that keeps merges clean.
2. Change the shared `:root` colours or fonts only after the team agrees.
3. Every new fact on a slide needs a source on that slide **and** an entry in the bibliography.
4. Open the file in a browser after each change to check that nothing runs off the slide.

## Turning on GitHub Pages (shareable link)

Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / root → Save.**
After a minute the deck is live at `https://<your-username>.github.io/<repo-name>/`.
(If the repo is private, Pages may need a paid plan; making the repo public works on any plan.)

## To-do before presenting

- [ ] Slide 17: replace `[Article on the LAPD drone-as-first-responder pilot]` with the real LA Times headline.
- [ ] Slide 16: check the Human Rights Watch report title against the report itself.
- [ ] Confirm the five-person team with the TAs (the assignment says four per team).
- [ ] Fill in the owners table above.
- [ ] Rehearse to 10–15 minutes.

## Note on the PowerPoint requirement

The assignment asks for a PowerPoint file. This HTML deck doesn't export to `.pptx`, so a companion version made in Claude's Slides editor exists and does. Keep the two in step before submitting.
