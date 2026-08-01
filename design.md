# QANT Labs Design Language

## Direction

QANT Labs uses a soft quantum glass visual language: pale blue light, translucent ribbon forms, frosted panels, and precise research-grade typography. The look is inspired by airy quantum education/product interfaces, but the site must keep stronger foreground contrast than the reference image.

The default hero and decorative visuals are CSS-generated abstract glass ribbons. Do not add bitmap hero assets unless a future page needs a concrete, inspectable subject.

## Palette

| Token | Hex | Use |
| --- | --- | --- |
| `--ql-ink` | `#102033` | Primary text and headings |
| `--ql-ink-soft` | `#31465F` | Body text |
| `--ql-muted` | `#5D718A` | Supporting copy and metadata |
| `--ql-surface` | `#F7FBFF` | Main page background |
| `--ql-surface-blue` | `#EAF4FF` | Blue section wash |
| `--ql-surface-lilac` | `#EEF0FF` | Lilac section wash |
| `--ql-glass` | `rgba(255, 255, 255, 0.72)` | Frosted panels |
| `--ql-glass-strong` | `rgba(255, 255, 255, 0.88)` | High-readability cards |
| `--ql-line` | `rgba(67, 95, 130, 0.18)` | Borders and dividers |
| `--ql-teal` | `#057A92` | Primary accent and links |
| `--ql-teal-bright` | `#25D6D0` | Glow accents |
| `--ql-blue` | `#4C7DD9` | Secondary accent |
| `--ql-rose` | `#D85B84` | Sparing warm highlight |
| `--ql-shadow` | `rgba(43, 72, 112, 0.16)` | Card and nav depth |

Contrast rules:
- Body text uses `#31465F` or darker on light/glass backgrounds.
- Headings use `#102033`.
- Links and accent text use `#057A92` or darker.
- White text appears only on dark ink or saturated accent backgrounds.

## Typography

- Primary font: Gotham Rounded when available, then Poppins, Inter, Helvetica Neue, Arial, sans-serif.
- Hero title: clamp from 4rem to 9rem, weight 900, tight line-height, zero or positive letter spacing.
- Section titles: clamp from 2rem to 3.5rem, weight 800.
- Card titles: 1.1rem to 1.35rem, weight 800.
- Body copy: 1rem to 1.15rem, line-height 1.7.
- Labels and nav: uppercase or small caps, 0.04em to 0.12em letter spacing.

## Layout

- Max content width: 1180px to 1240px.
- Section padding: 5rem to 7rem desktop, 4rem mobile.
- Cards use 14px to 22px radius depending on size; no deeply nested card stacks.
- Use full-width atmospheric section bands with constrained content inside.
- Preserve existing Jekyll routes, Bulma grid usage, and static-site simplicity.

## Components

Navigation:
- Fixed, translucent glass bar with blur, fine border, and compact pill links.
- Product and event links use filled pills with high contrast.
- Mobile menu keeps the glass surface and touch-friendly spacing.

Hero:
- Full viewport first impression.
- Left-aligned content on desktop and mobile.
- CSS-generated glass ribbons and orbital highlights sit behind text.
- Include a short eyebrow, large `QANT Labs` heading, high-contrast description, two CTAs, and a compact proof row.

Buttons:
- Primary: dark ink background, white text, rounded pill, subtle lift on hover.
- Secondary: translucent white surface, teal border/text, rounded pill.
- Minimum height: 44px.

Cards:
- Frosted white surfaces, fine blue-grey border, soft shadow.
- Hover lift is subtle and must not shift layout.
- Research cards and contact cards use compact geometric/icon chips.

Products:
- One section for all three, ordered as a ladder from "no experience needed" to
  "you write the code". The order is the argument, so it is data-driven
  (`_data/products.yml`) rather than hand-written per card.
- Numbered rungs and a one-line audience statement carry the progression; the
  cards themselves stay uniform so no product looks like the favourite.
- Qomposer keeps the hardware-neutral backend list, as a line on its own card.

GSoC:
- Keep existing content and accordion behavior.
- Apply the broader glass palette lightly to headings, accordions, and content panels.

## Accessibility

- Maintain at least 4.5:1 contrast for body text and interactive labels.
- Do not rely on color alone for buttons or statuses.
- Keep visible focus states on nav links, buttons, and accordions.
- Avoid text over busy visual regions unless a readable glass/scrim layer sits underneath.
- Respect reduced-motion preferences by disabling decorative animation.

## Scope

This design language covers the homepage, navbar, footer, blog/project/page layouts, GSoC layout styling, contact cards, research cards, the products ladder, and reusable content cards. `qomposer_ui_ux_design.md` remains the product-specific design reference for Qomposer.
