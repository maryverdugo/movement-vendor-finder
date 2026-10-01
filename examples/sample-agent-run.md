# Sample Agent Run

This example demonstrates how the Movement Vendor Finder workflow can turn a local-business research request into a structured, human-reviewable prospect.

## Request

Find potential local food and coffee vendors near the Pima Medical Institute Albuquerque campus.

**Target:** Pima Medical Institute — Albuquerque campus  
**Category:** Food and coffee  
**Initial geographic focus:** Approximately 1 mile  
**Preference:** Locally owned or independent businesses  
**Output:** Research findings, source notes, student-offer status, opportunity, outreach angle, and next step

## Agent Workflow

The agent follows this sequence:

SEARCH → VERIFY → RESEARCH CONTACT → CHECK EXISTING OFFER → IDENTIFY OPPORTUNITY → CREATE OUTREACH ANGLE → HUMAN REVIEW

## Example Prospect

**Business:** Example Local Café

**Category:** Coffee / Breakfast

**Location:** Near the target campus

**Local ownership:** Needs Research

**Decision-maker:** Needs Research

**Existing student discount:** No Offer Found in Sources Reviewed

**Potential student offer:** Consider a small Pima-specific benefit such as a percentage discount, free add-on, or student special.

## Why It May Be Relevant

The business is located near the target student population and serves products that may be relevant to students looking for convenient food and coffee options.

This is an opportunity for further research, not a recommendation that the business should automatically be contacted.

## Outreach Angle

Open with the business's proximity to the campus and the potential to provide a useful benefit to Pima students.

### Suggested Opening

"Hi, I'm reaching out because we're building a local student-benefit program for Pima Medical Institute students and are looking for independent businesses near campus that may be interested in participating."

## Mary's Next Move

Verify the business's current ownership and identify an appropriate public business contact before considering outreach.

## Human Review

The agent does not contact the business or make the final vendor decision.

Mary reviews the evidence, verifies unresolved information, decides whether the business is appropriate, and approves any outreach.

## Guardrails Demonstrated

- Do not invent ownership.
- Do not guess the decision-maker.
- Do not infer an email address.
- Do not claim that a business has no student offer unless the sources reviewed support that conclusion.
- Do not treat a general promotion as a student discount.
- Do not automatically contact a business.
- Flag conflicting or incomplete information for human review.

## Portfolio Note

This is a sanitized example. It intentionally uses a fictional business rather than publishing real vendor contact information.
