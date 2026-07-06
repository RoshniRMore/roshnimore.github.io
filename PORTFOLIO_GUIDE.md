# Portfolio Guide

This file is the working reference for future edits to this GitHub Pages portfolio. Use it to keep changes consistent, scoped, responsive, and easy for a future agent or maintainer to continue.

## Project Overview

- The site is a static GitHub Pages portfolio served from the repository root.
- The main page is `index.html`.
- The current implementation is a single HTML file with inline CSS, inline JavaScript, and embedded image data.
- The site uses a terminal-inspired visual style with dark backgrounds, green accents, monospace typography, and section-based navigation.

## Current Page Structure

The main sections in `index.html` are:

- Fixed navigation
- Hero
- About
- Skills
- Experience
- Projects
- Education
- Contact

When making content or layout changes, inspect the current section before editing. Prefer small, local changes over rewriting the whole file.

## Resume Convention

The resume PDF should live at:

```text
assets/resume.pdf
```

When the resume file is available, add it to the project using that exact path. Do not generate placeholder resume content or rename the file unless this guide is updated.

The portfolio exposes a visible resume download action in the hero button group:

```html
<a href="assets/resume.pdf" class="btn-secondary" download>Download Resume</a>
```

If the button text needs to match the terminal theme, use concise labels such as `Download Resume` or `Resume`. Keep the link target as `assets/resume.pdf`.

## Mobile-First Responsive Rules

- Design for small screens first, then enhance for tablet and desktop.
- Test layout at 375px, 768px, and desktop widths before considering a change done.
- Avoid fixed widths that can overflow mobile screens.
- Use wrapping, flexible grids, `max-width`, `minmax()`, and percentage-based widths where practical.
- Hero buttons, project links, contact links, forms, and two-column sections must stack or wrap cleanly on mobile.
- The page must not create horizontal scrolling on mobile.
- Tap targets should remain comfortable on touch devices.
- Text should wrap naturally instead of clipping or shrinking too aggressively.

## Editing Conventions

- Preserve the existing visual identity unless the requested change explicitly changes the design direction.
- Keep edits scoped to the requested feature or bug.
- Avoid unrelated refactors, formatting churn, or large rewrites.
- Prefer semantic HTML for new content.
- Use existing button classes such as `btn-primary` and `btn-secondary` when possible.
- Keep GitHub Pages compatibility in mind: use static files and relative paths.
- Do not introduce build tooling unless the project is intentionally migrated away from the current static setup.

## Accessibility And Quality Checklist

Before finishing a visible page change, check:

- Links have meaningful text.
- External links that open in a new tab include `rel="noopener noreferrer"`.
- Images have useful `alt` text.
- Buttons and links are keyboard reachable.
- Forms keep labels associated with their inputs.
- Color contrast remains readable.
- The browser console has no new errors.
- The resume link works when `assets/resume.pdf` exists.

## Agent Workflow

For future agents working in this repo:

1. Inspect `index.html` and this guide before editing.
2. Confirm whether `assets/resume.pdf` exists before wiring or testing the resume download.
3. Make the smallest practical change that satisfies the request.
4. Verify the page still works as a static GitHub Pages site.
5. Test responsive behavior at mobile, tablet, and desktop widths.
6. Summarize exactly what changed and whether the resume file was present.

## Future Improvement Backlog

These are useful improvements, but they should be done only when requested or when they are necessary for a specific change:

- Move inline CSS into a separate stylesheet.
- Move inline JavaScript into a separate script file.
- Replace embedded image data with normal image files under `assets/`.
- Fix visible text encoding artifacts in the page.
- Improve mobile navigation instead of hiding all nav links.
- Optionally add a second resume download link in the contact section.
- Add basic SEO and social preview metadata.
- Add a lightweight local preview workflow.
