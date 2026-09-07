# ProofScope — Week 4 Packet

## Problem
Students can have real project evidence, but that evidence can lose its meaning when reused in another role or employer context.

## Exact user
A student who owns project evidence and wants to reuse it for another opportunity while keeping control of sharing.

## Success
Before the module closes, a student can select synthetic project evidence, choose another role/employer context, receive a verification or mismatch result, and request human review after a mismatch.

## Flow

```mermaid
flowchart TD
A[Student opens ProofScope] --> B[View projects]
B --> C[Select evidence]
C --> D[Choose new role and employer]
D --> E[Verify context]
E --> F{Role and employer match?}
F -->|Yes| G[Context verified]
F -->|No| H[Context mismatch]
H --> I[Not verified for this context]
I --> J[Request human review]
J --> K[Human final authority]
Benchmark

The best existing solutions for career discovery and learning include LinkedIn, Handshake and Coursera. ProofScope differs by testing context-specific proof instead of discovery, learning, ranking or career recommendation.

Long view

If this slice works, ProofScope could become a student-controlled evidence layer where project proof stays tied to the context where it was authorized. The product could help organizations review evidence without becoming a ranking or profiling engine. Human authority and student control remain core constraints.

Scope cut

No hiring recommendation, ranking, profiling, potential prediction, career recommendation, real personal data or automatic sharing.

Architecture
Frontend: HTML/CSS/JavaScript
Structured data: synthetic project data
Hosting: GitHub Pages
AI: no live AI call in MVP
Security: no secrets and synthetic data only
Test plan

Mechanical pass: test matching and mismatching contexts, identify a bug, fix it and redeploy.

Persona pass: test the product with a synthetic student, log confusion and fix the most important issue.
