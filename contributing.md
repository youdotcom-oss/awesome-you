# Contributing

Thanks for contributing to the Awesome You.com list. This repo is the archive of projects built on You.com APIs at hackathons — every submission from each event, with winners called out. If you built something, we want it here.

## How this list works

**This list is an archive.** Each entry records what was built and awarded at a
You.com hackathon, as of that event. Placements come from the official results and are
never re-judged after the fact.

That means existing entries are not removed as they age. Hackathon projects are built
in a weekend, so repos get archived, free-tier demos spin down, and recordings expire.
That is expected in an archive, not a defect — an entry is a record of what happened,
and it stays.

## What qualifies

If you built it at a hackathon with You.com APIs and it has a working link, it belongs
here. That is the whole bar:

- Built at a hackathon — one of ours or anyone else's.
- Uses at least one You.com API, MCP tool, plugin, or skill for real, rather than as a
  stub or a placeholder.
- Has at least one public link that works: a repository, a live demo, or a demo video.
  A public repository with a README is preferred, and is what the entry should link to
  when it exists.

**You do not need to have won anything.** Winners and finalists are called out with
their placement, but most entries here never placed, and that is the point — this is a
record of what people built, not a leaderboard.

**Built it at a hackathon we didn't run?** Still welcome. Open a pull request and we
will add a section for that event.

Links should work at the time you submit them. Nobody is expected to keep them alive
forever.

## How to add your project

1. Fork this repo.
2. Add your entry to the correct event section in `README.md`:

   ```markdown
   - [Project Name](https://github.com/you/repo) - One-line description of what it
     does and why it is awesome. By [@you](https://github.com/you). [Demo](url)
     [Live](url) *Search · Research · MCP*
   ```

   Rules:

   - Name the project the way its own README names it. Submission forms and event
     spreadsheets carry typos, descriptions in place of names, and company prefixes,
     so the README wins. Two exceptions: ignore repository or venue suffixes that
     aren't part of the product name, and fall back to the submitted name when the
     README is unmodified scaffolding that never names the project.
   - Description starts with an uppercase letter and ends with a period.
   - Description does not repeat the project name.
   - Credit the builder by GitHub handle, not by full name. Handles are already
     public; names and contact details from event submission forms are not ours to
     publish. Omit the credit if the project has no repository.
   - End the entry with the You.com APIs it was built on, in italics, separated by
     `·`. Use the short names: `Search`, `Research`, `Finance Research`, `MCP`,
     `Plugins/Skills`, `SDKs`.
   - Put your entry in your event's section, under its track if that event had
     tracks. Entries are alphabetical within a subsection, except `Winners`, which
     is ordered by placement (1st, then 2nd, then 3rd).
   - Only podium finishes get a 🥇/🥈/🥉 medal, in the Winners subsection. Everything
     else goes in its track subsection with no medal or emoji.
   - All URLs must be HTTPS (unless the project is only hosted on HTTP).
   - Link only URLs that resolve. If a demo has already gone offline, leave it out
     rather than linking a dead page.

3. Run `npx awesome-lint` locally and fix anything it reports. CI runs the same
   check on every pull request.
4. Open a pull request titled `Add Project Name`.
5. In the PR body, include: the hackathon and event dates, which You.com APIs you used, and any demo or live URLs.

## Review

Maintainers review each new PR against the criteria above: links that resolve at submission time, and a description that matches what the project actually does. Markdown must be clean and grammatically correct. Existing entries are not re-reviewed as links age.

## Style notes

- No emoji in descriptions; medals on the project title are reserved for actual wins.
- Do not add a CI badge, sponsor badges, or "Inspired by awesome" links.
- Keep the Contents list in sync when adding an event section.

A few structural rules are enforced by `awesome-lint` and will fail CI if broken:

- Do not add a `License` section to the README. The `LICENSE` file at the repo
  root is the only place the license belongs.
- Do not add `Contributing` or `License` to the Contents list. Only event
  sections belong there.
- The `<!-- lint disable awesome-badge -->` comment at the top of the README is
  deliberate. This list keeps entries for archived and unmaintained projects, which
  the Awesome manifesto excludes, so it does not carry the Awesome badge and is not
  submitted to `sindresorhus/awesome`. `awesome-lint` is kept for entry formatting.
