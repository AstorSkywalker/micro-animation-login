# Micro-animation Login

A polished, responsive login-page concept for an internal electoral platform. The project is built with plain HTML, CSS, and JavaScript, so it runs without a build step or framework.

## Live demo

Once GitHub Pages finishes its first deployment, view the page here:

**[Open the live login page](https://astorskywalker.github.io/micro-animation-login/)**

The first deployment may take a minute or two after the workflow is enabled.

## Project files

- `login.html` — the complete login screen, including layout, styles, and interactions.
- `index.html` — a small entry-point redirect so the GitHub Pages root opens the login screen.
- `logo (1).webp` — the CNE Honduras logo used by the interface.
- `.github/workflows/deploy-pages.yml` — automatically publishes the static site with GitHub Pages.

## Animations and interactions

### Floating labels and focus states

The form labels begin inside each input and move above the field when it receives focus or contains text. Blue borders and a soft focus ring make the active field easy to identify without adding visual noise.

### Password visibility toggle

The eye button switches the password field between masked and visible text. Its accessible label updates to describe the current action.

### Lock-centered submit animation

Submitting the form triggers a short microinteraction around the lock icon:

1. The lock gently pops to acknowledge the click.
2. The shackle rotates upward to suggest access being granted.
3. Eight small, multicolored rays radiate outward from the icon.
4. The button remains disabled briefly to prevent duplicate submissions.

The interaction is intentionally centered on the lock instead of using a large page-wide effect. This keeps the feedback immediate, playful, and connected to the meaning of the action.

### Reduced-motion support

Users who prefer reduced motion receive shortened transitions, and the decorative rays are hidden through `prefers-reduced-motion`.

## Design ideas

- **Institutional trust:** deep navy backgrounds, restrained typography, a white card, and a security note create a dependable government-platform feel.
- **Quiet hierarchy:** the logo and title establish identity first, while the blue action button provides one clear primary action.
- **Soft depth:** gradients and a broad shadow separate the login card from the background without making the interface feel heavy.
- **Friendly precision:** rounded fields, line icons, floating labels, and the small lock burst make the formal experience feel approachable.
- **Responsive by default:** spacing, typography, and card proportions adapt for smaller screens.

## Run locally

Open `index.html` or `login.html` directly in a browser. No installation is required.

## Scope

This is a front-end prototype. The submit handler currently validates the fields and logs the normalized user value to the browser console; it does not connect to a real authentication backend.
