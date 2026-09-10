# Top 100 Regen makeover

The 2026 makeover is a small, surgical refresh rather than a rebuild.

## Identity
- Top 100 family blue remains the common visual DNA.
- Acid/lime green is Regen's distinct accent.
- Strapline: **Same DNA. New generation.**
- Homepage is evergreen rather than hard-coded around Season 1.
- Current season shown as **S4**.
- Regen is positioned as the gateway for new managers into the Top 100 family, created in 2025 for Top 100's 10th anniversary.

## Structure
- Thin Top 100 family navigation:
  Top 100 · Stats & History · Tournaments · Awards · Voting · Regen
- Regen-local navigation:
  News · Archive · Rules · Subscribe · Join
- Managers remains a category, not a first-class navigation destination.
- Homepage includes a simple Original Top 100 / Top 100 Regen explainer.
- Shared app gateways are visible without turning Regen into an app directory.

## Content
- Removed stale Season 1 / 25 seasons / 10 years hard-coding.
- Regen Rules work as an exceptions layer over the canonical Top 100 rulebook.
- Historical rule versions are retained but visually de-emphasised.
- Youth Cup / Shield are no longer permanent navigation items; future competition operation belongs in Tournaments.
- Removed the old waiting-list form. Joining is by recommendation, word of mouth or direct application in Soccer Manager when a club is available.
- Archive includes Regen-site history plus pre-site launch material from the original Top 100 blog.
- Subscribe page explains what emails contain and uses the standard Micro.blog subscription endpoint.

## Theme quirks discovered
- The inherited theme used sticky/fixed header rules strong enough to override ordinary custom CSS. A late inline override in `layouts/partials/header.html` is required to keep the header non-sticky.
- The inherited theme also applied a purple background treatment to visited links. The same late inline override removes it globally.
- Micro.blog's built-in Archive page is overridden at `layouts/_default/list.archivehtml.html`.
- Category term pages use `layouts/categories/term.html`.

## Final fine tuning
- Increased homepage hero-title contrast.
- Restyled the `How it started` links as deliberate launch-history links.
- De-emphasised historical Rules versions using collapsible details.
- Added a subtle current-rule-reference callout.
- Styled the Subscribe form and improved small-screen form layout.
- Managers removed from header/footer navigation.

## Domain integration
- Canonical target: `regen.smtop100.blog`.
- Main `smtop100.blog` migration is complete, so Regen integration can proceed now.
- Update family navigation and internal ecosystem links to the live Top 100 domains before cutover.
- Connect `regen.smtop100.blog` to the existing Regen Micro.blog site and make it canonical.
- Verify generated URLs, feeds, social-card metadata and subscriptions on the new host.
- Keep `top100regen.website` as a legacy domain and redirect it to `https://regen.smtop100.blog/` once the new domain is proven.
