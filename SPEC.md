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

## Research

**RESEARCH-001 · Reviewed sources November 9, 2026 · AI-drafted research synthesis.**
This continues the existing Common Canvas Brand Studio record and preserves its chosen audience and identity. Website observations below are from retrieved product-page text, not customer interviews or a visual usability test. Interpretations are hypotheses, not evidence of buyer behavior. [Implementation issue #3](https://github.com/seafelsayed/is117-brand-studio/issues/3) tracks this documentation work; it is not a peer-feedback issue.

### Three-site comparison

All sources accessed November 9, 2026. Brand claims are attributed to each retailer and have not been independently verified. No competitor product claims apply to the Common Canvas demo shirt.

| Source                                                                                                                  | Observation from the source                                                                                                                                                            | What it suggests for Common Canvas                                                                                                                                                                                                                                                      |
| ----------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [UNIQLO — SUPIMA Cotton T-Shirt](https://www.uniqlo.com/us/en/products/E455365-000/00)                                  | The product description emphasizes SUPIMA cotton, a balanced classic silhouette, and wearing the tee alone or layered. Materials and care are available alongside product information. | Everyday versatility can give a plain tee a clear purpose. Show understandable styling possibilities and useful controls; do not copy unsupported fabric or fit claims. This may serve someone seeking an uncomplicated wardrobe base.                                                  |
| [Everlane — Essential Organic Crew, White](https://www.everlane.com/products/mens-essential-organic-crew-uniform-white) | The page names the product an organic essential, supplies model height and size, and includes a certifications section identifying OCS100.                                             | Specific product context may help a detail-oriented shopper evaluate a basic. Common Canvas should distinguish known demo details from unknown materials and certifications, rather than borrowing an ethical halo. Certification labels alone do not prove every sustainability claim. |
| [Buck Mason — White Slub Curved Hem Tee](https://www.buckmason.com/products/white-slub-curved-hem-tee)                  | The page lists a $48 price, describes USA-grown cotton and production at its Mohnton, Pennsylvania mill, and offers a size/fit guide.                                                  | A basic can be positioned through provenance and construction. That premium route requires supporting facts; Common Canvas currently has stronger grounds for a style-and-belonging story. Price is a dated observation, not a lasting comparison.                                      |

The shared product category is a plain white tee, but the reasons to choose differ: everyday versatility, documented product context, and a manufacturing story. These page observations suggest possible audiences; they do not establish actual customer demographics or sales effectiveness.

### Two positions and the chosen audience

| Position                                                               | Visitor need and proposed promise                                                                                                                                                           | Tradeoff                                                                                                                       |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| A — Personal style without pressure (existing Common Canvas direction) | College students dressing for class want an outfit starting point that leaves room for their own expression. A simple starting point for expressing your style, without pressure to fit in. | Welcoming copy can feel generic unless the page gives concrete, optional styling ideas.                                        |
| B — A quick everyday uniform (comparison hypothesis)                   | Students rushing to class want fewer outfit decisions. A straightforward tee-centered outfit starting point.                                                                                | A prescribed uniform could weaken the existing emphasis on freedom and belonging. Speed and convenience are untested benefits. |

**Chosen audience:** retain position A and the existing primary audience: college students dressing for class who want to look put together and express their style without feeling judged. This choice reuses the Brand Studio agreement; the new competitor review does not independently validate it. Position B remains a contrasting hypothesis, not an approved rebrand.

### Two short persona hypotheses

- **Primary — style explorer before class:** wants an outfit that feels personal; may worry about judgment. The page should offer a white tee as an adaptable base with optional styling ideas. These needs are existing project assumptions, not an interviewed person's biography.
- **Secondary — rushed student before class:** wants to get dressed with little effort. The page should make the tee and next action easy to find. A possible concern is spending too much time choosing an outfit (new AI hypothesis; not yet validated or adopted as a recorded learner choice).

### Look, brand character, and honest persuasion

Reuse the chosen postmodernist direction, rounded forms, cream/dark-green palette, and shared Georgia/Arial typography already recorded above. Preserve clear hierarchy and easy navigation so expressive styling supports the student's task. Do not infer a competitor's rendered layout from extracted page text.

Common Canvas keeps the **Everyperson** character: welcoming, with a calm, casual, encouraging voice. The existing headline, “Your style. Your pace.”, connects that character to voluntary self-expression. An archetype describes the brand, not every customer.

- **Liking:** the existing “No dress code. Make it yours.” message communicates acceptance. Its proposed benefit is lower social pressure; that effect has not been measured.
- **Reciprocity:** the three existing optional styling ideas offer useful inspiration without signup or purchase. They should never imply an obligation to buy.
- Keep the demo-bag boundary visible. No real purchase, payment, or order is offered. Do not invent testimonials, scarcity, sales counts, certification, material quality, fit guarantees, or conversion results. Required size selection is validation, not evidence of a persuasion principle.

### Assumptions, peer review, and next question

**Assumptions to test:** students value a welcoming style message; styling ideas help them decide; the expressive visual direction remains easy to navigate; the rushed-student alternative is meaningfully different. The three competitor pages establish what retailers communicate, not whether these assumptions are true. No customer interviews or new student usability observations are claimed.

**Open question:** Do classmates understand Common Canvas as a flexible starting point for personal style, or as a prescribed outfit? Ask one classmate to explain the intended audience back and challenge one specific site observation.

**Real peer feedback — pending:**

- Classmate-authored feedback issue URL: pending; add the actual link after review.
- Observation challenged and classmate's explanation of the audience: pending.
- Response, resulting revision, or reason for retaining the decision: pending.
- Required constructive issues on classmates' projects: pending real class participation; no issues are fabricated here.

**Change note:** added a sourced three-site comparison and two positioning hypotheses to the existing record, retained the Common Canvas audience and brand, and made research limits and pending peer evidence explicit. This documentation does not certify completion of the in-class review requirement.

**Submission links:** [Research record](https://github.com/seafelsayed/is117-brand-studio/blob/docs/tshirt-research/SPEC.md#research) · [Repository](https://github.com/seafelsayed/is117-brand-studio) · [Existing storefront](https://seafelsayed.github.io/is117-brand-studio/) · [Existing live style guide](https://seafelsayed.github.io/is117-brand-studio/styleguide.html). Feedback issue: pending real classmate review.

## Group Business Research — GROUP-RESEARCH-001

The [published group research record](https://seafelsayed.github.io/is117-brand-studio/research.html) continues this Brand Studio as a proposed business for Seaf Elsayed and Varnit Monga. Source page text was rechecked November 16, 2026. It contains the research question, three original sources, evidence/assumptions, two positions, two persona hypotheses, working audience, design/brand/persuasion, F1–F3 → D1–D3 → C1–C3, proposed fair responsibilities, and AI disclosure. These are proposed refinements; no new product feature or customer study is claimed.

[Issue #6](https://github.com/seafelsayed/is117-brand-studio/issues/6) tracks implementation and pending real review. [Historical issue #5](https://github.com/seafelsayed/is117-brand-studio/issues/5) reports an earlier in-class T-shirt review and contains the owner's retain-audience decision, but lacks detailed reviewer feedback and a retry. It is not evidence of current group review. New member research/decisions, cross-review, and classmate feedback/verification/retry remain pending. Varnit's responsibilities are proposals, not completed work or recorded agreement.

### Reported review update

Seaf reports Varnit Monga opened an original source, checked the finding-to-decision connection, and recommended no changes. This is an owner report, not independent confirmation by Varnit. The specific source/IDs, reasoning, audience explanation and actual review date were not supplied. No revision or reviewer retry is claimed. Remaining contribution evidence stays open in issue #6.

## Plan — T-shirt (TSHIRT-PLAN-001)

Prepared November 16, 2026. Due November 17, 2026 at 8:30 a.m. Eastern. This extends the existing Common Canvas SPEC and style work. It plans the next Build; it does not claim checkout or SQLite already exists.

### Audience, promise and current boundary

Keep the existing audience hypothesis: college students dressing for class who want to express their own style without pressure. Promise: a simple starting point for expressing your style, without pressure to fit in. The earlier T-shirt research suggests useful styling possibilities and clear product information; competitor pages do not validate demand or guarantee usability.

Current prototype: a white-tee page with size selection and a temporary demo bag. The bag resets on reload; the static server rejects POST requests and does not store orders. No simulated checkout, SQLite backend, customer study or persistence result is claimed. This plan supersedes the earlier “no checkout or persistence” boundary only for the proposed next Build; BRAND-001's historical results remain unchanged. Real payments, fulfillment, accounts and manufactured-product claims stay outside scope.

### Two concise approaches

**A — Guided product-to-review flow (recommended):** retain the expressive product hero and optional styling ideas; choose size/quantity, add to bag, review an order summary, then explicitly confirm a simulated order. Show the demo reference and a local order-history lookup afterward. Benefit: review separates exploration from the final action and lets a visitor check the selection. Risk: an extra step may slow a rushed student; keep a clear progress label and back/edit action.

**B — Compact one-page flow:** use the same promise, product facts, styling ideas, size/quantity, review details and simulated confirmation, but place the expanded summary and checkout together below the product. Benefit: fewer page changes. Risk: the long page and adjacent actions may hide the distinction between editing and placing a demo order, especially on phones.

Both approaches must use identical content, fictional price, available demo sizes, backend validation and SQLite data model. Only arrangement/step structure differs. A is an AI recommendation because explicit review fits a low-pressure promise; a student's reasoned choice and the classmate's story explanation are still needed. Do not record either version as built or tested at Plan.

### Five user stories, essential features and observable checks

All checks below are planned and not run for this feature. Existing BRAND-001 checks do not prove checkout or persistence.

#### S1 — Choose a tee without a prescribed style

As a student dressing for class, I want optional styling ideas and clear size/quantity controls so I can choose a starting point that feels like me.

Essential features: existing styling cards, known white color, demo sizes S/M/L/XL, quantity 1–10, fictional $28 USD unit price, visible required-size error and keyboard-accessible controls. No invented fabric/fit guarantee.

Observable check: a reviewer explains one styling idea as optional. Trying to add without a size leaves the bag unchanged and exposes a useful error. Choosing M and quantity 2 adds exactly two M tees and shows $56 before the simulated checkout. Record actual outputs later; misunderstanding or an incorrect count fails the check.

#### S2 — Review and edit before confirming

As a shopper, I want to review size, quantity and the demo total and go back to edit them so I can correct mistakes without pressure.

Essential features: bag summary, edit/remove actions, explicit review step or section, clear back action, and an empty-bag state that cannot proceed. Display fictional demo pricing and no payment/fulfillment statement near confirmation.

Observable check: choose M × 2, open review, change to L × 1, and verify all displayed summaries show L, quantity 1 and $28. Remove the final item and verify checkout is unavailable with a useful explanation. No order may be written before final confirmation.

#### S3 — Complete simulated checkout safely

As a student trying the store, I want an explicit simulated checkout and confirmation reference so I understand what happened without making a real purchase.

Essential features: final order summary, a clearly labeled “Place demo order” action, synthetic email input using demo@example.test, no card/address fields, server-side validation and a reference returned only after successful database commit. Validate the email for the exercise but do not save, send or log it. Use synthetic data only; no signup, email delivery or payment integration.

Observable check: valid L × 1 and synthetic email produce exactly one committed demo order and a reference. Invalid email/size, quantities 0 or 11, and an empty order produce a validation error with no new database row. Disable repeat confirmation while a request is pending and use an idempotency token so retry/double-click returns the original order rather than duplicating it. A database/server failure must show failure without a success reference; the visitor retains a way to retry.

#### S4 — Save, stop, restart and reopen with SQLite

As a returning demo shopper, I want to reopen my saved order reference after the server restarts so I can see that it was stored by the backend.

Essential features: a working local Node 24+ SQLite service, database file outside public files, persistent orders/order-items, order lookup/history, validation and atomic inserts. Browser storage alone cannot satisfy this story. Keep saved unit prices/totals as order snapshots, rather than recalculating historical orders from a changed catalog.

Observable check: create M × 2 at $28, copy its reference and confirm a $56 order in SQLite. Stop the server, restart it using the same explicit database path, reopen history and retrieve the same reference/items/total. Clear browser storage or use another browser session to ensure the result comes from the backend. Change the catalog price in a controlled test and confirm the old order remains $56 while a new order uses the new price. A missing database row or reliance on localStorage fails the check. Record command, reference, database location, actual observed result and limitation in this same SPEC during Build.

#### S5 — Use and explain the flow on a phone and keyboard

As a keyboard or phone visitor, I want readable controls, visible focus and understandable errors so I can review and complete the simulated order.

Essential features: responsive layout, descriptive labels, skip link, visible focus, associated errors/status messages, preserved selections on back/edit, and an obvious local-SQLite versus static-preview mode label.

Observable check: at 375px and desktop width, complete S1–S4 using Tab/Shift+Tab/Enter, with no hidden focused controls or page overflow. Ask a classmate to explain S4 and how its restart check differs from refreshing browser storage. Record their real question and improve the plan accordingly; request their retry of an accepted change. Automated accessibility checks supplement the walkthrough; they do not prove all accessibility or audience fit.

### Planned backend and data contract

Use the professor's [Campus Cotton SQLite starter](https://kaw393939.github.io/is117-demo-days/examples/submissions/run-examples.html), accessed November 16, 2026, as the reference implementation. Its guide documents Node 24+, node:sqlite, server-side validation/prices, and SQLite storage outside public files. It instructs starting with Campus Cotton A and demonstrating save → stop → restart → reopen. The guide was read; the starter has not been run or adapted in this checkpoint.

During Build, inspect and preserve a working copy of the supported starter, then adapt its content and flow to Common Canvas. Keep the current storefront working until that slice passes. Reuse the existing static HTML/CSS/JavaScript identity; no framework migration is planned.

Proposed app API names (not yet implemented): GET /api/products for authoritative demo catalog; POST /api/orders to validate and commit a synthetic order; GET /api/orders/:reference and a local demo-history endpoint to read saved records. The chosen starter may use different route names; map and document the actual contract before coding rather than claiming these are its current routes.

Proposed schema: orders(id, reference UNIQUE, request_token UNIQUE, created_at, total_cents); order_items(id, order_id foreign key, product_id, size, quantity, unit_price_cents). Use integer cents, prepared statements, allowlisted size/product, bounded integer quantities and one transaction for order/items. The server computes totals from its catalog and ignores or rejects client price tampering. Test a request that submits a $1 total: the server must preserve the $28 unit price or reject the request, never trust the submitted total. Do not store email or payment details.

Development setup to document during Build: bind locally to 127.0.0.1 and use an explicit SQLite path outside public/; preserve that path across restarts. Do not expose the database file through HTTP or commit generated databases. Include a synthetic fixture and a reproducible setup command. A static GitHub Pages prototype may remain available for visual review, but it must state that it has no SQLite service. Provide the local backend code/setup and restart evidence as the working SQLite demonstration; any public backend deployment is a separate future decision. Do not deploy the classroom-only starter as a real store.

### Carry forward brand, visuals and two honest persuasion elements

Keep Common Canvas, the Everyperson character and calm/casual/encouraging voice. Reuse the selected postmodernist rounded forms, original wordmark, cream/dark-green palette, warm accents and shared Georgia/Arial styling from the live style guide. Both approaches retain identical branding so the flow comparison is fair.

**Liking:** keep “No dress code. Make it yours.” as a welcoming invitation. Intended benefit is less social pressure, not a measured result. Do not prescribe an identity or make belonging depend on buying.

**Reciprocity:** retain the three freely available styling ideas without signup or purchase. They offer inspiration without an obligation. Do not invent testimonials, scarcity, stock, quality certifications or conversion claims. Review/back/edit support voluntary decisions; required size validation alone is not a persuasion principle.

### Build order, peer feedback and evidence

Build in small slices: inspect/run the unchanged starter; adapt product data and branding; implement selection/review/checkout using one validated SQLite service; exercise positive/negative and restart cases; compare A/B with identical content; collect the classmate's story explanation and useful question; revise and retry accepted feedback. Record actual results, not this planned checklist as completed evidence.

Current feedback status: [review-request issue #8](https://github.com/seafelsayed/is117-brand-studio/issues/8) is open; no classmate feedback specific to this T-shirt Plan has been supplied. Varnit's earlier business Research and Portfolio Plan approvals are separate reviews and are not carried over as a T-shirt Plan review. Publish a review request in this repository. Ask a classmate to explain S4 and identify one failure its check would catch, then ask a useful question about the plan. For incoming issues, record implement/investigate/defer/decline with a reason, a linked documentation/code commit, actual verification and reviewer retry before closing a resolved issue. If feedback remains missing, contact the instructor promptly to arrange a reviewer.

AI assistance: Codex inspected the existing SPEC, storefront/server boundary and course starter guide, then drafted these approaches, stories, backend proposal and checks. The plan is AI-assisted and subject to Seaf's decisions. No classmate question, student explanation, backend implementation, checkout result, SQLite restart success or reviewer retry is fabricated. This checkpoint adds documentation; it does not submit Canvas coursework.
