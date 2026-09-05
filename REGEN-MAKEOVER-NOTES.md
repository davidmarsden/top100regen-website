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
  Top 100 · Archive · Tournaments · Awards · Rules · Regen
- Regen-local navigation:
  News · Archive · Rules · Subscribe · Join
- Managers remains a category, not a first-class navigation destination.
- Homepage includes a simple Original Top 100 / Top 100 Regen explainer.
- Shared app gateways are visible without turning Regen into an app directory.

## Content
- Removed stale Season 1 / 25 seasons / 10 years hard-coding.
- Regen Rules now work as an exceptions layer over the canonical Top 100 rulebook.
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

## Domain plan
- `top100regen.website` remains canonical for now.
- Planned future canonical home: `regen.smtop100.blog`.
- Do **not** move Regen first. Complete the main `smtop100.blog` migration to Micro.blog and stabilise the family navigation/URL structure before moving Regen underneath it.
- After the main-site cutover is proven, connect `regen.smtop100.blog`, update Micro.blog site/base URL and social-card metadata, and redirect `top100regen.website` to the new canonical domain.
