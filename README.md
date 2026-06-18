# SaaS Roadmap Strategist

`plan-saas-roadmaps` is a Codex skill for turning SaaS product ideas, requirements, notes, uploaded planning materials, and public product context into professional technology roadmaps from MVP through scale and enterprise readiness.

It is designed for founders, product leaders, CTOs, agencies, and technical teams who need a roadmap that is clear enough for business planning and specific enough for engineering review.

## What It Produces

The skill helps create phased SaaS technology roadmaps covering:

- MVP, early traction, growth, scale, and enterprise-readiness phases.
- Product scope, platform priorities, and delivery sequencing.
- Architecture, database, API, integration, auth, billing, and DevOps direction.
- Security, privacy, reliability, observability, testing, and release gates.
- Team composition, hiring needs, dependencies, tradeoffs, and technical debt.
- Scalability triggers and re-architecture signals.

## When To Use It

Use this skill for requests like:

- "Build a SaaS roadmap for my B2B analytics product."
- "Turn these product requirements into an MVP-to-scale technical plan."
- "Create a CTO-level roadmap for fundraising and engineering execution."
- "Plan the architecture, billing, security, and enterprise milestones for this SaaS."
- "Review this SaaS idea and tell me what to build now versus later."

## Skill Contents

```text
plan-saas-roadmaps/
  SKILL.md
  README.md
  agents/
    openai.yaml
  references/
    roadmap-checklist.md
```

- `SKILL.md` contains the runtime instructions and trigger metadata.
- `references/roadmap-checklist.md` provides a deeper checklist for comprehensive roadmap coverage.
- `agents/openai.yaml` provides UI metadata for Codex skill lists and default invocation.


## Example Prompt

```text
Use $plan-saas-roadmaps to build a phased SaaS technology roadmap for a B2B compliance workflow product. The target users are operations managers, the business model is seat-based subscriptions, and the first version needs workflow approvals, audit logs, notifications, and basic reporting.
```

## Design Notes

The skill favors pragmatic SaaS architecture: start with the smallest credible MVP, design tenant and data boundaries early, defer enterprise complexity until justified, and tie scaling investments to measurable product, customer, operational, or compliance triggers.

It avoids making unsupported claims about market traction, compliance status, security certifications, budgets, or traffic levels when the user has not provided that information.
