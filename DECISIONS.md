# ProofScope — Decisions

## Product
ProofScope is a Proof-of-Skill prototype testing a context-transfer attack.

## Core rule
Evidence is authorized for a specific role and employer context.

A context mismatch does NOT mean lack of ability. It means the evidence was not verified for the selected context.

## Constraints
- Synthetic data only.
- Student controls sharing.
- Human review has final authority.
- No automatic sharing.
- No ranking.
- No profiling.
- No hiring recommendation.
- No career prediction.
- No personality or potential scoring.

## Testing
Project 1:
- Data Analyst + Empresa A = verified.
- Data Analyst + Empresa B = mismatch.
- Marketing Analyst + Empresa A = mismatch.

Project 2:
- Research Assistant + Mercado Claro = verified.
- Research Assistant + Empresa A = mismatch.
- Data Analyst + Mercado Claro = mismatch.

## Mechanical bug fixed
Project 2 originally had an authorized context that was not available in the selector. Research Assistant and Mercado Claro were added so the authorized context could actually be tested.

## Persona
Synthetic persona: Valeria, 21, Business Administration student.

Main confusion tested:
“Not verified” must not be interpreted as “not skilled.”

The interface explicitly explains this distinction.
