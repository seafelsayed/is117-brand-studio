# Brand Studio decisions

This is the durable agreement between the learner and agent. Keep it concise and update it only with agreed choices or actual evidence. `Not chosen yet` is a valid status. Persona cards are hypotheses unless supported by real research.

[LEARNING.md](LEARNING.md) holds the short, reviewable record of learner explanations and help received. Keep the brand decisions and implementation evidence here; link rather than duplicate them.

## Current stage

- Stage: BRAND-001 kept, merged, and published.
- Current feature: `BRAND-001` — first branded storefront and live style guide.
- Status: Kept; PR #2 merged into main at 1dec4a9.
- Next small decision: Submit the verified live storefront URL; no follow-up feature selected.

## Product boundary

The product is the same white T-shirt throughout the comparison. The baseline offers a size selector and temporary demo bag. No real orders, payment, accounts, or persistence. Keep product facts stable between directions; do not add unsupported claims about materials, manufacturing, sustainability, fit, delivery, scarcity, reviews, or sales.

## Audience hypotheses

The primary need guides the page. Give the secondary card one contrasting need to check that same page; keep both cards brief.

| Tiny card                             | Primary audience                                                                   | Secondary audience                                               |
| ------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Person in a concrete situation        | College students dressing for class                                                | Students getting dressed quickly before class                    |
| Goal or meaning they seek             | Look put together and express their style                                          | Get dressed with little effort                                   |
| Concern before choosing               | Feeling judged for personal style (learner explanation)                            | Not chosen yet                                                   |
| What the page should help them decide | Explore styling a white tee as a personal outfit base (AI suggestion; provisional) | Find a simple outfit starting point (AI suggestion; provisional) |
| Evidence or assumption                | Assumption; not validated                                                          | Assumption; not validated                                        |

## Early brand brief

| Decision                                 | Agreement                                                                      |
| ---------------------------------------- | ------------------------------------------------------------------------------ |
| Brand name                               | Common Canvas                                                                  |
| One-sentence promise                     | A simple starting point for expressing your style, without pressure to fit in. |
| Primary archetype: the brand's character | Everyperson — welcoming and centered on belonging; approved AI suggestion      |
| Three voice traits                       | Calm, casual, encouraging                                                      |
| One example line in this voice           | Your style. Your pace.                                                         |
| Learner's predicted audience effect      | Feel relaxed: “they can wear what they want without feeling judged.”           |

## Visual decision

Compare two small hero previews before building the whole page. Hold the product, headline, supporting copy, and action identical. Use specific real design references and annotate visual choices, intended effect, and risk.

A simple original SVG wordmark is enough. Show small-size and one-color presentations; they may use the same asset when it works.

| Item                                              | Agreement or evidence                                                                                                                                                                                                                                                 |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Shared headline / support / action                | “Your style. Your pace.” / “Start with a white tee. Make it yours, whatever that looks like.” / “Choose your size” (preview action proposed by AI).                                                                                                                   |
| Modernist preview, reference, and annotations     | [Modernist hero](public/explorations/modern.html); Christian Dell, Dell-Lampe Type K (1929), V&A. Reference image inspected. Initial desktop image inspected; final hero responsive render inspection remains limited; prepared site browser suite passes in CI.      |
| Postmodernist preview, reference, and annotations | [Postmodernist hero](public/explorations/postmodern.html); Martine Bedin, Super prototype (1981), V&A. Reference image inspected. Initial desktop image inspected; final hero responsive render inspection remains limited; prepared site browser suite passes in CI. |
| Chosen direction and reason                       | B / postmodernist. Learner: “its more easy to navigate” after initially expressing a preference without a reason. AI had suggested mixed lettering/rounded shapes as possible reasons; learner supplied navigation instead.                                           |
| Original SVG logo                                 | [SVG proposal](public/assets/common-canvas-proposal.svg), [review board](public/explorations/logo.html); learner approved: “keep it.”                                                                                                                                 |
| Monochrome and small-size variants                | Same one-color SVG; proposed navigation presentation 190 × 44 px.                                                                                                                                                                                                     |
| Logo review at actual use size                    | AI inspected actual 190 × 44 px navigation render and enlarged one-color render; learner approved “keep it.”                                                                                                                                                          |
| Shared palette, typography, spacing, and assets   | Chosen B implementation: cream #f7f3e9, dark green #263d34, soft green #e2e7dc, warm accent #dfc7b2; Georgia + Arial italic/body; shared spacing tokens in public/styles.css; assets/wordmark.svg.                                                                    |

## Ethical persuasion

Choose two applications that help the visitor make a voluntary, informed decision. Record their real implementation and mechanism rather than a principle name alone. Required size selection or validation alone does not establish consistency. Do not invent social proof, scarcity, authority, or product facts.

