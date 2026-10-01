# Movement Vendor Finder

An AI-assisted local-business research workflow designed to help identify potential vendors for a student-benefit program.

> **Human-in-the-loop principle:** AI researches, verifies, organizes, and recommends a next step. A human makes the final vendor decision and approves all outreach.

## What this project does

The Vendor Finder turns an open-ended business-development task into a repeatable research workflow:

**SEARCH → VERIFY → RESEARCH CONTACT → CHECK EXISTING OFFER → IDENTIFY OPPORTUNITY → CREATE OUTREACH ANGLE → HUMAN REVIEW → OUTREACH**

The workflow is designed to help a business-development team spend less time researching and more time having qualified conversations.

## Core capabilities

- Finds potential local and independent businesses near a target location
- Verifies business details using public sources
- Separates verified facts from observations and assumptions
- Researches publicly listed decision-makers and business contacts
- Checks for existing student-specific offers
- Avoids treating general promotions as student discounts
- Identifies a potential student-benefit opportunity
- Creates a personalized outreach angle
- Produces one practical **Mary's Next Move** for the human reviewer
- Records research sources and unresolved conflicts
- Requires human approval before outreach

## Guardrails

The agent must **never**:

- Invent a business, owner, manager, email address, phone number, offer, or eligibility requirement
- Guess local ownership
- Guess who the decision-maker is
- Claim that no student offer exists when the research only failed to find one
- Treat a general promotion as a student-specific discount
- Automatically contact a business
- Resolve conflicting public sources by guessing
- Make a final vendor-selection decision for the human reviewer

When evidence is incomplete or conflicting, the correct output is **Needs Research** or **Conflicting — Verify**.

## Example use case

**Target:** Pima Medical Institute — Albuquerque campus  
**Initial category:** Food and coffee  
**Initial geographic focus:** Approximately 1 mile  
**Preference:** Locally owned or independent businesses

The same workflow can be reused for another school, employer, neighborhood, customer segment, category, or geographic area by changing the target parameters.

## Repository structure

```text
movement-vendor-finder/
├── README.md
├── LICENSE
├── docs/
│   ├── agent-instructions.md
│   ├── research-workflow.md
│   ├── data-dictionary.md
│   └── human-review-guide.md
├── examples/
│   └── sample-agent-run.md
└── templates/
    └── vendor-prospect-template.csv
```

## How the workflow works

### 1. Search
Find businesses matching the target location, category, radius, and qualification criteria.

### 2. Verify
Check address, category, local/independent ownership, public business contact information, and other important facts.

### 3. Research contact
Look for a publicly listed owner, manager, general manager, partnership contact, or business contact. If sources conflict, flag the conflict.

### 4. Check existing offers
Look for a current student-specific offer using official business sources first. A general special is not automatically a student offer.

### 5. Identify the opportunity
Explain why the business could be relevant to the student population and suggest a possible benefit without assuming the business has agreed to it.

### 6. Create the outreach angle
Generate a short, personalized reason for contacting the business and a suggested opening.

### 7. Human review
The human reviewer decides whether the prospect is ready for outreach.

### 8. Mary's Next Move
The agent gives one practical next action based on the current evidence and unresolved questions.

## Portfolio note

This repository contains the reusable workflow, instructions, templates, and a sanitized example. A separate working spreadsheet can be used for live prospect research and should not be published here when it contains operational contact information or other data that does not belong in a public portfolio.

## Why I built it

I built this project to demonstrate how AI can support real customer-success and business-development work without removing human judgment. The value is not simply finding businesses; it is creating a structured process that improves research quality, reduces unsupported assumptions, and turns research into an actionable next step.
