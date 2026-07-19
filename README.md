# GMC Audit Overview

**Chaos Unleashed** | Proprietary tooling (overview only; source code is private)

An auditing tool that checks an e-commerce catalog and its Google Merchant Center feed
against Google's Merchant Center requirements, then produces a prioritized, plain-language
report of likely violations and how to fix them. Built after a real Merchant Center
suspension, to replace guesswork with specifics.

## The problem

Merchant Center suspensions are often vague. A store gets flagged for "misrepresentation"
with no itemized list of what actually triggered it, and the merchant is left guessing
which of thousands of products or fields put the account at risk. Guessing wastes weeks
and often does not fix the real issue.

## What this tool does

- **Audits the live catalog line by line** against concrete policy checks rather than a
  general sense of the rules.
- **Cites the specific field and the specific rule** for every issue it raises, so a fix
  is actionable instead of speculative.
- **References current policy language** so findings point to the actual requirement, not
  a paraphrase that may be out of date.
- **Prioritizes by severity** so the highest-risk items get attention first, and produces
  a clean report a non-technical account owner can act on.
- **Refuses to bluff.** Anything the tool cannot positively verify is labeled as
  unverified rather than asserted as fact. Under a real suspension, a trustworthy report
  matters more than a confident-sounding one.

## Why it matters

Two things make this more than a checklist script: the discipline of citing the exact rule
behind every finding, and the honesty of flagging what it cannot confirm instead of
inventing certainty. Those are the same qualities that make any compliance or enforcement
output trustworthy - the specifics are defensible, and the gaps are labeled.

## Scale

The tool is deliberately self-contained and substantial (several thousand lines in a
single file) so it can be dropped into any environment and run without setup, auditing an
entire catalog in one pass.

---
*Chaos Unleashed. This repository is a public overview. The implementation is proprietary
and maintained privately.*