| Principle   | Actual copy or interaction                                                   | Visitor benefit / factual support                                                                                                                    |
| ----------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Liking      | “No dress code. Make it yours.” in welcome banner and styling section        | Learner: “they wont feel olbliagted to dress smth in speicifc.” Welcoming language supports voluntary personal style; proposed effect, not measured. |
| Reciprocity | Three optional styling ideas at #style-ideas; no signup or purchase required | Freely offers practical inspiration; learner approved “yea.” No obligation implied.                                                                  |

## BRAND-001 — first branded storefront and live style guide

**Scope:** turn the working neutral storefront into the chosen brand's first coherent page. Keep the existing size selector and demo bag usable. Do not add checkout or all future features.

Keep when:

- The learner has chosen the audience hypotheses, brief, visual direction, and logo; the page visibly expresses those choices.
- Two annotated hero directions compare modernist/postmodernist thinking with the same content and real source links.
- The selected SVG logo works at small size and in one color; the presentations may share one asset.
- The storefront and live style guide share CSS variables, typography, components, and assets; they do not drift into separate identities.
- Two ethical persuasion applications are visible and their claims are supportable.
- Prepared checks pass, the agent has reviewed the slice and discussed one actual check, and the learner has reported a browser impression plus keyboard/mobile observations.
- The issue, branch, commit, and PR explain this feature in the learner's repository; agreed decisions and actual evidence are saved here. The learner has approved keeping and merging the change, and the merge into `main` is verified. Publishing is a separate choice.

## Evidence

Write a short result and link only evidence that exists. A passing browser check is evidence for its assertions, not customer research or proof of full accessibility.

| Spec ID   | Files                                                                                                                          | Issue / PR                                                                                                                                                       | Actual checks and observations                                                                                                                                                                                                                                                                                            |
| --------- | ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BRAND-001 | public/index.html, public/styleguide.html, public/styles.css, public/shop.js, public/assets/wordmark.svg, public/explorations/ | [Issue #1](https://github.com/seafelsayed/is117-brand-studio/issues/1), [PR #2](https://github.com/seafelsayed/is117-brand-studio/pull/2), branch feat/brand-001 | Formatting/lint and 7 server tests pass; manual Chrome no-size and M-add checks pass. [GitHub CI passed](https://github.com/seafelsayed/is117-brand-studio/actions/runs/41558823089/job/125664194028) on c29c54f: formatting, lint, 7 server tests, 10 Chromium browser checks including axe. Learner observations below. |

## Later

No follow-up is selected. After keeping `BRAND-001`, choose one next cycle: perhaps a brand story, a supported fit guide, or richer demo-bag behavior. Agree its scope and add one new spec ID at that time.

### Implementation and current checks

- Shared `public/styles.css` and `public/assets/wordmark.svg` now drive storefront, guide, and studio identity. Storefront adds optional styling cards, approved message, and adjacent live bag feedback. Guide shows actual chosen identity and shared components.
- Prepared formatting and lint passed; all 7 server tests passed on rerun with network permission. Full browser suite remains blocked by the macOS Chromium launch sandbox, not reported as passed.
- Actual Chrome observation: adding without a size displayed the size error and left bag at 0. Selecting M and adding produced bag count 1, size-M item, and adjacent confirmation. Learner interpretation recorded below after an AI example.
- AI inspected storefront, guide, and studio header/hero at 400px in Chrome; desktop inspection remains partial due browser control interruptions. Full prepared browser/accessibility suite [passed in GitHub CI](https://github.com/seafelsayed/is117-brand-studio/actions/runs/41558823089/job/125664194028) on c29c54f.
- Persuasion reference: https://www.influenceatwork.com/7-principles-of-persuasion/ (official overview read); applications are design hypotheses.

### Learner review observations

- First impression: “looks nice and easy to navigate.”
- Keyboard: “it navigates through the website”; visible focus and keyboard add-to-bag completion not explicitly described.
- Narrow view: confirmed text and buttons fit on screen after a direct question.
- No-size check interpretation: “ask them for the size,” following an AI example; assisted evidence.
- Learner approved the four-point record summary as accurate: “all looks good.” Learner approved keeping/merging; PR #2 merge verified at 1dec4a9.

### Verified publication

- [Live storefront](https://seafelsayed.github.io/is117-brand-studio/), [style guide](https://seafelsayed.github.io/is117-brand-studio/styleguide.html), [successful publishing run](https://github.com/seafelsayed/is117-brand-studio/actions/runs/41559598925).
- Published site loaded; no-size submission showed error with bag 0; selecting M produced bag 1 and adjacent confirmation. Verified by AI in the live browser.
